# 4. Accept user input
There are two ways to accept user input in JavaScript.
1. You can use the prompt window.
     *Use the prompt window to ask for user input.*
     ```js
       let age;
       age = window.prompt("what is your age?");
       console.log(age);  
       ```
2. You can use HTML and DOM manipulation (professional).
     Add heading, input, label and a submit button in your HTML file.
     use `document.getElementById("")` to get all the HTML tags by their IDs (don't forget to add one) and then take user input using the input tag and `inputTagName.value` (this will log the user's typed value) and then edit the text content of the heading or paragraph using `textContent`

**More resources**: [MDN - JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)