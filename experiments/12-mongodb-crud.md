# Experiment 12: MongoDB CRUD Operations

## Aim
Perform Create, Read, Update, and Delete operations on MongoDB documents.

## Steps
1. Insert one or more student documents.
2. Read documents with `find()` and a filter.
3. Update a document with `$set`.
4. Delete a document and verify the collection.

## Example
```javascript
db.students.insertOne({ name: "Asha", age: 20 })
db.students.find({ age: { $gte: 18 } })
db.students.updateOne({ name: "Asha" }, { $set: { age: 21 } })
db.students.deleteOne({ name: "Asha" })
```

## Result
Performed and verified MongoDB create, read, update, and delete operations.
