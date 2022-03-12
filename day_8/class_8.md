[Live_URL](https://mujahedyousef.github.io/advanced-js-reading-notes.-/day_7/class_8.html)

# Read: Class 09

## Review, Research, and Discussion

> Q1 : What header(s) are used in authentication and authorization ?

* **HTTP authentication**
 a general framework for access control and authentication. This page is an introduction to the HTTP framework for authentication, and shows how to restrict access to your server using the HTTP "Basic" schema.

* **HTTP Authorization** request header contains the credentials to authenticate a user agent with a server.
APIs use authorization to ensure that client requests access data securely.

* >List of Authorization Request Headers
There are many types of Authorization Request Headers. Some of them are mentioned below.

* Basic Auth
* Bearer Token
* API Key
* Digest Auth
* OAuth 2.0
* Hawk Authentication
* AWS Signature

> Q2 : What is safe to put into a JWT?

* We use JSON Web Tokens (JWTs) quite a lot in the OAuth and OpenID Connect world.  that they're good for being used as ID Tokens or Access Tokens and that they're secure - as the tokens are usually signed or even encrypted. You have to remember though, that JWT is not a protocol but merely a message format. The RFC just shows you how you can structure a given message and how you can add layers of security, which will protect the integrity and, optionally, the content of the message. But JWTs are not secure just because they are JWTs, it's the way we use them that determines whether they are secure or not.

> Q3: How are JWTs validated?

* When an authorization server issues a token, it signs it using a key. When the client receives the ID token, the client validates the signature using a key as well.

----

## Document the following Vocabulary Terms

Term

|  Term  |   Mean |
|--- |--- |
|   RBAC | Role-based access control (RBAC) is a policy-neutral access-control mechanism defined around roles and privileges.  |
|  User Roles  | permission sets that control access to areas and features within the Professional Archive Platform |
|  JWT Token  | is an open standard that defines a compact and self-contained way for securely transmitting information between parties as a JSON object  |
