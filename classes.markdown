# 40. Classes
so it is basically constructors but better and more structured way to use them as it has its own syntax and boilerplate. 
So, let's create the previous laptop example using classes now:
```js
class Laptop {
  constructor(name, processor, gpu, ram, price) {
    this.name = name;
    this.processor = processor;
    this.gpu = gpu;
    this.ram = ram;
    this.price = price;
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
  
laptop1.displayLaptop();

/* 
Name: acer
Processor: i5
GPU: RTX 3050
RAM: 16GB
Price: $60000
/*
```
so, Everything is pretty much the same but this one's obvious as a constructor as it has such syntax.

**More resources**: [MDN - JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)