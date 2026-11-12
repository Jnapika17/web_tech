# Combined Practical 1: MongoDB Database and CRUD (Experiments 11 + 12)

## Aim
Create a MongoDB database and demonstrate CRUD operations on its collection.

## Steps
1. Select the `studentDB` database.
2. Create and populate the `students` collection.
3. Read documents, update a value, and delete a selected document.
4. Run a final query to verify the changes.

## Example
```javascript
use studentDB
db.students.insertMany([{ name: "Asha", age: 20 }, { name: "Ravi", age: 21 }])
db.students.find()
db.students.updateOne({ name: "Asha" }, { $set: { age: 22 } })
db.students.deleteOne({ name: "Ravi" })
db.students.find()
```

## Result
Created a database and demonstrated MongoDB CRUD operations.
