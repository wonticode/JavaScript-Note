# 33. filter()
creates a new array by filtering out elements, basically it takes a callback and filters if the elements returns true. Yeah, It takes Boolean.
```js
const numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9];

function isOdd(element) {
  return element % 2 !== 0;
}

console.log(numbers.filter(isOdd));

// [ 1, 3, 5, 7, 9 ]
```
so, we can see inside the isOdd function; it is checking if each element in that array is being divided by 2 and if the reminder is strictly NOT equal to 0. If yes, it will return true and those elements will be shown in a new array.

**More resources**: [MDN - JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)