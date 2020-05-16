### *Message Queues*

#### What is the main benefit of a message queue server?
A message queue server (or simply, queue server) runs independently and is tasked with routing events and messaging between clients. Any connected client can publish a message to the server, or subscribe to certain types of messages. This makes it easier to grow our application, and it means our clients can be even more lightweight.

Moreover, a queue server makes sure that all connected clients are up to date with the data they need. Subscribed clients can now “catch up” and pull down any events (or messages) they may have missed while disconnected.

#### Why might we want to initiate messages from an HTTP request?
To identify the type of request (GET, POST, PUT, DELETE)

#### Is the Message Queue Server a socket.io client, a socket.io server, or an api server?
A socket.io server
