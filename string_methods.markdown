# 14. String Methods
1. charAt - Lets you find out what is the character of selected index. e.g. 
```js
    let username = "MoonLight";
    username.charAt('0');
    console.log(username);
     // console will log the letter M  
```
2. indexOf - tells you the first occurrence of the character you are checking.
   e.g. 
   ```js
     let username = "MoonLight";
     console.log(username.indexOf("o"));
     // console will log 1.
     ```
3. lastIndexOf - tells you the last occurrence of a character. e.g.
   ```js
   let username = "MoonLight";
     console.log(username.lastIndexOf("o"));
     // console will log 6 this time.
    ```
4. length - a property added to a variable to check the length of the string characters. e.g.
   ```js
   let username = "Monalisa"
   console.log(username.length);
   // It will log 8.
     ```
5. trim - A method to remove any whitespaces (blank spaces) from a string. e.g.
   ```js
    let username = "  Monalisa  "
   console.log(username.trim());
   // console will log only Monalisa.
     ```
6. toUpperCase() and toLowerCase() - self explanatory.
7. repeat - to repeat a string. e.g,
   ```js
   username.repeat(5);
   // console will log MonalisaMonalisaMonalisaMonalisaMonalisa
      ```
8. endsWith and startsWith - returns a boolean if your string ends or starts with the value you are looking for. e.g.
   ```js
   username = "Monalisa"
   result1 = username.endsWith(" ");
   result2 = username.startsWith("M");
   console.log(result1, result2);
   // console will log false and true.
     ```
9. includes - looks for a value that is included in your string, returns boolean. e.g.
   ```js
   username.includes("M");
   // console will log true.
     ```
10. replaceAll - replaces all the selected value from a string. e.g. 
```js
    username.replaceAll("a", "o"); //first value is what to replace and second one is what to replace it with.
    // console will log Monoliso
```
11. padStart and padEnd - takes the first value as how long you want the string length to be and second value will add that value in the end or start to make the string match the length. e.g.
```js
    username.padStart(15, "M");
    username.padEnd(15, "A");
    // console will log "MMMMMMMMonalisa" and "MonalisaAAAAAAA"
```

**More resources**: [MDN - JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)