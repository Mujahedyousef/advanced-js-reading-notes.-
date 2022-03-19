[live URL](https://mujahedyousef.github.io/advanced-js-reading-notes.-/day_11/class_11.html)

# Readings: Socket.io

----

## Review, Research, and Discussion

* Q1: What is the benefit of transforming data into packets?

>Answer : enable new innovations, services, and business opportunities

* Q2: UDP is often refereed to as a connectionless protocol. Why is this?

>Answer :UDP is a connectionless protocol. It is known as a datagram protocol because it is analogous to sending a letter where you don't acknowledge receipt.

* Q3: Can a socket server application have multiple socket connections?

>Answer : Multiple connections on the same server can share the same server-side IP/Port pair as long as they are associated with different client-side IP/Port pairs.

* Q4: Can a socket connection application be connected to multiple socket servers?

>Answer : You cannot use a single socket to connect to multiple servers. You must create a separate socket for each connection.

* Q5: Can an application be both a socket server and a socket connection?

>Answer :  Can use the same socket for whatever you want, as long as your protocol handles it.

----
| Term|Mean|
|----|----|
|Observer Pattern|Is used when there is a one-to-many relationship between objects such as if one object is modified, its dependent objects are to be notified automatically. |
|Listener|The object that receives a notification (an object that implements the Event interface) when an event of the specified type occurs. |
|Event Handler|This is a block of code (usually a JavaScript function that you as a programmer create) that runs when the event fires.|
|Event Driven Programming|Is a programming paradigm in which the flow of program execution is determined by events.|
|Event Loop|is responsible for executing the code, collecting and processing events, and executing queued sub-tasks.|
|Event Queue| is responsible for sending new functions to the stack for processing.|
|Call Stack|is a mechanism for an interpreter (like the JavaScript interpreter in a web browser) to keep track of its place in a script that calls multiple functions. |
|Emit|Certain kinds of objects (called "emitters") periodically emit named events that cause Function objects ("listeners") to be called.|
|Raise| defining an exception|
|Trigger|triggers the specified event and the default behavior of an event (like form submission) for the selected elements.|
|Subscribe|function is similar to the Promise.then()|
|database|an organized collection of structured information, or data, typically stored electronically in a computer system.|

----

## WebSocket

> is a computer communications protocol, providing full-duplex communication channels over a single TCP connection.
![websocket](/day_11/websocketj.png)
[read More](https://en.wikipedia.org/wiki/WebSocket)

----

## Socket.io

>is a JavaScript library for real-time web applications.

> It enables real-time, bi-directional communication between web clients and servers. It has two parts − a **client-side library that runs in the browser**, and **a server-side library for node.js.** Both components have an identical API.

* Why Socket.IO?

> Sockets have traditionally been the solution around which most real-time systems are architected, providing a bi-directional communication channel between a client and a server. This means that the server can push messages to clients. Whenever an event occurs, the idea is that the server will get it and push it to the concerned connected clients.

* where using?

> used by Microsoft Office, Yammer, Zendesk, Trello and JavaScript frameworks on GitHub.

![socket.io](/day_11/socket.jpg)
----

## Difference Between WebSocket and Socket.io

* WebSocket is the communication Protocol that provides bidirectional communication between the Client and the Server over a TCP connection; WebSocket remains open all the time, so they allow real-time data transfer. When clients trigger the request to the server, it does not close the connection on receiving the response; it rather persists and waits for the Client or server to terminate the request.

* Socket.IO is a library that enables real-time and full-duplex communication between the Client and the Web servers. It uses the WebSocket protocol to provide the interface. Generally, it is divided into two parts; both WebSocket vs Socket.io are event-driven libraries.
----

## Resources
* [OSI Model Explained](https://www.youtube.com/watch?v=vv4y_uOneC0)
* [TCP Handshakes Explained](https://www.youtube.com/watch?v=xMtP5ZB3wSk)
* [Socket.io Documentation](https://socket.io/docs/v4/)
* [Socket.io Server API](https://socket.io/docs/v4/server-api)
* [Socket.io Client API](https://socket.io/docs/v4/client-api)
* [Socket Testing Tool](https://amritb.github.io/socketio-client-tool/)
