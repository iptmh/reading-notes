### *OAuth*

#### What's a benefit of using OAuth instead of your own basic authentication?
OAuth is more secure and efficient than basic authentication.

#### Write the following steps in the correct order:
- Ask the client if they want to sign in via a third party
- Redirect to a third party authentication endpoint
-Receive authroization code
-Make a request to a third-party API endpoint
-Make a request to the access token endpoint
-Receive access token
-Register your application to get a client_id and client_secret

#### What can you do with an authorization code?
The authorization code tells us that the client/user has allowed the server to read data from the user's Google account. In order to get this authorization code, the server needs to actually fully redirect the client to a Google endpoint. When redirecting, the server sends the following information in query parameters, so that the Google endpoint knows how to get back to the server.

#### What can you do with an access token?
An access token is basically a "signed in user", which can be used in any future request to get user data. Anyone who has an access token can act as an authenticated user, doing any of the actions specified in the scope originally provided. 
