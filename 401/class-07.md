# Read 07

## Review

- What’s the difference between PUT and PATCH?
PUT updates the full item , PATCH updates a part of the item.

- Provide links to 3 services or tools that allow you to “mock” an API for development like json-server

Firebase
Mirage
Postman

- Compare and contrast Swagger and APIDoc.js 1 Which HTTP status codes should be sent with each type of (un)successful API call?

Swagger is the most widely used tooling ecosystem for developing APIs with the OpenAPI Specification (OAS). Swagger consists of both open source as well as professional tools, catering to almost every need and use case.

apiDoc creates a documentation from API descriptions in your source code.


- Compare and contrast SOAP and ReST
 
SOAP stands for Simple Object Access Protocol. REST stands for Representational State Transfer.
SOAP is a protocol. REST is an architectural pattern.


## Preparation summary

### Express middleware

Express is a routing and middleware web framework that has minimal functionality of its own: An Express application is essentially a series of middleware function calls.

Middleware functions are functions that have access to the request object (req), the response object (res), and the next middleware function in the application’s request-response cycle. The next middleware function is commonly denoted by a variable named next.

### Express routing

Routing refers to how an application’s endpoints (URIs) respond to client requests. For an introduction to routing, see Basic routing.

You define routing using methods of the Express app object that correspond to HTTP methods; for example, app.get() to handle GET requests and app.post to handle POST requests. For a full list, see app.METHOD. You can also use app.all() to handle all HTTP methods and app.use() to specify middleware as the callback function (See Using middleware for details).

