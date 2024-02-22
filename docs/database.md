#### [Best practices for schema changes and data migrations to a live database without downtime](https://dba.stackexchange.com/questions/10913/best-practices-for-schema-changes-and-data-migrations-to-a-live-database-without?rq=1)
1. Create the new structure in parallel
2. Start writing to both structures
3. Migrate old data to the new structure
4. Only write and read new structure
5. Delete old columns

As for step 3, use something like this (in one transaction):

Insert what is not there yet:
```sql
INSERT INTO new_tbl (old_id, data)
SELECT old_id, data
FROM   old_tbl
WHERE  NOT EXISTS (SELECT * FROM new_tbl WHERE new_tbl.old_id = old_tbl.old_id);
```

Update what has changed in the meantime:
```sql
UPDATE new_tbl
SET    data  = old.data
USING  old_tbl
WHERE  new_tbl.old_id = old_tbl.old_id
AND    new_tbl.data IS DISTINCT FROM old_tbl.data;
```
New data will not be touched, because it is identical in both places.


#### [Data Archival Strategy](https://dba.stackexchange.com/questions/27577/data-archival-strategy-that-handles-schema-changes?rq=1)
* Why is archiving necessary? It sounds like the system already handles old data, so what does the business need to separate this data? Performance?
* Is archive data a read-only snapshot, or are historical data changes possible? If changes are possible, which types of changes will be supported (insert, update, delete, or some combination of those)?
* Is the database multi-tenant, and if so, do you require the ability of each tenant to be able to archive at different points in time?
* Does your application need to run with the archive data as a data source? I'm assuming yes since you mention synchronizing schema changes.
* What is the minimum version/edition of the DBMS you need to support? This will determine which features are available to use in your strategy.
* How much time do you have to implement archiving? Archiving is a very low-level design issue that ideally should be baked in right from the start; adding it on later can potentially take a significant amount of time to redesign and implement.
* Avoid multiple databases if at all possible, particularly if you require the ability to edit historical data.
