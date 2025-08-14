# 32. map()
similar to forEach but it creates a new array and returns it as an array while forEach changes the same array and then returns undefined.
Map takes a callback and applies to each element of an array and then returns a new Array. 
```js
const fruits = ["Banana", "Apple", "Mango", "kale"];

let uppercaseFruits = fruits.map(uppercase);

function uppercase(fruit) {
  return fruit.toUpperCase();
}

console.log(uppercaseFruits);

// [ 'BANANA', 'APPLE', 'MANGO', 'KALE' ]
```
but using forEach we get:
```js
const fruits = ["Banana", "Apple", "Mango", "kale"];

fruits.forEach(uppercase);

function uppercase(elememt, index, array) {
  array[index] = elememt.toUpperCase();
  console.log(elememt);
}

/* Banana
Apple
Mango
kale
/* 
```

**More resources**: [MDN - JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)