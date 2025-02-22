#### Why MongoDB
- NoSQL: Schema less, Gives flexibility for the developers
- No or few relations among data
- Good for read / write heavy workloads
- Ideal for e-comerce, blogging / CMS, storing timeseries data (e.g. smart sensor data)

#### How it works
- Runs a DB Server which maitains DBs (similary to DBs in MySQL world)
- DB has multiple collections (equivalent to table in MySQL)
- Each collection stores data like a JSON structure (internally BSON), which is called **Document**

#### Data Types
- Number
- Boolean
- String
- Object
- Array

#### BSON (Binary + JSON)
- The data stored inside each MongoDB collection is in the form of JSON.
- BSON is the format used internally by the MongoDB storage engine
- It is efficient

#### MongoDB Properties
- No perdefined Schema
- No / fewer relations i.e. we maintain a nested / embedded documents
- When needed we can add more data or different document format on the same collection

#### Comparision with SQL
- Follow opposite concept or philosophy compare to SQL sometimes
- Schema & Relationship
- Normalized - Store data distributed across different tables
