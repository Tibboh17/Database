# MongoDB
- Open source NoSQL database management system.
- Manage document-oriented information, store or retrieve information.

# BSON
- Binary JSON
- MongoDB manages data based on BSON.
- Search and process data rapidly.
```javascript
{
    name: "sue,
    age: 26,
    status: "A",
    groups: ["news", "sports"]
}
```

# Create
- Add new documents to a collection.
```javascript
db.collection.insertOne()
db.collection.insertMany()
```
<div align="center">
  <img src="https://github.com/TIBBOH17/Database/assets/121493257/857c40b0-6787-4299-a145-5002a1d08c26" width="70%">
</div>

# Read
- Retrieve documents from a collection.
```javascript
db.collection.find()
```
<div align="center">
  <img src="https://github.com/TIBBOH17/Database/assets/121493257/c25c8b78-1a99-4cc6-9bf7-3409f61c915f" width="70%">
</div>

# Update
- Modify existing documents in a collection.
```javascript
db.collection.updateOne()
db.collection.updateMany()
db.collection.replaceOne()
```
<div align="center">
  <img src="https://github.com/TIBBOH17/Database/assets/121493257/b88d1fa9-ed4c-4cd5-b406-61b930c5007a" width="70%">
</div>

# Delete
- Remove documents from a collection.
```javascript
db.collection.deleteOne()
db.collection.deleteMany()
```
<div align="center">
  <img src="https://github.com/TIBBOH17/Database/assets/121493257/4344a5dd-648e-45c0-b907-f43488967deb" width="70%">
</div>

# Aggregation Pipelines
<div align="center">
  <img src="https://github.com/TIBBOH17/Database/assets/121493257/812f07d5-5cee-4792-854f-d5defdc9525d" width="70%">
</div>

- Each stage performs an operation on the input documents.
- The documents that art output from a stage are passed to the next stage.
- An aggregation pipeline can return results for groups of documents.
