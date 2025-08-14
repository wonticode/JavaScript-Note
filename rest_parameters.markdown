# 27. Rest parameters
Bundles separate elements into an array contrary to the spread operator. can only be used on parameters. e.g.
```js
const food1 = "Biscuit";
const food2 = "Nameen";
const food3 = "bhujiya";
const food4 = "Papad";
const food5 = "golgappe";

function fridge(...foods) {
  console.log(foods);
}

fridge(food1, food2, food3, food4, food5);

// [ 'Biscuit', 'Nameen', 'bhujiya', 'Papad', 'golgappe' ]
```
but if we combine it with the spread operator like: 
```js
function fridge(...foods) {
  console.log(...foods);
}
// Biscuit Nameen bhujiya Papad golgappe
```
It now logs them as a string.

**More resources**: [MDN - JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)