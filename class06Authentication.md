##  Hash and store a password.


> When you create a password, it needs to be stored in a safe way so that nobody can easily steal it. One way to do this is by using something called a hash.

> Think of a hash like a secret code for your password. It takes your password and turns it into a jumbled-up string of characters that is unique to your password. This jumbled-up string is the hash.


## Bcrypt

Bcrypt is an adaptive hash function based on the **Blowfish symmetric block cipher cryptographic algorithm** and introduces a work factor (also known as security factor), which allows you to determine how expensive the hash function will be.


## Why might you use something like Bcrypt?
Bcrypt is used to make password storage more secure. It slows down attackers by making the hashing process slow and computationally expensive. It also adds uniqueness to each password with automatically generated salts. Bcrypt is widely trusted and adopted in the most of web Application.

**Resourse:**
[Securing Passwords with Bcrypt Hashing Function](https://thehackernews.com/2014/04/securing-passwords-with-bcrypt-hashing.html)

---

## What is Basic Authentication?

Authentication is the process of verifying that an individual, entity or website is whom it claims to be. Authentication in the context of web applications is commonly performed by submitting a username or ID and one or more items of private information that only a given user should know.

## What properties are necessary in the header of a Basic Auth request?

> Authorization: This property indicates that the request is using Basic Auth.

- Base64-encoded credentials: The username and password are combined and encoded in Base64 format. 

- The encoded credentials are included in the header.

- the header of a Basic Auth request should include the "Authorization" property with the Base64-encoded username and password.

## How are username:password in Basic Auth encoded?

In Basic Auth, the username and password are combined with a colon `: ` separator, and the resulting string is encoded using Base64 encoding.

```JSON
username:password
```

--- 

## Define the authentication process to a non-technical recruiter.
 >authentication is the process of confirming a user's identity by verifying their unique identifier (username/email) and matching it with the associated password.


 ## Authentication and Error Messages

Incorrectly implemented error messages in the case of authentication functionality can be used for the purposes of user ID and password enumeration. An application should respond (both HTTP and HTML) in a generic manner.

[OWASP Cheat Sheet Series
](https://cheatsheetseries.owasp.org/cheatsheets/Authentication_Cheat_Sheet.html)



