#### Why MongoDB
- NoSQL: Schema less, Gives flexibility for the developers
- No or few relations among data
- Good for read / write heavy workloads
- Ideal for e-comerce, blogging / CMS, storing timeseries data (e.g. smart sensor data)

#### How it works
- Runs a DB Server which maitains DBs (similary to DBs in MySQL world)
- DB has multiple collections (equivalent to table in MySQL)
- Each collection stores data like a JSON structure (internally BSON), which is called **Document**
- Storage engine manages data between Memory and File Storage for quick read and write

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
- Performance (read & write)

#### Ecosystem
- Self-managed / enterprise
- Atlas (Cloud)
- Mobile DB
- Compass GUI
- Drivers
- Shell (CLI)
- Stitch
  - Serverless Query API (e.g: Query directly from Reac.js app)
  - Serverless Functions - Allows to execute JavaScript functions directly similar to AWS Lambda or Google Cloud Functions
  - DB Triggers: a service listem to evens in DB like when document inserted, execute a function in response to that to send an e-mail informing user that document being inserted something like that
  - Real-time Sync: Synchronize data with cloud with mobile offline support

#### Use cases
MongoDB is better suitable for
- Operational Data
- Timeseries
- AI
- Streaming data
- Ful-text search
- Geospatial
- Graph
- Vector Search
