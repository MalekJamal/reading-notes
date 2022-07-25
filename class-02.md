## State and Props

1. **Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?**
>  When the component file is called it calls the render() method by default because that component needs to display the HTML markup or we can say JSX syntax.

1. **What is the very first thing to happen in the lifecycle of React?**

>> Mounting.

3. Put the following things in the order that they happen: **componentDidMount**, **render**, constructor, **componentWillUnmount**, **React Updates**.
> 1. render.
> 2. componentDidMount.
> 3. React Updates.
> 4. componentWillUnmount.

***
***
1. **What types of things can you pass in the props?**
> It's like argumants for a function

2. **What is the big difference between props and state?**

> State inside the component, props pass into the component and handles outside the component and must update oustside the component, and state handles inside that component.

3. **When do we re-render our application?**
> When change the state inside the app

4. **What are some examples of things that we could store in state?**
> user input.(counter)