[Home Page](https://sueduclos.github.io/reading-notes/)

## Class 07 Reading - Express

### Links
- [Express Middleware Explained](https://www.youtube.com/watch?v=9HOem0amlyg)             
- [Using Express Middleware](https://expressjs.com/en/guide/using-middleware.html)       
- [Express Middleware](https://www.tutorialspoint.com/expressjs/expressjs_middleware.htm) 
- [Using Express Routing](https://expressjs.com/en/guide/routing.html)                    
- [Supertest](https://github.com/visionmedia/supertest)                                   
- [Express Middleware List](https://expressjs.com/en/resources/middleware.html)           
- [HTTP Status Codes](https://www.restapitutorial.com/httpstatuscodes.html)

### Vocabulary
- Express
- endpoint
- routing
- query
- event
- application middleware
- route middleware
- error middleware

### Discussion Questions:

#### 1. What code does the server actually run?
It waits for events to fire and then responds to those events and runs the code defined. 

#### 2. What Express/HTTP operations map to CRUD operations?
POST, GET, PUT, DELETE
```javascript
app.post('/products', (req, res) => {
    // CREATE PRODUCT
});

app.get('/products', (req, res) => {
    // READ PRODUCTS
});

app.put('/products/:id', (req, res) => {
    // UPDATE PRODUCT WITH ID req.params.id
});

app.delete('/products/:id', (req, res) => {
    // DELETE PRODUCT WITH ID req.params.id
});
```

#### 3. What does `res.send()` do? 
It is used to send data back to the client in the properly formatted way.
 
#### 4. What is the order of operations for the three categories of middleware (handler, application, route)?
-   Application Middleware
    -   Run whenever the server receives a request
    -   Useful for generic server actions like JSON parsing, error handling, etc.
    -   Can be set to run only when a request belongs to a specific method (`GET`, `POST`, `PUT`, `DELETE`)
-   Route Middleware
    -   Runs whenever the server receives a request to a specific url endpoint
    -   Will execute for any method request on that route (`GET`, `POST`, `PUT`, `DELETE`)
    -   Useful for authentication, authorization, etc.
-   Handler Middleware
    -   Runs when the server receives a specific method request (`GET`, `POST`, `PUT`, `DELETE`) to a specific route
    -   The handler allows you to provide a list of functions
    -   This list is exectued from left to right

#### 5. What is the parameter `next` used for?
To call the next middleware in the chain.
