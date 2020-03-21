[Home Page](https://sueduclos.github.io/reading-notes/)

## Class 03 Reading

### Discussion Questions:

#### 1. Why would a developer choose to make data models?
It is a more planned and structured approach to handling data. Plus it allows by having checks built in to enforce that structure holding the data. 

#### 2. What purpose do CRUD operations serve?
To watch and regulate every action that may create or change data. To be able to create, read, update, and delete data in a structured and error-safe way.
* Create - add a new data entry
* Read - recieve the contents of an existing data entry
* Update - change an existing data entry
* Delete - remove an existing data entry

#### 3. What kind of database is Postgres? What kind of database is MongoDB?
**PostgreSQL** is a relational database management system. A SQL database can be thought of as more ridgid. Everything belongs in defined tables, and you use SQL to filter through those tables.

**MongoDB** is an open source, non- relational database management system. A NoSQL database does not impose a structure; instead it uses a system of ids to find the data you’re looking for. NoSQL databases are handy because they are much more flexible than SQL databases. NoSQL databases can support changing needs and can scale up easily.

 
#### 4. What is Mongoose and why do we need it? 
**Mongoose** is a package that acts as our middleman between our application and our database. Think of Mongoose as a JavaScript translator; our application speaks to Mongoose in JavaScript, and Mongoose translates that into the terms MongoDB understands. Mongoose also adds a lightweight structure and validity checking to our MongoDB, so that we get some of the benefits of an SQL database while actually using a NoSQL database


#### 5. Define three related pieces of data in a possible application. An example for a store application might be Product, Category and Department. Describe the contraints and rules on each piece of data and how you would relate these pieces to each other. For example, each Product has a Category and belongs in a Department.
Products, Vendors, Customers. Customers reach out to vendors to obtain products. 

