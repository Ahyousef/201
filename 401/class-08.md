# Read 08

## Review

- Name 3 real world use cases where you’d want to change the request with custom middleware
    - Validating data
    - Adding a time stamp to the request
    - Sending an obj instead of a string
- True or false: The route handler is middleware?
    False
- In what ways can a middleware function end the process and send data to the browser?
    Return, response.
- At what point in the request lifecycle can you “inject” middleware?
    Everywhere works.
- What can cause express to error with “Request headers sent twice, cannot start a second response”
    When you send two responses instead of one in the same request.


## Preparation summary

### Express routing

Routing refers to how an application’s endpoints (URIs) respond to client requests. For an introduction to routing, see Basic routing.

You define routing using methods of the Express app object that correspond to HTTP methods; for example, app.get() to handle GET requests and app.post to handle POST requests. For a full list, see app.METHOD. You can also use app.all() to handle all HTTP methods and app.use() to specify middleware as the callback function (See Using middleware for details).

The following code is an example of a very basic route.
```
var express = require('express')
var app = express()

// respond with "hello world" when a GET request is made to the homepage
app.get('/', function (req, res) {
  res.send('hello world')
})
```

### 

Express 4.0 comes with the new Router. Router is like a mini express application. It doesn't bring in views or settings, but provides us with the routing APIs like .use, .get, .param, and route.

we can:

Use express.Router() multiple times to define groups of routes
Apply the express.Router() to a section of our site using app.use()
Use route middleware to process requests
Use route middleware to validate parameters using .param()
Use app.route() as a shortcut to the Router to define multiple requests on a route


