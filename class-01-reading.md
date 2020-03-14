## Class 01 Reading

### Discussion Questions:

#### 1. Why would you want to run JavaScript code outside of a browser?
It lets us do a lot more with JavaScript aside from simple websites. It allows developers to add in a database, an API, events, triggers, a phone app, and much more. To do this we use a new ecosystem, or environment, called **Node.js** to run our JavaScript code.

#### 2. What is the difference between a module and a package?
**Modules** are pieces of JavaScript code that are meant to be called in another file or chunk of code. Think of a function with inputs and outputs; you can define the function, but it’s not run until the function is called later in the code.

**Packages** are an extension of modules, and they are what make the Node.js ecosystem so powerful. Packages allow developers to make complex chunks of code that serve a certain purpose, and then publish and share those packages for other developers to use.

#### 3. What is one benefit of Test Driven Development?
To ensure that code is working correctly. Many developers employ a practice called **test driven development(TDD)**, where they write tests for their code before they write the actual code itself! This means planning out the input format and expected outputs of a module before development, and it can help prevent uncertainty during the development process.

**Benefit:** Because you are writing small tests at a time, it forces your code to be more modular (otherwise they’d be hard to test against). **TDD** helps you learn, understand, and internalise the key principles of good modular design.

#### 4. What is one potential downside of Test Driven Development?
**Potential downside:** Initially, it slows down development; for rapidly iterative startup environments the implementation code may not be ready for some time due to spending time writing tests first. (But in the long run, it actually speeds up development)

#### 5. What does the node package manager do?
To make use of these tools (or packages) in **Node.js**, we need to be able to install and manage them in a useful way. This is where `npm`, the Node package manager, comes in. It installs the packages you want to use and provides a useful interface to work with them.
