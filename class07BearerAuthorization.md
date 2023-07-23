## intro to Jwat 

#### What is a JSON Web Token (JWT)?

JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.


#### When should we use JSON Web Tokens?

**Authorization:** Once the user is logged in, each subsequent request will include the JWT, allowing the user to access routes, services, and resources that are permitted with that token.

**Information Exchange:** Because JWTs can be signed—for example, using public/private key pairs—you can be sure the senders are who they say they are. 


#### Claims are expected in which structural component of a JWT?

JWTs contain claims in the **payload component.** Claims can be registered (predefined), public (standardized custom), or private (custom for specific parties). They provide information about an entity and additional data.


--- 
## Are JWTs Secure?

#### If I get a JWT and I can decode the payload, how can we call that secure?
If dealing with a client like the web browser for example, you can store the JWT tokens in a cookie that is secure (is not transmitted via HTTP, only via HTTPS) and httpOnly (can't be read by Javascript) and talks to the server over an encrypted channel (HTTPS). Once you know you have a secure channel between the server and client you can securely exchange JWT or whatever else you want.


#### If sending a JWT, what must sender and receiver both know?
![Alice and Bob exmple ](https://www.open.edu/openlearn/pluginfile.php/697247/mod_oucontent/oucontent/34284/e1d42cc2/f558174e/ou_futurelearn_cyber_security_fig_1177.tif.jpg)

Let's assume Alice wants to send a JWT to Bob. They both know some shared secret. Mallory doesn't know that secret, but wants to interfere and change the JWT. To prevent that, Alice calculates `Hash(payload + secret)` and appends this as signature.

When receiving the message, Bob can also calculate Hash(payload + secret) to check whether the signature matches. If however, Mallory changes something in the content, she isn't able to calculate the matching signature (which would be Hash(`newContent + secret`)). She doesn't know the secret and has no way of finding it out. This means if she changes something, the signature won't match anymore, and Bob will simply not accept the JWT anymore.

#### Explain how concatenated content and secret can be sent and received securely to a non-technical recruiter.
- Encrypt the concatenated content using a strong encryption algorithm.

- Share the encrypted content with the recruiter via a secure file transfer method.

- Provide the recruiter with the secret separately, such as through a secure messaging platform or in person.

- Instruct the recruiter to decrypt the content using the secret to access the original information.

--- 
## JWTs Explained

#### Why use JWT?

JWTs are favored for authentication and authorization purposes because they eliminate the need for server-side storage, allowing for a scalable and efficient system.

 Their compact format enables easy transmission over networks with limited bandwidth. 
 
 Being self-contained, JWTs contain all necessary information, reducing database lookups. 
 
 Additionally, they offer cross-domain capabilities, enabling seamless authentication and authorization across different systems.

#### JWT is Compact and self-contained. Describe how this is useful to a non-technical friend.

Imagine having a USB drive that contains all your project files, allowing you to access them on any computer without relying on servers or the internet. Similarly, JWTs are compact, containing all necessary information in a single token. They are self-contained, like a mini-computer, carrying their own data and reducing dependence on external systems. This independence and efficiency make JWTs a reliable and convenient choice for authentication and authorization.


#### What are the three components (the structure) of a JWT signature?

The three components of a JWT signature are:

Header: Contains metadata about the type of token and the algorithm used for the signature.

Payload: Also known as claims, it contains the actual data and additional information about the entity or user.

Signature: Created by combining the encoded header, encoded payload, and a secret key. It ensures the integrity and authenticity of the token.




--- 
## Reflection

#### What are your learning goals after reading ?





implementation JWT by express js