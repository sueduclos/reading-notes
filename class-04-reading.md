[Home Page](https://sueduclos.github.io/reading-notes/)

## Class 04 Reading - Advanced Mongo/Mongoose

### Discussion Questions:

#### 1. What makes an interface useful?
**Interfaces** can be very helpful in standardizing how certain operations are called, and allowing for operations to be largely changed without the code having to be changed too much.

#### 2. Why is middleware called middleware?
**Middleware** typically means “software between two other softwares” - you can think of it as a middleman between two operations that helps the process go more smoothly.

#### 3. Fundamentally, what does it mean to have a mock of something? Why is this useful?
A **mock** of something is that is essentially made for practice. It's useful in testing and allows us to run tests without actually changing the actual data in the real database.  
 
#### 4. What does it mean to have a mock database?
Testing can be a challenge with databases, since we don’t ever want to modify our actual database when we run our tests. A **mock database** only exists during the lifetime of the test: it is created and initialized when we start our tests and deleted when tests are complete.
