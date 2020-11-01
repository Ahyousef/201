# Read 13

## Review
- Write the following steps in the correct order:

Register your application to get a client_id and client_secret
Ask the client if they want to sign in via a third party
Redirect to a third party authentication endpoint
Make a request to the access token endpoint
Receive access token
Make a request to a third-party API endpoint
Receive authorization code


- What can you do with an authorization code?

Sent to the provider to get certain information like username,name,email

- What can you do with an access token?

Store it in the headers/database to make sessions so the user doesn't have to login for every page, and to authenticate the user.

- What’s a benefit of using OAuth instead of your own basic authentication?

Big companies have high security, not force the user to sign up in the long way.


## Preview

### JWT

What is JSON Web Token?
JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.

Although JWTs can be encrypted to also provide secrecy between parties, we will focus on signed tokens. Signed tokens can verify the integrity of the claims contained within it, while encrypted tokens hide those claims from other parties. When tokens are signed using public/private key pairs, the signature also certifies that only the party holding the private key is the one that signed it.


### JWT security

JWTs can be either signed, encrypted or both. If a token is signed, but not encrypted, everyone can read its contents, but when you don't know the private key, you can't change it. Otherwise, the receiver will notice that the signature won't match anymore.

