# 47. Arrays of Objects
as the name suggests, an Array of objects is an array of objects. Yeah. An Array that has multiple objects in it. That way you don't have to name each object for something and you can just access them by their index.
```js
const oil = [
  { name: "oil1", price: 8 },
  { name: "oil2", price: 9 },
  { name: "oil3", price: 4 },
];
  
console.log(oil[1]);
console.log(oil[0].price);

// { name: 'oil2', price: 9 }
// 8
```
And it works! Fairly simple as well and using this, you can also use the array methods on objects >:3

**More resources**: [MDN - JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)