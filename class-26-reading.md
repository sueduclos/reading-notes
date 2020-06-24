[Home Page](https://sueduclos.github.io/reading-notes/)

## Class 26: Hooks API

### Links

- [Making Sense of Hooks](https://medium.com/@dan_abramov/making-sense-of-react-hooks-fdbde8803889) 
- [The State Hook](https://reactjs.org/docs/hooks-state.html)  
- [Hooks API](https://reactjs.org/docs/hooks-overview.html)    
- [Hooks API Reference](https://reactjs.org/docs/hooks-reference.html) 
- [Effects Hook](https://reactjs.org/docs/hooks-effect.html)   
                                              

### Discussion Questions:

#### 1. What does a component's lifecycle refer to?
Another feature that class components have is the ability to plug into lifecycle methods. These are functions such as componentDidMount, componentDidUpdate, etc. These are functions that are automatically called by React when a class component renders, mounts, changes, unmounts, etc. When we write our own class components, we can overwrite these function definitions to run our own code.

#### 2. Why are functional components preferred over class components? 
Developers tended to favor functional components for their ease of implementation, and so Hooks were added as a way to enable that further.

#### 3. What is wrong with the following code? 
Hooks should only be defined/called at the top level, and never inside loops, conditions or nested functions. It is nested in a for loop. 

   ```jsx
   import React, {useState, useEffect} from 'react'; 
   
   function MyComponent(props) {
     const [count, setCount] = useState(0); 
     
     function changeCount(e) {
       setCount(e.target.value); 
     }
     
     let renderedItems = []
     
     for (let i = 0; i < count; i++) {
       useEffect( () => {
         console.log('component mount/update'); 
       }, [count]); 
       
       renderedItems.push(<div key={i}>Item</div>); 
     }
     
     return (<div>
       	<input type='number' value={count} onChange={changeCount}/>
         {renderedItems}
       </div>);
   }
   ```
