# 45. Deconstructing
extract values from arrays and objects and assign them to a variable in a convenient way. 

> [!info] Symbols to use
> [ ] = to deconstruct an array
> { } = to deconstruct an object

Then Let's check out the example.  First we will deconstruct an Array
```js
const names = ["Munnu", "Chunnu", "Punnu"];
[names[0], names[2]] = [names[2], names[0]];
console.log(names);

// [ 'Punnu', 'Chunnu', 'Munnu' ]
```
It works! Munnu has been replaced by Punnu and vice versa. 
Now another example would be:
```js
const names = ["Munnu", "Chunnu", "Punnu", "Gunnu"];
const [firstPerson, secondPerson, ...others] = names;
console.log(others);

// [ 'Punnu', 'Gunnu' ]
```

We can also use the same to give our array elements a name by declaring them like above. 
We used the Rest parameter here to combine `Punnu` and `Gunnu` in the `...others` variable.  

Now for objects, it is similar:
```js
const pokemon = {
  name: "Pikachu",
  attack: 13,
  defense: 9,
};

const { name, attack, defense } = pokemon; 
console.log(name);

// Pikachu
```
Well, unlike arrays you can't just give them a different name but turning the properties of an object into variables make it accessible without having to type `pokemon.name` to access it as you can just do `name`.
It works the same in functions too.

**More resources**: [MDN - JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)