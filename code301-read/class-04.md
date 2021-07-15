# React Forms and Ternary Operators

## Key Terms and Concepts

Term | Definition
----- | -----

### Forms have a controlled internal state.

- What is a ‘Controlled Component’?

***A component whose state is not controlled by setState() but rather by React***

- Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why?

***The value will update on every keystroke and you can pass the value to other elements.***

- How do we target what the user is entering if we have an event handler on an input field?

***this.setState by pulling the value and updating the state on every keystroke.***

## Ternary Operators

```
condition ? value if true : value if false
```

- Why would we use a ternary operator?

***The code is readable and succint.***

- Rewrite the following statement using a ternary statement:

```
  if(x===y){
 console.log(true);
  } else {
 console.log(false);
  }
```
- ANSWER

```
x===y ? console.log(true) : console.log(false)
```


### FURTHER LEARNING

- What is the .bind method?


*Resources:*

https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff

https://reactjs.org/docs/forms.html*