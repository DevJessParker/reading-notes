# Message Queues

## Discussion Questions

- What does it mean that web sockets are bidirectional? Why is this useful?

*Data flow occurs on the same channel. Sockets are kept open to receive data.*

- Does socket.io use HTTP? Why?

*No. It uses TCP which allows it to be much faster.*

- What happens when a client emits an event?

*The server can process the data if it has a listener event.*

- What happens when a server emits an event?

*All sockets with a listen event can hear the data.*

- What happens if a client “misses” an event?

*Nothing. The event is considered unhandled and is ignored.*

- How can we mitigate this?

*Establish edge case handlers to accept or manage all events emitted by a server.*

Term | Definition
----- | -----
Web Socket | A two-way communication channel over a TCP connection.
Socket | An endpoint of two-way data.
Socket.io | A javascript library giving access to event-driven methods.
Client | Receives the socket's data.
Server | Can request or receive event-driven data.
OSI Model | Framework model for networking system.
TCP Model | *Application Layer, Transport Layer, Internet Layer, Network Interface.*
TCP | Transmission Control Protocol that allows open event-driven data transfer below the http level.
UDP | Connectionless protocol that sends data without knowing if the endpoint is prepared to accept the data. 
Packets | A unit of data transferred over TCP

References:

https://www.guru99.com/tcp-ip-model.html