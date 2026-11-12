# Experiment 8: Node.js Modules and the HTTP Module

## Aim
Create a basic HTTP server using Node.js's built-in module.

## Steps
1. Save the example as `server.js`.
2. Run it with `node server.js`.
3. Visit `http://localhost:3000` in a browser.

## Example
```js
const http = require("node:http");

const server = http.createServer((request, response) => {
  response.writeHead(200, { "Content-Type": "text/plain; charset=utf-8" });
  response.end("Hello from Node.js");
});

server.listen(3000, () => console.log("Listening on port 3000"));
```

## Result
Started a Node.js HTTP server that sends a response to a browser.
