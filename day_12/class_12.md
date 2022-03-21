[Link URL](https://mujahedyousef.github.io/advanced-js-reading-notes.-/day_12/class_12.html)

# Readings: Message Queues

----

## Review, Research, and Discussion

>Q1: What does it mean that web sockets are bidirectional? Why is this useful?
>
* BIDIRECTIONAL.  WebSockets allow for full-duplex bidirectional communication. This enables the server to send real-time updates asynchronously, without requiring.

>Q2:Does socket.io use HTTP? Why?
>
* Yes, It does. and will use HTTP long-polling as fallback.

>Q3:What happens when a client emits an event?
>
* It triggers events in the server and listens to events.

>Q4:What happens when a server emits an event?
>
* These events trigger for all the clients that are connected to this server.

> Q5 : What happens if a client “misses” an event?
>
* When mistakes happen it’s important to be honest and identify where errors have occurred.

>Q6 : How can we mitigate this?
>
1. Report it to your line manager or group leader and make a written record with them.
1. Assess with your manager whether the Risk Assessment and Client Support Plan was clear enough to prevent the mistake that occurred. Re-assess or re-word as necessary.
1. Learn from it.

----
| Term|Mean|
|----|----|
|Socket|Is one endpoint of a two-way communication link between two programs running on the network.|
|Web Socket|Is an advanced technology that makes it possible to open a two-way interactive communication session between the user's browser and a server. |
|Socket.io|is a library that enables low-latency, bidirectional and event-based communication between a client and a server.|
|Client|Is any computer hardware or software device that requests access to a service provided by a server.|
|Server|is a computer or system that provides resources, data, services, or programs to other computers.|
|OSI Model|describes seven layers that computer systems use to communicate over a network.|
|TCP Model|refers to Transmission Control ProtocolTCP/IP has 4 layers. [read more](https://www.geeksforgeeks.org/tcp-ip-model/)|
|TCP|  **Transmission Control Protocol** is one of the main protocols of the Internet protocol suite. |
|UDP|User datagram protocol (UDP) operates on top of the Internet Protocol (IP) to transmit datagrams over a network.|
|Packets|Is a small segment of a larger message.|
----

## Socket.io Chat Example

> Writing a chat application with popular web applications stacks like LAMP (PHP) has normally been very hard. It involves polling the server for changes, keeping track of timestamps, and it’s a lot slower than it should be.

> Sockets have traditionally been the solution around which most real-time chat systems are architected, providing a bi-directional communication channel between a client and a server.

> This means that the server can push messages to clients. Whenever you write a chat message, the idea is that the server will get it and push it to all other connected clients.
[read more](https://socket.io/get-started/chat)
