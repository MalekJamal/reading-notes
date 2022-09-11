# Readings: Putting it all together
- ### [Thinking in React](https://reactjs.org/docs/thinking-in-react.html)

1. What is the single responsibility principle and how does it apply to components?
>

2. What does it mean to build a ‘static’ version of your application?
> static version requires a lot of typing and no thinking

3. Once you have a static application, what do you need to add?
>adding interactivity, you’ll want to build components that reuse other components and pass data using props.

4. What are the three questions you can ask to determine if something is state?

>1. Is it passed in from a parent via 
props? **If so, it probably isn’t state.**
> 2. Does it remain unchanged over time? **If so, it probably isn’t state.**
>3. Can you compute it based on any other state or props in your component?**If so, it isn’t state.**

5. How can you identify where state needs to live?


***
***
### [Higher-Order Functions](https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK)

1. What is a “higher-order function”?
> Functions that operate on other functions, either by taking them as arguments or by returning them.

2. Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?
>Creating new function.

3. Explain how either map or reduce operates, with regards to higher-order functions.
>> The map method transforms an array by applying a function to all of its elements and building a new array from the returned values. The new array will have the same length as the input array, but its content will have been mapped to a new form by the function.

>> with reduce the higher-order operation that represents this pattern is called reduce (sometimes also called fold). It builds a value by repeatedly taking a single element from the array and combining it with the current value