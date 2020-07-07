[Home Page](https://sueduclos.github.io/reading-notes/)

## Class 29: Application State with Redux

### Links

- [Dan Abramov Redux Tutorials](https://egghead.io/courses/getting-started-with-redux) 
- [World's Easiest Guide to Redux](https://medium.freecodecamp.org/understanding-redux-the-worlds-easiest-guide-to-beginning-redux-c695f45546f6) 
- [Testing with Redux and Enzyme](https://medium.com/netscape/testing-a-react-redux-app-using-jest-and-enzyme-b349324803a9) 
- [Testing Reducers](https://medium.com/@netxm/testing-redux-reducers-with-jest-6653abbfe3e1) 
- [Redux Docs](https://redux.js.org/)                          
- [enzyme-redux npm module](https://www.npmjs.com/package/enzyme-redux) 
- [Middleware Tests with a Mock Store](https://gist.github.com/johncokos/4902683c8e33ed38fb2ba066b8764831) 
                                              

### Discussion Questions:

#### 1. Why would you wrap your entire application within a context?
Context is primarily used when some data needs to be accessible by many components at different nesting levels. Apply it sparingly because it makes component reuse more difficult.

#### 2. What is the purpose of a reducer?
A reducer's purpose is to take in the current state and an action, and then determine how to modify the state based on the action.

#### 3. What does an `action` contain?
 Actions are a plain JavaScript object that contains information.

#### 4. Why do we need to copy the state in a reducer? 
We don't mutate the state. A reducer's purpose is to take in the current state and an action, and then determine how to modify the state based on the action. This is why it is common to begin each reducer function with copying the current state (you can't mutate / change the state parameter directly) and then running a switch statement based on the type of action. 
