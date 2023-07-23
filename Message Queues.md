## Message Queues

### Caht Example
Chat  is a real-time messaging system built using React for the frontend, Node.js and Express.js for the backend, and Socket.IO for instant communication between users. 

### Proof of life

the "proof of life" we are getting on the backend is the successful establishment of a socket connection between the server and the client. The ``` io.on('connection', ...) ```event is triggered when a client successfully connects to the server using Socket.IO. This event serves as a confirmation that the server is alive and actively listening for incoming connections.

### Expect Port
To send a message to everyone except for a certain emitting socket in Socket.IO, you can use the ```.to()``` method along with the ```.emit() ```

---
### Room
A room is an arbitrary channel that sockets can join and leave. It can be used to broadcast events to a subset of clients

### Join to Room

You can call join to subscribe the socket to a given channel:

```Java Script

io.on("connection", (socket) => {
  socket.join("some room");
});

```
And then simply use to or in (they are the same) when broadcasting or emitting:
```Java Script
io.to("room1").to("room2").to("room3").emit("some event");
```

###  leave Room

.leave() method to make a socket leave a specific room. This allows you to control which rooms a socket is a part of and restrict the scope of certain events

```Java Script
socket.leave('roomName');
```

----
### Namespace 

A Namespace is a communication channel that allows you to split the logic of your application over a single shared connection (also called "multiplexing").


### Each namespace potentially has its own what?
- Sockets: Sockets represent individual connections between the server and clients in Socket.IO.

- Rooms: Rooms allow you to group sockets together and send targeted messages to specific subsets of connected clients.

- Events: Events are the mechanism for communication between the server and clients, allowing the exchange of data and triggering actions within the application.



### possible use case for separate namespaces

In a multi-tenant application, separate namespaces in Socket.IO can be used to provide isolated real-time communication channels for different groups or organizations. 




