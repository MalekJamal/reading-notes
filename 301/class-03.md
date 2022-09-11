## Lists and Keys
### Keys
> Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity:
```javascript
const numbers = [1, 2, 3, 4, 5];
const listItems = numbers.map((number) =>
  <li key={number.toString()}>
    {number}
  </li>
);
```
- The best way to pick a key is to use a string that uniquely identifies a list item among its siblings.
- Keys only make sense in the context of the surrounding array.
- Keys Must Only Be Unique Among Siblings
Keys used within arrays should be unique among their siblings. However, they don’t need to be globally unique.
- Keys serve as a hint to React but they don’t get passed to your components.

### JSX allows embedding any expression in curly braces so we could inline the map() result:
```javascript
function NumberList(props) {
  const numbers = props.numbers;
  return (
    <ul>
      {numbers.map((number) =>
        <ListItem key={number.toString()}
                  value={number} />
      )}
    </ul>
  );
}
```

1. What does .map() return?
> Return An array.

2. If I want to loop through an array and display each value in JSX, how do I do that in React?
>  By using the JavaScript map() function. And you can build collections of elements and include them in JSX using curly braces {}.
3. Each list item needs a unique >**ID**.

4. What is the purpose of a key?

> Keys serve as a hint to React but they don’t get passed to your components.

****
### The Spread Operator

1. What is the spread operator?
> The spread operator was added to JavaScript in ES6 (ES2015), just like the rest parameters, which have the same syntax: three magic dots …

2. List 4 things that the spread operator can do.
> - Copying an array.
> - Concatenating or combining arrays.
> - Using Math functions.
> - Using an array as arguments.
> - Adding an item to a list.
> - Adding to state in React.
> - Combining objects.
> - Converting NodeList to an array.

3. Give an example of using the spread operator to combine two arrays.
```javascript
const myArray = [`🤪`,`🐻`,`🎌`]
const yourArray = [`🙂`,`🤗`,`🤩`]
const ourArray = [...myArray,...yourArray]
console.log(...ourArray) // 🤪 🐻 🎌 🙂 🤗 🤩
```
4. Give an example of using the spread operator to add a new item to an array.
```javascript
const fruits = ['🍏','🍊','🍌','🍉','🍍']
const moreFruits = [...fruits];
console.log(moreFruits) // Array(5) [ "🍏", "🍊", "🍌", "🍉", "🍍" ]
fruits[0] = '🍑'
console.log(...[...fruits,'...',...moreFruits]) //  🍑 🍊 🍌 🍉 🍍 ... 🍏 🍊 🍌 🍉 🍍
```
5. Give an example of using the spread operator to combine two objects into one.
```javascript
const objectOne = {hello: "🤪"}
const objectTwo = {world: "🐻"}
const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}
console.log(objectThree) // Object { hello: "🤪", world: "🐻", laugh: "😂" }
const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("😂".repeat(5))}}
objectFour.laugh() // 😂😂😂😂😂
 ```
![ browser compatibility ](https://miro.medium.com/max/700/1*eqKBiABFRy_uEBdchVZ9Qw.png)
***
***
#### [React - How to Pass Functions between Components](https://www.youtube.com/watch?v=c05OL7XbwXU)

1. In the video, what is the first step that the developer does to pass functions between components?
> Pass it just like any other props, create the refernce to the function in the parent class.
```javascript
increment={this.increment},
```

2. In your own words, what does the increment function do?
> Increment the state count for each person by 1.

3. How can you pass a method from a parent component into a child component?
> Using props
4. How does the child component invoke a method that was passed to it from a parent component?
> And use the method in the child component by adding this line inside the child increment method.
```this.props.incremet,```
****
****

- [Lists and Keys](https://reactjs.org/docs/lists-and-keys.html)

- [Spread Operator ](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)
- [React - How to Pass Functions between Components](https://www.youtube.com/watch?v=c05OL7XbwXU)

### Bookmark and Review
- [React Tutorial through ‘Declaring a Winner’](https://reactjs.org/tutorial/tutorial.html)
- [React Docs - Lifting State Up](https://reactjs.org/docs/lifting-state-up.html)

## Things I want to know more about
- Lists and Keys
- Spread Operator