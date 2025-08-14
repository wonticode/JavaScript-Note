# 44. Getters and Setters
getters - special method that makes a property readable.
setters - another method that makes a property writable. 

They help you validate a value when reading/writing a property.

```js
class Laptop {
  constructor(name, price) {
    this.name = name;
    this.price = price;
  }

  buy() {
    console.log(
      `You have sucessfully purchased ${this.name} laptop!\n It costed you $${this.price}`
    );
  }

  
  set name(value) {
    if (value.length > 1) {
      this._name = value;
    } else {
      console.error("Please write a valid laptop name.");
    }
  }
}
  
class Acer extends Laptop {}

const acer = new Acer(" ", "lala"); //garbage values

console.log(acer.name);

// Please write a valid laptop name.
// undefined
```
So, as you can see it works and throws a manual error for it and the value is undefined now. but even if you put a valid name for the `name` it will still show undefined because with setters we also need getters. so, let's add it. oh also, you need to use the private property thing like `this._name` I don't know what the exact use is but the code breaks if you don't use it. 

```js
  get name() {
    return this._name; //added a get method after the set method.
  }
  const acer = new Acer("Hello", "lala");
 
 // Hello
```
and it works! So, this is how getters and setters work, you can even do stuff with what you get in getters like adding or removing something from it e.g. 
```js
  get name() {
    return this._name + "!";
  }
 // Hello!
```
and That is how it works!

**More resources**: [MDN - JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)