# Combined Practical 3: Express Routing and REST API (Experiments 9 + 10)

## Aim
Build an Express application with middleware and REST routes.

## Steps
1. Add JSON parsing middleware and a request logger.
2. Implement routes for GET, POST, PUT, and DELETE.
3. Test each route with an HTTP client and verify its response.

## Example
```js
app.use(express.json());
app.use((request, response, next) => {
  console.log(request.method, request.path);
  next();
});

app.get("/items", listItems);
app.post("/items", createItem);
app.put("/items/:id", updateItem);
app.delete("/items/:id", deleteItem);
```

## Result
Created an Express API demonstrating routing, middleware, and REST methods.
