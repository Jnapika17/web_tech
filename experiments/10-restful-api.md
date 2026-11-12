# Experiment 10: RESTful APIs Using GET, POST, PUT, and DELETE

## Aim
Create REST endpoints that demonstrate the four common HTTP methods.

## Steps
1. Enable JSON request parsing with `express.json()`.
2. Add collection routes for listing and creating records.
3. Add item routes for updating and deleting a record by ID.
4. Test requests and inspect status codes and JSON responses.

## Example
```js
app.use(express.json());
app.get("/items", listItems);
app.post("/items", createItem);
app.put("/items/:id", updateItem);
app.delete("/items/:id", deleteItem);
```

## Result
Implemented and tested REST API routes for reading, creating, updating, and deleting data.
