# 16. Method chaining 
to make your 50 lines of method codes into 1 or 2, you can use method chaining. e.g.
```js
let username = window.prompt("type your username");

username =

  username.trim().charAt(0).toUpperCase() +

  username.trim().slice(1).toLowerCase();

console.log(username);
```

**More resources**: [MDN - JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)