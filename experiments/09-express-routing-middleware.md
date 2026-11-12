# Experiment 9: Express.js Routing and Middleware

## Aim
Handle requests in an Express application using routes and middleware.

## Steps
1. Install Express in the project.
2. Add middleware that logs each request and calls `next()`.
3. Create routes for `/` and `/about`.
4. Run the server and open each route.

## Example
```js
const express = require("express");
const app = express();

app.use((request, response, next) => {
  console.log(request.method, request.path);
  next();
});

app.get("/", (request, response) => response.send("Home"));
app.get("/about", (request, response) => response.send("About"));
app.listen(3000);
```

## Result
Created an Express application with request middleware and multiple routes.
