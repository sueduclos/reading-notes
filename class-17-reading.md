[Home Page](https://sueduclos.github.io/reading-notes/)

## Class 17: TCP Server

### Links

- [OSI Model Explained](https://www.youtube.com/watch?v=vv4y_uOneC0) 
- [TCP Handshakes Explained](https://www.youtube.com/watch?v=xMtP5ZB3wSk)
- [OSI Model](https://www.cloudflare.com/learning/ddos/glossary/open-systems-interconnection-model-osi/)
- [What is TCP](https://searchnetworking.techtarget.com/definition/TCP)
- [Build a TCP Server (code only)](https://techbrij.com/node-js-tcp-server-client-promisify)
- [Net Module Documentation](https://nodejs.org/api/net.html)
                                              

### Vocabulary
- OSI Model         : The Open Systems Interconnection model is a conceptual model that describes the process of transferring data from source to destination. Each layer of the model feeds into the next layer, and each layer specifies some common protocols to use at that step of the process.
- TCP/IP Model      : The Internet Protocol Suite, or the TCP/IP model, is a simplified version of the OSI model, specifically suited for data transfer between internet applications. 
- TCP               : The Transmission Control Protocol is a reliable way to transport packets of data over the internet. TCP is connection-oriented, and a connection between the source and destination is established before data can be sent. 
- UDP               : The User Datagram Protocol is a simple connectionless communication between the source and destination, so there is no guarantee of delivery. This can be beneficial in some cases, since UDP avoids some overhead time that TCP relies on. 
- packets           : A kilobyte of information that represents a piece of a larger data stream. All packets have a header. 
- header            : The packet header provides valuable information about the packet, the source application and the destination application. This information can be used to verify packet security, reassemble multiple packets into the original data stream, and more! 
- socket server     : A TCP socket server is an application that sends data to other applications. 
- socket connection : A TCP socket connection is an application that subscribes to and receives data from a TCP socket server. 

### Discussion Questions:

#### 1. What do the layers in the OSI and TCP/IP models represent? 
They are a series of rules and structure so that security is ensured and both applications know what to do at each step of the process.

#### 2. What is the benefit of transforming data into packets? 
The benefit is that these packets are about one kilobyte in size, so that they’re easy to send over the internet. 

#### 3. UDP is often referrered to as a *connectionless* protocol. Why is this? 
The server is continually sending another server some simple information. When transferring data it doesn’t establish a strong secure connection between the sending server and the receiving server.

#### 4. Can a socket server application have multiple socket connections? Can a socket connection application be connected to multiple socket servers? Can an application be both a socket server and a socket connection? 
Yes, there can be multiple socket connections listening in on a single socket server. Typically one is “serving out” data for the second to consume. 
