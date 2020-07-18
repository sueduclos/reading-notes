[Home Page](https://sueduclos.github.io/reading-notes/)

## Class 32: Redux - Asynchronous Actions

How do we use the synchronous action creators? The standard way to do it with Redux is to use the Redux Thunk middleware.

- It is a middleware that looks at every action that passes through the system, and if it’s a function, it calls that function. That’s all it does.
                                              

### What is a Thunk? What are they the best for?

[Resource](https://daveceddia.com/what-is-a-thunk/)

- A thunk is another word for a function. But it’s not just any old function. It’s a special (and uncommon) name for a function that’s returned by another. Like this:

```
function wrapper_function() {
  // this one is a "thunk" because it defers work for later:
  return function thunk() {   // it can be named, or anonymous
    console.log('do stuff now');
  };
}
```

- Thunks are best for complex synchronous logic (especially code that needs access to the entire Redux store state), and simple async logic (like basic AJAX calls). With the use of async/await, it can be reasonable to use thunks for some more complex promise-based logic as well.

Redux has a few main concepts: there are “actions”, “action creators”, “reducers”, and “middleware.”

Actions are just objects. As far as Redux is concerned, out of the box actions must be plain objects, and they must have a type property. Aside from that, they can contain whatever you want – anything you need to describe the action you want to perform.

Actions look like this:

```
// 1. plain object
// 2. has a type
// 3. whatever else you want
{
  type: "USER_LOGGED_IN",
  username: "dave"
}
```

And, since it’s kind of annoying to write those objects by hand all the time (not to mention error-prone), Redux has the concept of “action creators” to stamp these things out:

```
function userLoggedIn() {
  return {
    type: 'USER_LOGGED_IN',
    username: 'dave'
  };
}
```

