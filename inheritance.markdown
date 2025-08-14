# 42. inheritance 
allows a new class to inherit the properties and method of an existing class. the existing class here becomes the parent and can extend to have multiple children. 
```js
class Laptop {
  RAM = "32GB";
  Processor = "i5 13405H";

  buy() {
    console.log(
      `You have sucessfully purchased ${this.name} laptop!\n It costed you $${this.price}`
    );
  }
}  
class Acer extends Laptop {
  name = "an Acer Aspire 7";
  price = "63,000";
}
 
class HP extends Laptop {
  name = "an HP Pavilionx36";
  price = "70,000";
}

const acer = new Acer();
const hp = new HP();

console.log(acer.RAM);
acer.buy();
hp.buy();

/* 
32GB
You have sucessfully purchased an Acer Aspire 7 laptop!
 It costed you $63,000
You have sucessfully purchased an HP Pavilionx36 laptop!
 It costed you $70,000
 /* 
```
So, as you can see here that the new laptops are inheriting the properties and methods of the parent (Laptop) like the `buy()` method. Each individual children can have their own new properties and methods too but that will only be accessible by the child itself, others will show undefined.

**More resources**: [MDN - JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)