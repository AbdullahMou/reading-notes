# JSON Web Token
* JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.

  * Authorization: This is the most common scenario for using JWT.

  * Information Exchange: JSON Web Tokens are a good way of securely transmitting information between parties.

## Payload
* Payload The second part of the token is the payload, which contains the claims.
* Claims are statements about an entity (typically, the user) and additional data.
* There are three types of claims: registered, public, and private claims.

  * **Registered claims**: These are a set of predefined claims which are not mandatory but recommended, to provide a set of useful, interoperable claims. Some of them are: iss (issuer), exp (expiration time), sub (subject), aud (audience), and others.

  * **public claims**: These can be defined at will by those using JWTs. But to avoid collisions they should be defined in the IANA JSON Web Token Registry or be defined as a URI that contains a collision resistant namespace.

  * **Private claims**: These are the custom claims created to share information between parties that agree on using them and are neither registered or public claims.

## How do JSON Web Tokens work?

* **In authentication**
  * when the user successfully logs in using their credentials, a JSON Web Token will be returned. Since tokens are credentials, great care must be taken to prevent security issues. In general, you should not keep tokens longer than required.

