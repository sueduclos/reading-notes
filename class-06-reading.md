[Home Page](https://sueduclos.github.io/reading-notes/)

## Class 06 Reading - HTTP and REST

### Links
- [HTTP Protocol Documentation](https://tools.ietf.org/html/rfc7231)
- [HTTP and REST](https://www.youtube.com/watch?v=Q-BpqyOT3a8) 
- [HTTP Basics](https://code.tutsplus.com/tutorials/http-the-protocol-every-web-developer-must-know-part-1--net-31177) 
- [json-server (npm)](https://github.com/typicode/json-server) 
- [Star Wars API Docs](https://app.swaggerhub.com/apis/ahardia/swapi/1.0.0#/) 
- [Swagger.io](https://swagger.io)                             
- [Swagger Inspector](https://inspector.swagger.io/builder)    
- [What is REST](https://restfulapi.net/)                      
- [Swagger Editor](https://editor.swagger.io)                  
- [HTTP Reference](https://code-maze.com/the-http-reference/)  
- [REST Reference](https://www.restapitutorial.com/lessons/httpmethods.html) 
- [Swagger Documentation](https://swagger.io/docs/)    

### Vocabulary
- server                                  
- HTTP                                    
- REST                                    
- request                                 
- response                                
- Web Request Response Cycle (WRRC)       
- HTTP status codes                       
- client                                  
- Application Programming Interface (API) 
- Swagger                                 
- REST Endpoint  

#### Common HTTP Status Codes

| Code | Name                          | Meaning                                                      |
| ---- | ----------------------------- | ------------------------------------------------------------ |
| 200  | OK                            | Generic success in sending the response                      |
| 201  | Created                       | The request was completed and a new data entry was created on the server |
| 202  | Accepted                      | The request has been accepted and an action that has been kicked off but not completed. When the action completes, another response will be sent. |
| 203  | Non-Authoritative Information | The server is a middleman, and recieved a 200 OK response from its request to another server. Now, when sending a response to the original client, the server will be modifying some of the data it recieved. |
| 204  | No Content                    | The server successfully processed the request and is not returning any content |
| 300  | Multiple Choices              | The client requested something that was ambiguous; for example they asked for something that is stored in multiple formats, or has a duplicate somewhere. The response does not include the requested data, but instead a list of the possible data entries the client should choose from. |
| 301  | Moved Permenantly             | The client requested something from a location that no longer holds that data |
| 304  | Not Modified                  | The client already requested this data, and the data has not changed since then. Instead of sending the same data again, the server sends nothing with a 304 response status code. |
| 400  | Bad Request                   | The client made some error when creating the request and so the server can't understand it. |
| 401  | Unauthorized                  | The server wanted the client to provide some authorization for security purposes, but the client did not |
| 403  | Forbidden                     | The client provided authorization, but the server is not willing to give a response (either the authenticated client doesn't have permissions to access this data, or some other reason) |
| 404  | Not Found                     | The requested data was not found on the server               |
| 405  | Method Not Allowed            | The server API doesn't support this method (GET, POST, PUT, DELETE, etc) on this data |
| 500  | Internal Server Error         | Generic server error                                         |
| 501  | Not Implemented               | The request is not recognized by the server and thus can't be completed |
| 502  | Bad Gateway                   | The server is also waiting on another server, and never got a response |
| 503  | Service Unavailable           | The server cannot handle the request because it is temporarily overloaded or down for maintenance |
| 504  | Gateway Timeout               | The server is also waiting on another server, but it took too long, resulting in a timeout= |


### Discussion Questions:

#### 1. What does protocol mean? 
A **protocol** is a set of rules that must be followed. HTTP was developed as a way for clients and servers to interact over the web in a consistent way.Protocol defines how messages are formatted and transmitted, and what actions Web servers and browsers should take in response to various commands.

#### 2. How does any web browser understand how to open any webpage? 
When you enter a Web address (URL) in your browser, this actually sends an HTTP command to the Web server directing it to fetch and transmit the requested Web page and display the information in your browser.

#### 3. Name one thing a request object *must* have, and one thing a response object *must* have
- **Request** object must have a `method`

- **Response** object must have a `status`

#### 4. What is the difference between HTTP and REST? 
**HTTP** is the protocol, set of rules that must be followed and **REST** is a collection of guidelines that call for a standard way to document API's. 

#### 5. Why is REST important?
The REST guidelines dictate how to format a server’s APIs so that a client can access all the methods / functionality they need.
