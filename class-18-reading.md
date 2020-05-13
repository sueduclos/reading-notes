[Home Page](https://sueduclos.github.io/reading-notes/)

## Class 18: Socket.io

### Links

- [Web Sockets](https://en.wikipedia.org/wiki/WebSocket)                     
- [Socket.io Tutorial](https://www.tutorialspoint.com/socket.io/)            
- [Socket.io vs Web Sockets](https://www.educba.com/websocket-vs-socket-io/) 
- [Socket.io Documentation](https://socket.io/docs/)                         
- [Socket.io Server API](https://socket.io/docs/server-api)                  
- [Socket.io Client API](https://socket.io/docs/client-api)                  
- [Socket Testing Tool](https://amritb.github.io/socketio-client-tool/)  
                                              

### Vocabulary
- WebSocket : A communication protocol, where the client can talk to the server and the server can talk to the connected clients. This protocol is different from HTTP, but WebSocket is designed to work _over_ HTTP, thus making it compatible with HTTP. All WebSocket communication is done over TCP. 
- socket.io : A package that builds upon the WebSocket protocol, and makes it very seamless to communicate events between clients and servers.                                                                                                                                                            
- client    : A client in the context of this class is any application that is connecting to a server, with the goal to share data and events over TCP, with connection being maintained over HTTP.                                                                                                       
- server    : A server in the context of this class is any application that allows multiple clients to connect to it, with the connection maintained over HTTP, and the data transfer happening over TCP.

### Discussion Questions:

#### 1.What does it mean that web sockets are bidirectional? Why is this useful?
Bidirectional means two-way. It is useful because, its capable of both sending and receiving. 

#### 2. Does `socket.io` use HTTP? Why?
Yes. The HTTP layer is to ensure that the connection between the client and server is kept active and authenticated.

#### 3. What happens when a client emits an event? What happens when a server emits an event? 
Client emits event - 
Server emits event -
