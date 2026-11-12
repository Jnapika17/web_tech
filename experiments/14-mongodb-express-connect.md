# Experiment 14: Connect MongoDB with Node.js and Express.js

## Aim
Connect an Express application to MongoDB through Mongoose.

## Steps
1. Store the MongoDB connection URI in an environment variable.
2. Connect with Mongoose and wait for the connection before listening.
3. Add an Express route that reads data from a model.
4. Handle connection and query errors explicitly.

## Example
```js
const mongoose = require("mongoose");
const express = require("express");

async function start() {
  await mongoose.connect(process.env.MONGODB_URI);
  const app = express();
  app.get("/", (request, response) => response.send("MongoDB connected"));
  app.listen(3000);
}

start().catch((error) => {
  console.error("Application startup failed:", error);
  process.exitCode = 1;
});
```

## Result
Connected an Express application to MongoDB using Mongoose.
