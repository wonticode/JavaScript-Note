# 39. constructors 
special property for defining the methods and properties of an object.
It makes the code reusable and you don't have to update the original object again and again. 
```js
function Laptop(name, processor, gpu, ram, price) {
  (this.name = name),
    (this.processor = processor),
    (this.gpu = gpu),
    (this.ram = ram),
    (this.price = price);
}

const laptop1 = new Laptop("acer", "i5", "RTX 3050", "16GB", 60000);
const laptop2 = new Laptop( "HP", "i3", "Integrated intel iris Xe",
  "8GB",
  35000
);

console.log(laptop1.name);

console.log(laptop2);

/* 
acer
Laptop {
  name: 'HP',
  processor: 'i3',
  gpu: 'Integrated intel iris Xe',
  ram: '8GB',
  price: 35000
} 
/*
```
So, as you can see it is a convenient way of creating an object, some things to remember here is the format and that we write a constructor function's name in normal English like first letter capital. 
>  When `new` is used, it performs several actions: it creates a new empty object.

This is how new works. a constructor utilizes the new and this keywords.

**More resources**: [MDN - JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)