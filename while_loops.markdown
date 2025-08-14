# 19. While loops 
Basically written like an if else statement but are loops. Logic is the loop will keep running till the condition is true. e.g.
```js
let yourName = "";
while (yourName === "") {
  yourName = window.prompt("Type your name...");
}
console.log(`Hello ${yourName}`);

// keep running until the user types something in the prompt window.
```
Another type of while loop is do while loop. basically if the condition is false, the loop will still run once. e.g.
```js
let yourName = "Mama";
do {
  yourName = window.prompt("Type your name...");
} while (yourName === "");
console.log(`Hello ${yourName}`);

// the loop will run once even when the condition is false here. It will keep running till the condition is false again.
```

**More resources**: [MDN - JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)