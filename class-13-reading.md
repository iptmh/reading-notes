### *Bearer Authorization*

#### When is Basic Authorization used vs. Bearer Authorization?
Instead of having the user continually send their username and password over the internet, or undergo the long OAuth process, the server creates an encrypted token (bearer token) for the user to send instead.

#### What does the JSON Web Token package do?
It securely transmits information between two systems (servers, clients, etc.) as a JSON object. 

#### What considerations should we make when creating and storing a SECRET?
There is still a slight risk that the content encrypted could be hacked into. Because of this, we try not to put any sensitive user data (such as a password) into the JWT. Typically, the server only stores either the user’s unique username, or the id of the user record within the server’s database.
