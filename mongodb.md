

#### Delta dump of all MongoDB collections
```sh
#!/bin/bash

# Set MongoDB connection details
MONGODB_HOST="localhost"
MONGODB_PORT="27017"
MONGODB_DATABASE="crm_db"

# Output directory
out_dir="/opt/${MONGODB_DATABASE}"
mkdir -p $out_dir

# Set start and end dates of the date range to search within
START_DATE="2024-05-25T06:00:00.000Z"
END_DATE="2024-05-26T06:00:00.000Z"

# Connect to MongoDB and retrieve documents within date range
start_timestamp=$(printf '%x' $(date -d "${START_DATE}" +%s))
end_timestamp=$(printf '%x' $(date -d "${END_DATE}" +%s))
start_id="${start_timestamp}0000000000000000"
end_id="${end_timestamp}ffffffffffffffff"

query="{\"_id\": { \"\$gte\": {\"\$oid\" :\"${start_id}\"}, \"\$lte\": {\"\$oid\": \"${end_id}\"} } }"
collections=`echo "show collections" | mongo $MONGODB_DATABASE --quiet`

for collection in $collections;
do
  echo "Exporting collection ${collection} ..."  
  mongoexport --host "${MONGODB_HOST}" --port "${MONGODB_PORT}" --db "${MONGODB_DATABASE}" --collection "${collection}" --query "${query}" --out "${out_dir}/${collection}".json
done

# Compress the output directory
zip -r /opt/${MONGODB_DATABASE}-new.zip ${MONGODB_DATABASE}

# Print output
echo "Documents in ${MONGODB_DATABASE}'s  collections are created between ${START_DATE} and ${END_DATE}:" 
```
