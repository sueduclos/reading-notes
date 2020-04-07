[Home Page](https://sueduclos.github.io/reading-notes/)

## Class 08 Reading - Express Routing & Connected API

### Links
- [Using Express Routing](https://expressjs.com/en/guide/routing.html)
- [Express Routing](https://scotch.io/tutorials/learn-to-use-the-new-router-in-expressjs-4)

### Router (picture to follow)
There's a lot going on here! Let's tackle each step based on the numerical markings above: 

1. First, the client must build a request and send that off to a server. Clients can use many tools such as fetch, axios or SuperAgent to properly build and format a request. 
2. The properly formatted HTTP-compliant request is sent to our Express server, which should hopefully be live and running in order to accept that request. 
3. The server runs any pre-emptive middleware for the application or specific route. This middleware is usually modularized into discrete files, typically located in a `/middleware` folder. 
4. The server then runs the specific route + method handler middleware functions. Using `express.Router()`, we can now modularize these as well into discrete files, typically located in a `/routes` folder.
5. When running the handler middleware, there is a strong likelyhood that some data operation needs to take place. The handler function kicks off this asynchronous data operation by calling a model function such as `create()`, `read()`, `update()` or `delete()`. This refers to a model class built in a `/models` folder, utilizing a schema also defined in the `/models` folder. The handler then `awaits` this data operation to complete
6. The model CRUD functions themselves call MongoDB specific commands such as `save()`, `find()`, etc. This triggers the Mongoose schema to be called.  
7. The Mongoose schema runs any `pre`middleware, does any schema validation, and sends things off to the actual MongoDB database. 
8. After the MongoDB database makes the final data operation within the data store, the Mongoose schema can run its `post` middleware and then the async action can be marked as complete, with the Promise being resolved. Thus, the Express handler function is able to continue onwards, receiving some data from MongoDB. 
9. Having received some proof that the data operation was completed either successfully or unsuccessfully, the Express handler function can send a response to the client, setting the response status code and the response body to the expected data values. 

By the end of this class, you'll be tasked to implement an application that mimics this data flow. Try to keep files small and modular, and refer back to this diagram to understand how the pieces interact. 


### Discussion Questions:

#### 1. What is a benefit to using express.Router()
We can modularize specific rout + method handler mmiddleware functions into discrete files, typically located in a `/routes` folder.

#### 2. When I say that top-down order matters in Express, what does that mean?
Code in ran from the top of the page and then down the page in order. This means that even though Application Middleware is typically meant to be run before Handler Middleware, you can change this by moving an Application Middleware assignment after a Handler Middleware assignment. 

#### 3. Why do we use a model class (with create(), read(), etc.) instead of directly calling MongoDB operations (such as save(), find(), etc.) within our Express route handlers?
Due to asynchronous data operation being called. A model class is built in a /models folder, utilizing a schema also defined in the /models folder. The handler then awaits this data operation to complete.
