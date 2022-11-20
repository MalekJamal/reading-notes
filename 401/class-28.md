# Redux

### What is redux?
> Redux is a predictable state container designed to help you write JavaScript apps that behave consistently across client, server, and native environments, and are easy to test.

### what is Redux used for?

> Simply put, Redux is used to maintain and update data across your applications for multiple components to share, all while remaining independent of the components.

> Without Redux, you would have to make data dependent on the components and pass it through different components to where it’s needed.

### What is state management in Redux?

> State management is essentially a way to facilitate communication and sharing of data across components. It creates a tangible data structure to represent the state of your app that you can read from and write to. That way, you can see otherwise invisible states while you’re working with them.

### How Redux works?

> The way Redux works is simple. There is a central store that holds the entire state of the application. Each component can access the stored state without having to send down props from one component to another.
There are three core components in Redux — actions, store, and reducers.


1) store hold all the data of our state (one big state). globalized state.
createStore(reducer)

2) Action, the action to update the state.(simple fuction return an object)

3) Reducer, describe how the actions transform the state into next state.(function take 2 params (state, action))

4) Dispatch, the way of how to excute the action, "dispatch this action to the rducer".

### What are Redux actions?

> Simply put, Redux actions are events.
They are the only way you can send data from your application to your Redux store. The data can be from user interactions, API calls, or even form submissions.
Actions are plain JavaScript objects that must have
a type property to indicate the type of action to be carried out, and
a payload object that contains the information that should be used to change the state.

> Actions are created via an action creator, which in simple terms is a function that returns an action. And actions are executed using the store.dispatch() method which sends the action to the store.
***

### What are Redux reducers?

> Reducers are pure functions that take the current state of an application, perform an action, and return a new state. The reducer handles how the state (application data) will change in response to an action.

> A pure function is a function that will always return the same value if given the same parameters. i.e. the function depends on only the parameters and no external data.

>  Reducers take the previous state of the app and return a new state based on the action passed to it. As pure functions, they do not change the data in the object passed to them or perform any side effect in the application. Given the same object, they should always produce the same result.

***
### What is Redux Store?
> The store is a “container” (really a JavaScript object) that holds the application state, and the only way the state can change is through actions dispatched to the store. Redux allows individual components connect to the store and apply changes to it by dispatching actions.

> It is highly recommended to keep only one store in any Redux application. You can access the state stored, update the state, and register or unregister listeners via helper methods.
***
### When to use Redux?

> Lately one of the biggest debates in the frontend world has been about Redux. Not long after its release, Redux became one of the hottest topics of discussion. Many favored it while others pointed out issues.

> Redux allows you to manage your app’s state in a single place and keep changes in your app more predictable and traceable. It makes it easier to reason about changes occurring in your app. But all of these benefits come with tradeoffs and constraints. One might feel it adds up boilerplate code, making simple things a little overwhelming; but that depends upon the architecture decisions.

> One simple answer to this question is you will realize for yourself when you need Redux. If you’re still confused as to whether you need it, you don’t. This usually happens when your app grows to the scale where managing app state becomes a hassle; and you start looking out for making it easy and simple.

## Resources
- [Understanding Redux](https://blog.logrocket.com/understanding-redux-tutorial-examples/#what-redux)
- [Redux](https://egghead.io/lessons/react-redux-avoiding-array-mutations-with-concat-slice-and-spread)

- [Getting Started with Redux
](https://redux.js.org/introduction/getting-started#basic-example)