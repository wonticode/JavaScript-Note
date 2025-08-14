# 34. reduce()
Reduces the elements of an array to a single value. 
```js
const prices = [21, 54, 37, 92, 33, 12];

function sum(accumulator, element) {
  return accumulator + element;
}

console.log(prices.reduce(sum));

// 249
```
The `accumulator` here is basically, It will start from 0 and will be added to the element and then it will become the result of first addition and then the result will be added to element again and so on...
like: 0 + 21 = 21; 21 + 54 = 75; 75 + 37 = 112, etc.

**More resources**: [MDN - JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)