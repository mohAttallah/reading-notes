### 1- Web Socket
WebSocket is a computer communications protocol, providing full-duplex communication channels over a single TCP connection. 

WebSocket are Located in layer 7 in the OSI model at Network Architecture

### 2- WebSockect (request/response handshake)

![WebSockect handshake](https://upload.wikimedia.org/wikipedia/commons/1/10/Websocket_connection.png)

To establish a WebSocket connection, the client sends a WebSocket handshake request, for which the server returns a WebSocket handshake response,
The handshake starts with an HTTP request/response, allowing servers to handle HTTP connections as well as WebSocket connections on the same port. Once the connection is established, communication switches to a bidirectional binary protocol which does not conform to the HTTP protocol.
### 3-
Web Sockets provide a standardized way for the server to send content to a client without first receiving a **requested** from that client.

---
### event handler io.on()
The event handler io.on() is used in the context of Socket.IO library. It allows you to define event handlers for various events emitted by the Socket.IO

### Describe some possible proof of life or proof that the code works as expected

1- Test Scenarios: Develop a collection of test scenarios that encompass various facets of your code's functionality.
2- Peer Review: Participate in a peer review process where seasoned developers assess your code for logical flaws, compliance with industry standards, and possible bugs.
3- User Validation Testing: Engage end-users or stakeholders to conduct user validation testing, ensuring the code meets their acceptance criteria.

###  socket.emit()
socket.emit() is a function in Socket.IO that sends custom events from the client to the server (or vice versa) over a WebSocket connection, enabling real-time communication between the two.

----
### The relationship between WebSocket and Socket.IO 

WebSocket is a lower-level protocol that enables real-time bidirectional communication between a client and a server. Socket.IO, on the other hand, is a higher-level library built on top of WebSocket that provides additional features, fallback mechanisms, and ease of use, making it a more comprehensive and flexible solution for real-time communication. The relationship between WebSocket and Socket.IO is similar to Git and GitHub or OAuth and Auth0, where the latter builds upon the former to offer enhanced functionality and convenience.

### When would you use Socket.IO?

Socket.IO is used when you need real-time, bidirectional communication between clients and servers. It provides broadcasting capabilities, platform compatibility, automatic WebSocket upgrade, custom protocol implementation, and event-based functionality. It requires client-side and server-side libraries and offers reserved events for both sides.

### When would you use Socket.IO?
WebSocket is beneficial in various scenarios that require real-time, bidirectional communication between a client and a server. Some use cases for WebSockets include live chat applications, real-time collaboration tools, multiplayer online games, stock market tickers, sports score updates, and any application where immediate data updates and real-time interaction are essential.



