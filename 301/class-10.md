# Reading
- ### [Understanding the JavaScript Call Stack](https://medium.freecodecamp.org/understanding-the-javascript-call-stack-861e41ae61d4)
***
1. What is a ‘call’?
> calling a or invoked the function (function invocation).

2. How many ‘calls’ can happen at once?
> once at time

3. What does LIFO mean?
>  Last In, First Out 
4. Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.
> ![](https://cdn-media-1.freecodecamp.org/images/QgR2uIk7tW0YNz0Xm8g0jAPeRFI0e4sCejsv)
5. What causes a Stack Overflow?
> A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error. 
***
***
***
- [JavaScript error messages && debugging](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)

1. What is a ‘reference error’?
>This is as simple as when you try to use a variable that is not yet declared you get this type os errors.
> ```console.log(foo) // Uncaught ReferenceError: foo is not defined```
2. What is a ‘syntax error’?
> this occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.
```JSON.parse( {'foo': 'bar'} ) // Uncaught SyntaxError: Unexpected token o in JSON at position 1```
3. What is a ‘range error’?
>Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up. length of the array also.(negative length).
4. What is a ‘tyep error’?
> Like the name indicates, this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.
5. What is a breakpoint?
> it's a feature in editers, which will make your program stop at that point only if a condition is met,
6. What does the word ‘debugger’ do in your code?
> Let you to debugg your code and trace the errors and bugs