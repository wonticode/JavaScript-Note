# 31. forEach()
Method used to iterate over the elements of an Array and apply a specified function (callback) to each element of that array.
To use - `array.forEach(callback)`
It is basically a in built loop for arrays. Very useful. 
**It takes 3 arguments that are element, index, array.**
```js
const fruits = ["Banana", "Apple", "Mango", "kale"];
fruits.forEach(upperCase);
fruits.forEach(display);

function upperCase(element, index, array) {
  array[index] = element.toUpperCase()
}
  
function display(element) {
  console.log(element);
}

/* 
BANANA
APPLE
MANGO
KALE
*/
```
so, here the forEach method is attached to an array named fruits and it is going to convert every string in there in uppercase, using the for each method we are going to iterate (`array[index] = element.toUpperCase()`) over the array's each index (meaning every string in there) and turn every element which are the strings stored in the array (`["Banana", "Apple", "Mango", "kale"]`)  to upper case. and then we will call the function again to display all the elements using the display function as callback.

**More resources**: [MDN - JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)