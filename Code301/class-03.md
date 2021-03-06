![react](https://i.ibb.co/bgwz2Ky/Webp-net-resizeimage-1.png)
# React

## What does .map() return?
A new array has the same length as orginal array with each element being the result of the callback function.
## If I want to loop through an array and display each value in JSX, how do I do that in React?
You can build collections of elements and include them in JSX using curly braces {}.
```
{Array.map(value => <h3>value<h3/>)}
```
## Each list item needs a unique ____.
Key
## What is the purpose of a key?
Keys help React identify which items have changed, are added, or are removed.
## What is the spread operator?
Spread operator refers to the use of an ellipsis of three dots (âĶ) to expand an iterable object into the list of arguments.
## List 4 things that the spread operator can do.
1. find the largest number in an array with Math.max().
2. Copying an array.
3. Concatenating or combining arrays
4. Adding an item to a list

## Give an example of using the spread operator to combine two arrays.
```
const myArray = [`ðĪŠ`,`ðŧ`,`ð`]
const yourArray = [`ð`,`ðĪ`,`ðĪĐ`]
const ourArray = [...myArray,...yourArray]
console.log(...ourArray) // ðĪŠ ðŧ ð ð ðĪ ðĪĐ
```
## Give an example of using the spread operator to add a new item to an array.
```
const fewFruit = ['ð','ð','ð']
const fewMoreFruit = ['ð', 'ð', ...fewFruit]
console.log(fewMoreFruit) //  Array(5) [ "ð", "ð", "ð", "ð", "ð" ]
```
## Give an example of using the spread operator to combine two objects into one.
```
const objectOne = {hello: "ðĪŠ"}
const objectTwo = {world: "ðŧ"}
const objectThree = {...objectOne, ...objectTwo, laugh: "ð"}
console.log(objectThree) // Object { hello: "ðĪŠ", world: "ðŧ", laugh: "ð" }
const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("ð".repeat(5))}}
objectFour.laugh() // ððððð
```
## what is the first step that the developer does to pass functions between components?
implement the function :) 
## In your own words, what does the increment function do?
increment the count of selected person object
## How can you pass a method from a parent component into a child component?
just like props
## How does the child component invoke a method that was passed to it from a parent component?
 by calling the function received in props
 
### Helpful resources:
- [Lists and Keys](https://reactjs.org/docs/lists-and-keys.html)
- [The Spread Operator](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)
- [How to Pass Functions Between Components](https://www.youtube.com/watch?v=c05OL7XbwXU)
