## React and Forms

1. What is a ‘Controlled Component’?

>  An input form element whose value is controlled by React.

2. Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why?
> We Should update the user responsees as soon as they enter them, to apply making the React state the source of truth.

3. How do we target what the user is entering if we have an event handler on an input field?
> By using onChange, and add a name attribute to each element and let the handler function choose what to do based on the value of event.target.name.
***
***
## The Conditional (Ternary) Operator


Why would we use a ternary operator?
> Becuase it's esaier than if-statment and need less lines of code to write it. 

Rewrite the following statement using a ternary statement:
```javascript 
if(x===y){
  console.log(true);
} else {
  console.log(false);
}
```
```javascript 
(x===y)?console.log(true):console.log(false);

```

>>> ***Bookmark and Review***

- [Forms](https://reactjs.org/docs/forms.html)
- [The Conditional (Ternary) Operator](https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff)
- [React Bootstrap - Forms](https://react-bootstrap.github.io/forms/overview/)
- [React Docs - conditional rendering](https://reactjs.org/docs/conditional-rendering.html)
***
## Things I want to know more about
- onChange handler.
- Controlled Component.
