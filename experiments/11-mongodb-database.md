# Experiment 11: MongoDB Databases, Collections, and Documents

## Aim
Create a MongoDB database and store documents in a collection.

## Steps
1. Connect to MongoDB using `mongosh`.
2. Select or create a database and insert a document.
3. List the collection and inspect its documents.

## Example
```javascript
use studentDB
db.students.insertOne({ name: "Asha", course: "Web Technology" })
db.students.find()
```

## Result
Created a database collection and inserted a document.
