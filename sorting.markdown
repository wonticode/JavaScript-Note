# 48. Sorting
a method used to sort elements of an array in place. It sorts elements as strings in lexicographic order which are not alphabetical. They are basically (alphabets + numbers + symbols) as strings. It will fuck up if you try to do this:
```js
const numbers = [3, 4, 5, 30, 4, 3];
numbers.sort();
console.log(numbers);

// [ 3, 3, 30, 4, 4, 5 ]
```
as you can see how 30 has been sorted before 4...while it is OBVIOULSY larger than any of those numbers, duh!
we can do something like this in such cases:
```js
const numbers = [3, 4, 5, 30, 4, 3];
numbers.sort((a, b) => a - b);
console.log(numbers);

// [ 3, 3, 4, 4, 5, 30 ]
```
Well, this basically compares two numbers together and checks their result and swap them based on the result being positive or negative, don't think much. Just use it and also, if you want it in descending order then do `b - a` instead.

**More resources**: [MDN - JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)