# 38. this
a reference to the object where THIS is used. e.g. 
```js
const person1 = {
  name: "Mana",
  age: 16,
  sayHello: function () {
    console.log(`hello, this is ${this.name}`);
  },
};

person1.sayHello();

// hello, this is Mana
```
well, it is like using person1 there rather than this but one benefit of it seems like you can change the object name without having to change anything there.

**More resources**: [MDN - JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)