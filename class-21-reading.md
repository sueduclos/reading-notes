[Home Page](https://sueduclos.github.io/reading-notes/)

## Class 21: Component Based UI

### Links

- [React Hello World](https://facebook.github.io/react/docs/hello-world.html)         
- [Introducing JSX](https://facebook.github.io/react/docs/introducing-jsx.html)       
- [Rendering Elements](https://facebook.github.io/react/docs/rendering-elements.html) 
- [SASS](https://sass-lang.com/)                                                      
- [SASSmeister](http://www.sassmeister.com)                                           
- [SASS Cheatsheet](https://devhints.io/sass)                                         
- [React Cheatsheet](https://devhints.io/react)                                       
- [Another React Cheatsheet](https://reactcheatsheet.com/)  
                                              


### Discussion Questions:

#### 1. What is the benefit of breaking up HTML webpage content into components?
Because the components are modular, they can then be imported, duplicated and shared around multiple files, and thus your application composition can be neatly defined.

#### 2. What is JSX? Why is it useful?
`JSX` stands for “JavaScript XML”, and refers to React JavaScript files which allow for JavaScript and HTML to be seamlessly mixed together.

#### 3. What can cause a render (or re-render) of a component?
The `state` of a component refers to a collection of variables which trigger a structural change or re-render of the component.

#### 4. When a render happens, how is the DOM affected?
Render means to build and display the HTML element(s) on your webpage. When a component is rendered, it appears on the page and within the DOM. By changing a component’s state variables, you can trigger a re-render of the component, which means that React will “rebuild” that HTML block within the DOM.

#### 5. What is one thing a framework does that a library doesn't do? 
A framework, on the other hand, sets up rigid places for you to add your code, and the framework is what controls when certain pieces of code are called.
