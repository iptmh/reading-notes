### *Socket.io*

#### What does it mean that web sockets are bidirectional? Why is this useful?
Web sockets follow a communication ruleset (or protocol) also called WebSocket, where the communication between the connection and socket server is bidirectional, or two-way. Web sockets remain connected during their lifetime, and they are really well suited for real-time data transfer over the web. 

#### Does socket.io use HTTP? Why?
Yes, socket.io does connect the client and server via HTTP and TCP. The TCP layer is for data transfer, and the HTTP layer is to ensure that the connection between the client and server is kept active and authenticated.

#### What happens when a client emits an event? What happens when a server emits an event?
They communicate to each other. 

#### Benefits of socket.io:
+ The http layer ensures that the connection is continuous, so even when the server restarts, the clients are not killed, and they're just on hold until the server restarts again. So that way your applications won't just crash. 
+ It allows us to emit specifc events whereas the net package only allows us to admit the data event. We can subscribe or listen to other built-in events like connection, things like that, but we can only emit the data event which is very limiting. Socket io allows us to emit any event similar to our event driven package. 
+ Server can emit or broadcast things to all of its clients

#### From class demo:
Server can make:
1. Shouter can hear shouter and whisper. Whisper can hear shouter message.
2. Make Shouter in a specific building called message (localhost:3000/message), a specific url path

Make a sub server:
const messageServer = server.of ('message')
+ whatever happens in the building, stays in this building
+ kind of like a mini server within a server
+ can only hear things in the building (sub server)
    + on scout.js, need to make sure 
    1. messageServer.emit ('shout heard', payload)
    2. not just server, then can broadcast to the field too
    3. create room: can hear things in the room and also thing in the field
