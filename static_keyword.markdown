# 41. Static keyword
a keyword that defines properties or methods and those directly belong to the class rather than an object. for example: 
```js
class Laptop {
  static laptopCount = 0; // Added here
  constructor(name, processor, gpu, ram, price) {
    this.name = name;
    this.processor = processor;
    this.gpu = gpu;
    this.ram = ram;
    this.price = price;
    Laptop.laptopCount++;
  }

  displayLaptop() {
    console.log(`Name: ${this.name}`);
    console.log(`Processor: ${this.processor}`);
    console.log(`GPU: ${this.gpu}`);
    console.log(`RAM: ${this.ram}`);
    console.log(`Price: $${this.price}`);
  }
}

const laptop1 = new Laptop("acer", "i5", "RTX 3050", "16GB", 60000);
const laptop2 = new Laptop(
  "HP",
  "i3",
  "Integrated intel iris Xe",
  "8GB",
  35000
);
  
console.log(Laptop.laptopCount); //logging

// 2
```
so basically, statics can be logged using the class name only, no need to create a new object and also it is useful for cases like this!

**More resources**: [MDN - JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)