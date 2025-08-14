# 20. For loops 
works similarly like while loops but serves different purpose as for loops run the loop for a defined number of times. e.g.
```js
for (i = 0; i < 5; i++) {
  console.log(i);
}

/* result:
0
1
2
3
4
 */
```
so basically the first step `i = 0` is creating a variable to run the loop on, which is usually i for some reason and then setting up where the i will start from, that is 0 here.
then `i < 5` the loop will continue to run until this condition is false. meaning it will log 0 to 4 because 4 is smaller than 5. You can change the condition to `i <= 5` then it will log 5 too. lastly, what to do? `i++` increments the i every time the loop runs until the condition is met. 

**Additionally:**  Break and Continue keywords. You can add `break;` to stop executing the code at one point. e.g. 
```js
for (i = 0; i <= 5; i++) {
  if (i == 4) {
    break;
  } else {
    console.log(i);
  }
}
/* result: 
0
1
2
3
/*
```
so, here the console stops logging after the condition is true using the break keyword.

and the `continue;` keyword skips over the matching condition.  e.g.
```js
for (i = 0; i <= 5; i++) {
  if (i == 4) {
    continue;
  } else {
    console.log(i);
  }
}
/* result:
0
1
2
3
5
*/
```
as you can see it skipped 4 and continued logging the rest.

**More resources**: [MDN - JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)