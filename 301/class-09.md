# Readings: Functional Programming
- [Functional Programming Concepts](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)
***
1. What is functional programming?
>Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data — Wikipedia.

2. What is a pure function and how do we know if something is a pure function?
> - It returns the same result if given the same arguments.
> - Pure functions are stable, consistent, and predictable.
> - If our function reads external files, it’s not a pure function — the file’s contents can change.
> - It does not cause any observable side effects
> - Any function that relies on a random number generator cannot be pure.

3. What are the benefits of a pure function?
> The code’s definitely easier to test. We don’t need to mock anything. So we can unit test pure functions with different contexts:
> - Given a parameter A → expect the function to return value B
> - Given a parameter C → expect the function to return value D

4. What is immutability?
>Unchanging over time or unable to be changed.
>When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.
5. What is Referential transparency?
> - pure functions + immutable data = referential transparency
***
***
- [Node JS Tutorial for Beginners #6 - Modules and require()](https://www.youtube.com/watch?v=xHLd36QoS4k)

1. What is a module?
> A module in JavaScript is just simply a file containing related code.
2. What does the word ‘require’ do?
> is a built-in function to include external modules that exist in separate files.
> require() statement basically reads a JavaScript file, executes it, and then proceeds to return the export object.
3. How do we bring another module into the file the we are working in?
> first thing we need to import it, then use it but it should be exported so we can use it.
> - ```const module_name = require("/the module path");```.
> - then we can use it.


4. What do we have to do to make a module available?
> ```module.exports = the code we need to be available to use globaly (functions, classes,...). ```