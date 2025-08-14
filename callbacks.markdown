# 30. Callbacks
A function that is passed down as an argument for another function. 

used to handle asynchronous operations: 
1. Reading a file
2. Network Requests
3. Interacting with Databases

"When you are done, call this next"  e.g.
```js
function sum(callback, x, y) {
  let result = x + y;
  callback(result);
}
function displayConsole(result) {
  console.log(result);
} 
sum(displayConsole, 5, 6);

// 11
```
here the function sum is adding x and y and invoking the callback parameter right after.
in the displayConsole function, we are naming the parameter result and logging it to console, meaning whatever we get as parameter to the displayConsole function will be logged to console. 
When we are calling the sum function `sum(displayConsole, 5, 6);` we are putting displayConsole as the callback and in the sum function the callback will be invoked with result as its parameter, In this case, The displayConsole function gets invoked and logs result. I HOPE IT MAKES SENSE. 

**A simpler example would be:** 
```js
function hello(callback) {
  console.log("Hello");
  callback();
}
function bye() {
  console.log("Bye");
}
hello(bye);

// Hello
// bye
```
the function hello is calling the bye function and it makes sure that the bye function gets invoked after the hello function. the bye function in `hello(bye);` is the callback function.

**More resources**: [MDN - JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)