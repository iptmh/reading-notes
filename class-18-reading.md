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
