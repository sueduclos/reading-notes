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

#### 2. Why are functional components preferred over class components? 

#### 3. What is wrong with the following code? 

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
