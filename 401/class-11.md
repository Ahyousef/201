# Read 11

## Review

- Explain what a “Singleton” is (in Computer Science terms)
Restricting the instantiation of a class to one "single" instance.

- Explain how the Singleton pattern can be used with Node modules, specifically with classes
If you need only one instance/object of your class, then singleton pattern can be used, otherwise it isn't.

- If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?
All about making it most efficient but working at the same time, so I would make modules.


## Preparation summary

### Securing passwords

We all know storing passwords in clear text in your database is ridiculous. Many desktop applications and almost every web service including, blogs, forums eventually need to store a collection of user data and the passwords, that has to be stored using a hashing algorithm.
Cryptographic hash algorithms MD5, SHA1, SHA256, SHA512, SHA-3 are general purpose hash functions, designed to calculate a digest of huge amounts of data in as short a time as possible. Hashing is the greatest way for protecting passwords and considered to be pretty safe for ensuring the integrity of data or password.
The benefit of hashing is that if someone steals the database with hashed passwords, they only make off with the hashes and not the actual plaintext passwords. But why do we always hear about passwords being cracked? There are some weaknesses in cryptographic hash algorithm that allows an attacker to calculate the original value of a hashed password


### Authentication

Basic access authentication
From Wikipedia, the free encyclopedia
Jump to navigationJump to search
HTTP
PersistenceCompressionHTTPSQUIC
Request methods
OPTIONSGETHEADPOSTPUTDELETETRACECONNECTPATCH
Header fields
CookieETagLocationHTTP refererDNTX-Forwarded-For
Status codes
301 Moved Permanently302 Found303 See Other403 Forbidden404 Not Found451 Unavailable for Legal Reasons
Security access control methods
Basic access authenticationDigest access authentication
Security vulnerabilities
HTTP header injectionHTTP request smugglingHTTP response splittingHTTP parameter pollution
vte
In the context of an HTTP transaction, basic access authentication is a method for an HTTP user agent (e.g. a web browser) to provide a user name and password when making a request. In basic HTTP authentication, a request contains a header field in the form of Authorization: Basic <credentials>, where credentials is the Base64 encoding of ID and password joined by a single colon :.


### JSON Web Tokens

What is JSON Web Token?
JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.
