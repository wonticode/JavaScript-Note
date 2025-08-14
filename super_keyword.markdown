# 43. Super keyword
Super keyword is used to call the constructor in a class or, use the properties and methods of a parent class (superclass). 

> [!info] Similar to this keyword
> This = this object
> Super = parent object

So, let's try it out on the previous example we have been using all along, this time we will not rewrite the properties and just reuse it by declaring them in the parent class. 

```js
class Laptop {
  constructor(name, price) {
    this.name = name;
    this.price = price; // created a constructor and added parent property.
  }
 
  buy() {
    console.log(
      `You have sucessfully purchased ${this.name} laptop!\n It costed you $${this.price}`
    );
  }
}
  
class Acer extends Laptop {} //removed duplicate code from here.
class HP extends Laptop {}

const acer = new Acer("an Acer Aspire 7", "63,000"); //added the individual property values here.
const hp = new HP("an HP Pavilionx36", "70,000");

acer.buy();
hp.buy();

/* 
You have sucessfully purchased an Acer Aspire 7 laptop!
 It costed you $63,000
You have sucessfully purchased an HP Pavilionx36 laptop!
 It costed you $70,000
 /* 
```
So, this code works but you don't see a super keyword here, do you? 
You must be wondering where is it used then? well, because since `HP` and `Acer` here do not have any individual properties or methods of their own; we probably don't need super keyword but let's try adding one!
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
}
  
class Acer extends Laptop {
  buy() {
    console.log("You get a FREE Acer bag!");
  }
}

class HP extends Laptop {}
const acer = new Acer("an Acer Aspire 7", "63,000");
const hp = new HP("an HP Pavilionx36", "70,000");  
acer.buy();

// You get a FREE Acer bag!
```
So, we tried it but now the buy method is only logging what we set up in Acer's buy method and doesn't log the one in `Laptop` what to do now? Let's try using super here.
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
}

class Acer extends Laptop {
  buy() {
    super.buy();
    console.log("You get a FREE Acer bag!");
  }
}

class HP extends Laptop {}
const acer = new Acer("an Acer Aspire 7", "63,000");
const hp = new HP("an HP Pavilionx36", "70,000");
  
acer.buy();

/*
You have sucessfully purchased an Acer Aspire 7 laptop!
 It costed you $63,000
You get a FREE Acer bag!
/*
```
Here, we are calling the buy method from the parent/super class `super.buy();` so, it logs both the new and previous methods and thus, the result. that is where you can use Super!

**More resources**: [MDN - JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)