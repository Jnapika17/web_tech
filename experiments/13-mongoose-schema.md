# Experiment 13: Mongoose Schemas, Models, and Queries

## Aim
Define a Mongoose schema and use its model to query MongoDB.

## Steps
1. Install Mongoose and connect to a MongoDB database.
2. Define a schema with field types and validation.
3. Create a model and use it to create and find documents.

## Example
```js
const mongoose = require("mongoose");

const studentSchema = new mongoose.Schema({
  name: { type: String, required: true },
  age: { type: Number, min: 0 },
  course: String
});

const Student = mongoose.model("Student", studentSchema);
```

## Result
Defined a validated model for creating and querying student documents.
