### *Class 07 Express*

#### What code does the server actually run?
Server-side code is run on a web server and that its main role is to control what information is sent to the user (while client-side code mainly handles the structure and presentation of that data to the user)
Code runs on a server is meant to be run indefinitely; to always be accessible by clients requesting data.

#### What Express/HTTP operations map to CRUD operations?
GET, POST, PUT and DELETE

#### What does res.send() do?
It sends data back to the client in the properly formatted way

#### What is the order of operations for the three categories of middleware (handler, application, route)?
Application, Route, Handler.

#### What is the parameter next used for?
It calls the next middleware in the chain
