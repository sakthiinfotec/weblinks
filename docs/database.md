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
