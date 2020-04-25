[Home Page](https://sueduclos.github.io/reading-notes/)

## Class 13: Bearer Authorization

### Links                                                       

- [JWTs Explained](https://www.youtube.com/watch?v=926mknSW9Lo)
- [Intro to JWT](https://jwt.io/introduction/)                
- [Are JWTs Secure?](https://stackoverflow.com/questions/27301557/if-you-can-decode-jwt-how-are-they-secure) 
- [NPM JSON Web Token Documentation](https://www.npmjs.com/package/jsonwebtoken) 

### Vocabulary
- encryption: Encryption is the method by which information is converted into a secret code that hides the information's true meaning. During encryption, a secret key is used to make sure that only those parties with the secret key can later decrypt the code. Encryption is commonly used to protect data in transit. 
- token: In general, a token is an object that represents something else, such as another object. In the world of authentication, a token typically is an encrypted string that represents a signed in user.
- bearer: This refers to a client bringing a token to a server.  
- secret: A unique string that only a few parties know (in our case, just the server knows). Because it can be used to decrypt sensitive information, the secret should be kept protected or well hidden. 
- JSON Web Token: A package that lets us lightly encrypt data as a JSON object. 
- key: A value that lets us decrypt an encrypted string. Typically this is kept secret.

### Discussion Questions:

#### 1. When is Basic Authorization used vs. Bearer Authorization? 

#### 2. What does the JSON Web Token package do?

#### 3. What considerations should we make when creating and storing a `SECRET`? 
