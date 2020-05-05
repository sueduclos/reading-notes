[Home Page](https://sueduclos.github.io/reading-notes/)

## Class 15: Event Driven Applications

### Links

- [Event Driven Programming](https://alligator.io/nodejs/event-driven-programming/)
- [Node Documentation: Events](https://nodejs.org/api/events.html)
- [What the Heck is the Event Loop Anyway?](https://www.youtube.com/watch?v=8aGhZQkoFbQ)
- [Events and Event Emitter in Node.js](https://www.youtube.com/watch?v=l20MBBFZAmA)
                                              

### Vocabulary
- Observer Pattern:        :  This is a software design pattern where an object, called the _subject_, has a list of _observers_ that are notified when something about the _subject_ changes. Events follow the Observer Pattern. 
- event                    :  Events are actions within our application ecosystem that are "raised" or "triggered" either manually within a function, by some user input, or by connections to other services. 
- listener                 :  A listener continually waits for a specific event to be raised, and then executes some code (a handler) each time the event is raised.
- event handler            :  An event handler is the code that executes after an event is raised. An event listener will first acknowledge that the event was raised and call an event handler. The content of an event handler can be anything specific to the application and event. 
- event driven programming :  This is an approach to programming where code emits events instead of using callbacks. While event driven applications can use both events and callbacks in conjunction, this style of programming generally places a preference on emitting events. 
- event loop               :  The event loop is a continually running process in every application that checks whether the call stack is empty. When the call stack is empty, the event loop pushes the front of the event queue onto the call stack, and then repeats the process of checking for an empty call stack. Through the event loop, programs can have asynchronous processes and event handling. 
- event queue              :  The event queue exists throughout the lifetime of your application, and it enqueues callback functions and listeners that need to be run in the call stack. The event queue enqueues these callbacks and listeners when an asynchronous operation ends, or when an event is triggered. 
- call stack               :  The call stack is a stack that exists throughout the lifetime of your application. The call stack pushes lines of code that needs to be executed, and pops off lines of code that have completed execution. 
- emit / raise / trigger   :  These terms refer to the process of saying an event has occurred, causing the event listener to tell the program to run one or more event handler functions. 
- thread                   :  A thread is a processor for running some lines of code. All modern computers allow for multi-threading - having multiple processors independently running multiple lines of code. The web also allows for multi-threading, allowing multiple web processors to run code at one time. 


### Discussion Questions:

#### 1. Given the examples of front-end events such as button click, window resize, form submit, etc, what are some examples of back-end events? 
Logging messages, etc.

#### 2. Why are events sometimes better than asynchronous actions with callbacks? 
The benefit of this approach is that now you can have multiple listeners on a single event - having multiple callbacks however is harder to do and can quickly get very confusing.

#### 3. What does an `EventEmitter` instance do? 
It allows us to both raise new events and to listen to events that have been raised. 

#### 4. When is a program's call stack, event queue, and event loop active? 
When you run your application, each line of your code starts by being pushed onto the `call stack`. When this line of code is done executing, it is popped off of the stack. When the asynchronous command is complete, the callback is pushed onto another data structure called the `event queue`. There is a continuous process that runs outside of our application called the `event loop`. The event loop’s sole job is to dequeue things from the event queue, and push them onto the call stack only when the call stack is empty. 

