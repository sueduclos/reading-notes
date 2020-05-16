[Home Page](https://sueduclos.github.io/reading-notes/)

## Class 19: Message Queues

### Links

- [Rooms and Namespaces](https://socket.io/docs/rooms-and-namespaces/) 
- [Socket.io Emit Cheatsheet](https://socket.io/docs/emit-cheatsheet/) 
- [Messaging Queues \| System Design Basics](https://www.youtube.com/watch?v=sfQwMu0SCT8)  
                                              

A message queue server (or simply, queue server) runs independently and is tasked with routing events and messaging between clients. Any connected client can publish a message to the server, or subscribe to certain types of messages. 

### Discussion Questions:

#### 1. What is the main benefit of a message queue server? 
A queue server makes sure that all connected clients are up to date with the data they need. Subscribed clients can now "catch up" and pull down any events (or messages) they may have missed while disconnected.

#### 2. Why might we want to initiate messages from an HTTP request? 
So it can maintain a connection to the server.

#### 3. Is the Message Queue Server a socket.io client, a socket.io server, or an api server?
Its a socket.io server. 
