# Authentication
-------------------------------------------

### Singleton

**It is a software design pattern that restricts the instantiation of a class to one "single" instance. This is useful when exactly one object is needed to coordinate actions across the system. The term comes from the mathematical concept of a singleton.**

**The singleton design pattern is one of the twenty-three well-known "Gang of Four" design patterns that describe how to solve recurring design problems to design flexible and reusable object-oriented software, that is, objects that are easier to implement, change, test, and reuse.**
-----------------------------------------------------

### Singleton with ES6 classes:

**The classes should be private constructor , getInstance() methods that returns instance of the class .We have to export the class name.**
--------------------------------------------------------------------
## If you were tasked with building a middleware system like Express uses, what approach might I take to construct/operate it?
--------------------------------------------------------------------------
* I'll create a function with (req,res, next)
* I'll then export it , and require it in the file which contains the express, and use it in the app by using line of code: app.use(middleWare)

## Term Vocabulary
* *Router-level middleware works in the same way as application-level middleware, except it is bound to an instance of express.Router().*
* *Dynamic Module Loading:the import(module) expression loads the module and returns a promise that resolves into a module object that contains all its exports. It can be called from any place in the code.*

* *Singleton pattern : is a software design pattern that restricts the instantiation of a class to one “single” instance. This is useful when exactly one object is needed to coordinate actions across the system. The term comes from the mathematical concept of a singleton.*

* *CRUD -> REST Method Matches:Create, Read, Update, and Delete.*
------------------------------------------------------

## Preview:

## Securing Passwords with Bcrypt Hashing Function:

**Passwords are the first line of defense against cyber criminals. It is the most vital secret of every activity we do over the internet and also a final check to get into any of your user account, whether it is your bank account, email account, shopping cart account or any other account you have.**

**Cryptographic hash algorithms MD5, SHA1, SHA256, SHA512, SHA-3 are general purpose hash functions, designed to calculate a digest of huge amounts of data in as short a time as possible. Hashing is the greatest way for protecting passwords and considered to be pretty safe for ensuring the integrity of data or password.**
------------------------------------------------------------
*Hash Collision attack:*

**Hash functions have infinite input length and a predefined output length, so there is inevitably going to be the possibility of two different inputs that produce the same output hash. MD5, SHA1, SHA2 are vulnerable to Hash Collision Attack i.e. two input strings of a hash function that produce the same hash result.**
------------------------------------------

### Bcrypt:

**is an adaptive hash function based on the Blowfish symmetric block cipher cryptographic algorithm and introduces a work factor (also known as security factor), which allows you to determine how expensive the hash function will be.**
-------------------------------------------------

### Basic access authentication:

*Authentication* is the process of verifying that an individual, entity or website is whom it claims to be. Authentication in the context of web applications is commonly performed by submitting a username or ID and one or more items of private information that only a given user should know.

basic access authentication is a method for an HTTP user agent (e.g. a web browser) to provide a user name and password when making a request. In basic HTTP authentication, a request contains a header field in the form of Authorization: Basic , where credentials is the Base64 encoding of ID and password joined by a single colon :

HTTP does not provide a method for a web server to instruct the client to "log out" the user. However, there are a number of methods to clear cached credentials in certain web browsers. One of them is redirecting the user to a URL on the same domain, using credentials that are intentionally incorrect. However, this behavior is inconsistent between various browsers and browser versions.



*OpenId* **is an HTTP-based protocol that uses identity providers to validate that a user is whom he says he is. It is a very simple protocol which allows a service provider initiated way for single sign-on (SSO). This allows the user to re-use a single identity given to a trusted OpenId identity provider and be the same user in multiple websites, without the need to provide any website with the password, except for the OpenId identity provider.**

*Security Assertion Markup Language (SAML)* **is often considered to compete with OpenId. The most recommended version is 2.0 since it is very features complete and provides strong security. Like OpenId, SAML uses identity providers, but unlike OpenId, it is XML-based and provides more flexibility. SAML is based on browser redirects which send XML data. Furthermore, SAML isn't only initiated by a service provider; it can also be initiated from the identity provider. This allows the user to navigate through different portals while still being authenticated without having to do anything, making the process transparent.**

*The Fast Identity Online (FIDO)* **Alliance has created two protocols to facilitate online authentication: the Universal Authentication Framework (UAF) protocol and the Universal Second Factor (U2F) protocol. While UAF focuses on passwordless authentication, U2F allows the addition of a second factor to existing password-based authentication. Both protocols are based on a public key cryptography challenge-response model.**


## node.bcrypt.js
------------------------------------------------------------------------


It is a library to help you hash passwords.

Per bcrypt implementation, only the first 72 bytes of a string are used. Any extra bytes are ignored when matching passwords. Note that this is not the first 72 characters. It is possible for a string to contain less than 72 characters, while taking up more than 72 bytes (e.g. a UTF-8 encoded string containing emojis).

This library supports $2a$ and $2b$ prefix bcrypt hashes. $2x$ and $2y$ hashes are specific to bcrypt implementation developed for John the Ripper. In theory, they should be compatible with $2b$ prefix.