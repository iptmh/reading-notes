### *Class 06 HTTP and RESTs*

#### What does protocol mean?
A protocol is a set of rules that must be followed. HTTP was developed as a way for clients and servers to interact over the web in a consistent way. A client is anyone asking for/requesting data for an end user. A server is anyone sending/responding with data over the web to a client. This pattern of requests and responses is commonly referred to as the Web Request Response Cycle (WRRC).

#### How does any web browser understand how to open any webpage?
The REST guidelines dictate how to format a server’s APIs so that a client can access all the methods / functionality they need.

#### Name one thing a request object must have, and one thing a response object must have
Request object must have a method, and response object must return a body message.

#### What is the difference between HTTP and REST?
HTTP is a communications protocol that transports messages over a network. Rest is a protocol to exchange any(XML or JSON) messages that can use HTTP to transport those messages.

#### Why is REST important?
When designing a web API, we must follow the rules of HTTP. We also should follow the guidelines of Representational State Transfer (REST). The REST guidelines dictate how to format a server’s APIs so that a client can access all the methods / functionality they need. It is encouraged to use REST guidelines when building APIs, so that various servers can have some sense of consistency. If every API adopts the same standards, it makes it easier for clients to understand how to use your API!
