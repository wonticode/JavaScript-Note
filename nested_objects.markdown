# 46. Nested Objects
An object contained in another so, a parent object having children. pretty simple and they can be accessed using the same way properties of objects are accessed but one needs to `parent.child1.child2.child3`  and so on, for example:
```js
const pokemon = {
  name: "Pikachu",
  attack: {
    atk: 7,
    spA: 5,
  },

  defense: {
    def: 9,
    spD: 7,
  },
};
  
console.log(pokemon.attack.atk);

// 7
```
It works! It can also be used in classes using the same.

**More resources**: [MDN - JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)