[Home Page](https://sueduclos.github.io/reading-notes/)

## Class 10 Authentication

### Links
- [Securing Passwords](http://cs.wellesley.edu/~cs304/lectures/bcrypt/dustwell.html) 
- [Basic Auth](https://en.wikipedia.org/wiki/Basic_access_authentication)             
- [OWASP Auth Cheatsheet](https://www.owasp.org/index.php/Authentication_Cheat_Sheet) 
- [Bcrypt Documentation](https://www.npmjs.com/package/bcrypt)                        
- [Introduction to JWT](https://jwt.io/introduction/)  

### Vocabulary
- authentication 
- authorization
- encyption
- hashing 
- session    
- cookie     
- token
- Basic Auth
- encoding
- secret
- cryptography

### Discussion Questions:

#### 1. Why is authentication important?
Authentication is important because it enables organizations to keep their networks secure by permitting only authenticated users to access its protected resources, which may include computer systems, networks, databases, websites and other network-based applications or services.

#### 2. Why should we be careful about storing a user’s password?
It prevents anyone (including developers with database permissions) from ever getting access to the user’s password.

Sensitive user data should never be sent to clients. When a client asks to log in, they provide a password, and the server validates it. But a password (or any other sensitive information) is not sent from the server back to the client.

#### 3. What is the difference between hashing and encryption?
Hashing is a method of one-way encryption. 
Encryption is a method of two-way encryption.
 
#### 4. What is the difference between encryption and encoding?
Encryption isfor maintaining data confidentiality and requires the use of a key (kept secret) in order to return to plaintext.
Encoding is a simple language translation- data is not actually protected. Anyone who knows the "language" can reverse the translation.

#### 5. What is a token used for?
It's a validation response. It is something the server gives the client to pass along in any future requests
