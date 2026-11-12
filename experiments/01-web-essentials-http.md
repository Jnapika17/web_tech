# Experiment 1: Web Essentials, HTTP Requests and Responses, and Web Servers

## Aim
Understand how a browser requests resources from a web server.

## Steps
1. Open a website and inspect its Network tab in browser developer tools.
2. Identify the request URL, method, status code, and response content type.
3. Compare a successful response (such as `200 OK`) with a missing page (`404 Not Found`).

## Example
```http
GET / HTTP/1.1
Host: localhost:3000
```

```http
HTTP/1.1 200 OK
Content-Type: text/html
```

## Result
Observed the HTTP request/response cycle between a client and server.
