[Home Page](https://sueduclos.github.io/reading-notes/)

## Class 23: Props and State

### Links

- [SetState Explained](https://css-tricks.com/understanding-react-setstate/) 
- [Handling Events](https://facebook.github.io/react/docs/handling-events.html) 
- [Forms](https://facebook.github.io/react/docs/forms.html)    
- [State and Lifecycle](https://facebook.github.io/react/docs/state-and-lifecycle.html) 
- [Components and Props](https://facebook.github.io/react/docs/components-and-props.html) 
                                              


### Discussion Questions:

#### 1. Why might you want to create a `FormInput` component?
It allows the input element to be reusable in other places. If we want to make any changes to how the input functions, we can make those changes inside the FormInput component file we created and they will be applied to every instance where the input component is used. 

#### 2. Can a parent component access the state of a child component? 
Yes, the parent component can access the state of the child component through props.

#### 3. What can be passed along in a prop variable?
`props` are akin to parameters being passed from a parent component to a child component. These parameters can be static variable data or entire functions.



