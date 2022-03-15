[Live URL](https://mujahedyousef.github.io/advanced-js-reading-notes.-/day_10/class_10.html)

# Readings: Event Driven Applications

----

## Review, Research, and Discussion

> Q1 : Why is access control important?

* mitigate the risk of information being accessed without the appropriate authorization, unlawfully, and the risk of a data breach.

> Q2 : Describe an application that would need access control?

* use it at Role-Based Access Control. Permissions are allocated only with enough access as needed for employees to do their jobs.

> Q3 : Describe an application that would need access control?
*used to determine permission for any user and determine access and jobs to can use it

> Q4 :Why is role based access control more scalable than discretionary or mandatory access control?

* Role-based access control grants access privileges based on the work that individual users do.
* Discretionary access control decentralizes security decisions to resource owners. The owner could be a document’s creator or a department’s system administrator.
* Mandatory access control uses a centrally managed model to provide the highest level of security.

* the four most common access control models:

1. Mandatory Access Control (MAC)
2. Discretionary Access Control (DAC)
3. Role-Based Access Control (RBAC)
4. Privileged Access Management (PAM)

* [Read more](https://www.twingate.com/blog/access-control-models/)

----
| Term|Mean|
|----|----|
|Authorization| the process of giving someone permission to do or have something.|
|Role Based Access Control|Is an approach to restricting system access to authorized users.|
|Capabilities|The access rights that are given user to determine what allow actions|
----

## Event-Driven Programming in Node.js

* **Is a logical pattern that we can choose to confine our programming within to avoid issues of complexity and collision.**

> **The basic components of an Event-Driven Program are:**

* A callback function ( called an event handler) is called when an event is triggered.
* An event loop that listens for event triggers and calls the corresponding event handler for that event.

> **EventEmitter:** The EventEmitter is a Node module that allows objects to communicate with one another. The core of Node’s asynchronous event-driven architecture is EventEmitter. Many of Node’s built-in modules inherit from EventEmitter.

* How to do?

> emitter objects send out named events, which trigger listeners that have already been registered. Hence,  an  emitter object has ***two key characteristics:***

1. mitting name events: The signal that something has happened is called emitting an event. A status change in the emitting object is often the cause of this condition.
2. Registering and unregistering listener functions: It refers to the binding and unbinding of the callback functions with their corresponding events.

> Event-Driven Programming Principles:

1. A suite of functions for handling the events.These can be either blocking or non-blocking, depending on the implementation.
2. Binding registered functions to events.
3. When a registered event is received, an event loop polls for new events and calls the matching event handler(s).

[Read more](https://www.geeksforgeeks.org/explain-event-driven-programming-in-node-js/)

 [More photos](https://prezi.com/5gtq0roq7wx9/event-driven-programming/)
