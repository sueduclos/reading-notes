[Home Page](https://sueduclos.github.io/reading-notes/)

## Class 12: OAuth

### Links                                                       

- [OAuth2 simplified](https://aaronparecki.com/oauth-2-simplified/)                                         
- [What is OAuth Really All About?](https://www.youtube.com/watch?v=t4-416mg6iU)                            
- [OAuth wiki](https://en.wikipedia.org/wiki/OAuth)                                                         
- [Build a Node API with OAuth](https://developer.okta.com/blog/2018/08/21/build-secure-rest-api-with-node) 

### Vocabulary
- client ID:    The `client_id` is a public identifier for an application. When you register your application with a third party such as Google, a client ID is produced to refer to your application publicly. You can think of this as your "record id" in the database of registered applications that Google stores.

- client secret: The `client_secret` is a hidden string known only to the application and the third party such as Google. You can think of this as your "password" in the database of registered applications that Google stores. With the combination of `client_id` and `client_secret`, you allow Google to know that you're a registered application.              

- authentication endpoint: This is a URL that any third party OAuth provider has implemented. This page usually allows a user to sign into their third party account, and verify that they want to share data with your server application. Then, a redirect happens back to your server.                                                                                       

- access token endpoint: This is an endpoint that any third party OAuth provider has implemented. Making a request to this endpoint should provide you with an access token for the signed-in user.                                                                                                                                                               
- API endpoint: This is any endpoint that a third party OAuth provider has implemented. We say "API endpoint" typically when we refer to an endpoint that gives us user data or lets us do some user action. This is different from the "authentication endpoint" and "access token endpoint", which are part of the sign-in process and don't give actual user data. 

- authorization code: This is a code that allows a server application to request an access token. It is generated from the authentication endpoint, after a user has signed-in and verified that your server application has permission.                                                                                                                                   
- access token: This is a token that represents a signed in user on a third party application. With this token, you can request from an API endpoint to get user data or carry out user actions.                                                                                                                                                                     
- OAuth: An open standard for access delegation - this is a standard way for independent applications to share sensitive user data.                                                                                                                                                                                                                           

### Discussion Questions:

#### 1. What's a benefit of using OAuth instead of your own basic authentication?
It allows limited access to the user's data and allows accessing when authorization tokens expire. It has ability to share data for users without having to release personal information. It is easier to implement and provides stronger authentication.

#### 2. Write the following steps in the correct order:
    ```
    - Ask the client if they want to sign in via a third party
    - Redirect to a third party authentication endpoint
    - Receive authorization code
    - Make a request to the access token endpoint
    - Receive access token
    - Make a request to a third-party API endpoint
    - Register your application to get a `client_id` and `client_secret` 
    ```
    
#### 3. What can you do with an authorization code?
The authorization code tells us that the client/user has allowed the server to read data from the user's Google account. The authorization code is a temporary code that the client will exchange for an access token. The code itself is obtained from the authorization server where the user gets a chance to see what the information the client is requesting, and approve or deny the request.

#### 4. What can you do with an access token?
An access token is basically a "signed in user". Anyone who has an access token can act as an authenticated user, doing any of the actions specified in the scope originally provided. Access tokens are the thing that applications use to make API requests on behalf of a user. The access token represents the authorization of a specific application to access specific parts of a user's data. Access tokens must be kept confidential in transit and in storage.
