### *Authentication*

#### Why is authentication important?
For security reasons and storing sensitive information. 

#### Why should we be careful about storing a user’s password?
To avoid leaking the user's information.

#### What is the difference between hashing and encryption?
Encryption is a two-way function; what is encrypted can be decrypted with the proper key. Hashing, however, is a one-way function that scrambles plain text to produce a unique message digest. With a properly designed algorithm, there is no way to reverse the hashing process to reveal the original password.

#### What is the difference between encryption and encoding?
Encoding is for maintaining data usability and can be reversed by employing the same algorithm that encoded the content, i.e. no key is used. Encryption is for maintaining data confidentiality and requires the use of a key (kept secret) in order to return to plaintext.

#### What is a token used for?
A Server can decode the Basic Authorization header to retrieve the username and password. If the combination is validated, the server generally responds back to the client with some sort of validation response (token) so that the client can re-authenticate without having to continually send the username:password combination in plain text over the internet.
