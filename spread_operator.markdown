# 26. Spread operator 
a spread operator basically helps you to unpack or spread an array or a string. e.g.
```js
let numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9];
let max = Math.max(numbers);
console.log(max);
// NaN
```
If we try to log max as an array in `Math.max` function, we get NaN because an Array itself is not a number but...
```js
let numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9];
let max = Math.max(...numbers);
console.log(max);
// 9
```
if we use the spread operator here before the numbers array, it will unpack the array and then we can get the maximum number by using the `Math.max` function.

A Spread operator can also be used on string using the same. e.g.
```js
let string = "Munni";
console.log(...string);
// M u n n i
```
you can also log your string as an array of the substrings. e.g.
```js
let string = "Munni";
let letters = [...string];
console.log(letters);
// [ 'M', 'u', 'n', 'n', 'i' ]
```

 **Join method**
using the join method you can join all the strings in an Array. `array.join(separator)` the default separator is comma. e.g. 
```js
let string = "Munni";
let letters = [...string].join(" ");
console.log(letters);
// M u n n i
```
as you can see the array is now a string with space between each letter.

**More resources**: [MDN - JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)