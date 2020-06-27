[Home Page](https://sueduclos.github.io/reading-notes/)

## Class 27: Hooks API

### Links

- [Custom Hooks - All You Need to Know](https://www.telerik.com/blogs/everything-you-need-to-create-a-custom-react-hook) 
- [Async Hooks](https://dev.to/vinodchauhan7/react-hooks-with-async-await-1n9g) 
- [useReducer Hook](https://reactjs.org/docs/hooks-reference.html#usereducer) 
- [React Custom Hooks](https://reactjs.org/docs/hooks-custom.html) 
- [Use Hooks](https://usehooks.com/)                           
- [Hooks List](https://github.com/rehooks/awesome-react-hooks) 
- [10 Essential React Hooks](https://blog.bitsrc.io/10-react-custom-hooks-you-should-have-in-your-toolbox-aa27d3f5564d) 
                                              

### Discussion Questions:

#### 1. Why do custom hooks need the `use` prefix?
This tells the React linter that it is acceptable for that function to utilize other hook functions inside of it. Without it, we wouldn’t be able to automatically check for violations of rules of Hooks because we couldn’t tell if a certain function contains calls to Hooks inside of it.

#### 2. What do custom hooks usually do? 
Modularization. A custom hook is just a function that uses one or more of any other established hook functions.

#### 3. Using the links above, list one custom hook that you would be interested in trying/using. 
I would be interested in using the useForm custom hook.
     
