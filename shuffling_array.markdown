# 49. Shuffling an Array
This is not some built in method or anything but rather a formula to shuffle things effectively in games or something similar where you need proper shuffling. 
```js
const array = ["em1", "em2", "em3", "em4", "em5"];
shuffle(array);

function shuffle(array) {
  for (let i = array.length - 1; i > 0; i--) {
    const RandomIndex = Math.floor(Math.random() * (i + 1));
    [array[i], array[RandomIndex]] = [array[RandomIndex], array[i]];
  }
}
console.log(array);

// will log different order each time.
```
The logic is simple, the loop will run till `i` is greater than 0 where `i` is `array.length - 1` because index of an array starts from 0. then, we will get a random index (since it is index again, we will add 1 because an index is not equal to the length; sucks.) and then we will use deconstructing to replace the looping array with a random index and so on.

**More resources**: [MDN - JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)