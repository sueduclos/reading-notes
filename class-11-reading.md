[Home Page](https://sueduclos.github.io/reading-notes/)

## Class 11 DSA: Stacks and Queues

### Links                                                       

[Data Structures: Stacks and Queues](https://www.youtube.com/watch?v=wjI1WNcIntg) 

[Stacks and Queues](https://everythingcomputerscience.com/discrete_mathematics/Stacks_and_Queues.html)

### Vocabulary
Common terminology for a stack is

* `push` - a `Node` is put onto the top of the stack
* `pop` - a `Node` is removed from the top of the stack
* `top` - the last-added or topmost `Node` in the data structure 
* `peek` - an action where you look at the value of the top `Node` without removing that `Node` from the data structure 

Common terminology for a queue is: 

* `enqueue` - Add a `Node` to the end of the queue
* `dequeue` - Remove a `Node` from the beginning of the queue
* `front` - The first `Node` of the queue
* `rear` - The last `Node` of the queue
* `peek` - an action where you look at the value of the front `Node` without removing that `Node` from the data structure

### Discussion Questions:

#### 1. Come up with an application scenario where you would want to use a stack.
To reverse a word. You push a given word to stack - letter by letter - and then pop letters from the stack.

#### 2. Come up with an application scenario where you would want to use a queue. 
Call Center phone systems uses Queues to hold people calling them in an order, until a service representative is free.

#### 3. Why are `pop`, `push`, `enqueue` and `dequeue` always `O(1)`?
This is done with an O(1) operation in time because it does not matter how many other items in the queue or stack; it always takes the same amount of time to perform the operation.
 
#### 4. Why do stacks and queues not have traversal or searching operations? 
Because they are mostly meant for temporary storage instead of long-term storage or traversal.
