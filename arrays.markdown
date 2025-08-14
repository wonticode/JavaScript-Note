# 24. Arrays
works like a box that stores strings, numbers, boolean or any values. 
e.g. 
```js
let veges = ["Tomato", "Potato", "Onion"]
```
These strings under the Array can be accessed using indexes like `veges[0]` for Tomato or the first value in the array. The same way one can change the array like 
```js
veges[0] = "Spring onion";
```

**Methods to modify the array.**
1. push() - you can use this to add a value in the end of the array.
   ```js
      veges.push("Kale");
      // ["Tomato", "Potato", "Onion", "Kale"]
    ```
2. pop() - to remove the last value from an array. 
3. unshift() - to add a value to the beginning of an array. 
4. shift() - to remove an element from the beginning of an array. 
5. length - the length property can also be used on an array to know how many elements the array has. 
6. indexOf - other than using it on a string to find the index of a substring, indexOf method can be used on arrays to find a specific value. e.g. `veges.indexOf("Onion")`

  **for loops to display an Array.**
1. The regular for loop to log an array. e.g.
   ```js
   let fruits = ["mango", "banana", "orange"];
for (let i = 0; i < fruits.length; i++) {
  console.log(fruits[i]);
}
     ```
2. a for loop e.g.
   ```js
   for (let fruit of fruits) {
  console.log(fruit);
} 
     ```

 **to sort an array:**
3. sort() - It will sort the array in an alphabetical order. e.g. `arr.sort()`
4. sort().reverse() - to sort the array in reverse alphabetical order. e.g. `arr.sort().reverse()`

**More resources**: [MDN - JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)