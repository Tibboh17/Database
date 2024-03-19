# MongoDB
- Open source NoSQL database management system.
- Manage document-oriented information, store or retrieve information.

# BSON
- Binary JSON
- MongoDB manages data based on BSON.
- Search and process data rapidly.
```JSON
{
    name: "sue,
    age: 26,
    status: "A",
    groups: ["news", "sports"]
}
```

# Create
- Add new documents to a collection.
```
db.users.insertOne(
    {
        name: "sue",
        age: 26
    }
);

db.products.insertMany(
    [
        { _id: 13, item: "envelopes", qty: 60 },
        { _id: 13, item: "stamps", qty: 110 },
        { _id: 14, item: "packing tape", qty: 38 }
    ]
);
```
# Read
- Retrieve documents from a collection.
```
```
# Update
- Modify existing documents in a collection.
# Delete
- Remove documents from a collection.
