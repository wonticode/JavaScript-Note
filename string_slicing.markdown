# 15. String slicing 
Helps you to get a substring out of the portion of a string. often combined with indexOf method to use properly and make it more dynamic. It takes two values, first as where to start the slicing and 2nd as where to end it.
e.g. 
```js
const email = "kendenza@gmail.com";

let emailDomain = email.slice(email.indexOf("@"));

console.log(emailDomain);

// console logs @gmail.com
```

**More resources**: [MDN - JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)