## Debugging: Use the JavaScript Console to Check the Value of a Variable
```js
//Your code should use console.log() to check the value of the variable a.
let a = 5;
let b = 1;
a++;
// Add your code below this line
console.log(a);

let sumAB = a + b;
console.log(sumAB);
```
---
---
## Debugging: Understanding the Differences between the freeCodeCamp and Browser Console
```js
/*Use console.log() to print the outputTwo variable. In your Browser Console this should print out the value of the variable two times.
Use console.log() to print the outputOne variable.
Use console.clear() to modify your output so that outputOne variable only outputs once.*/
// Open your browser console
let outputTwo = "This will print to the browser console 2 times";
// Use console.log() to print the outputTwo variable
console.log(outputTwo);

let outputOne = "Try to get this to log only once to the browser console";
// Use console.clear() in the next line to print the outputOne only once

console.clear();
// Use console.log() to print the outputOne variable
console.log(outputOne);
```
---
---
## Debugging: Use typeof to Check the Type of a Variable
```js
//Add two console.log() statements to check the typeof each of the two variables seven and three in the code.
let seven = 7;
let three = "3";
console.log(seven + three);
// Add your code below this line
  console.log(typeof seven);
  console.log(typeof three);  
  // 73, number, string
```
---
---
## Debugging: Catch Misspelled Variable and Function Names
```js
// Fix the two spelling errors in the code so the netWorkingCapital calculation works.
/*Check the spelling of the two variables used in the netWorkingCapital calculation, the console output should show that "Net working capital is: 2".
There should be no instances of mis-spelled variables in the code.
The receivables variable should be declared and used properly in the code.
There should be no instances of mis-spelled variables in the code.
The payables variable should be declared and used properly in the code.*/
let receivables = 10;
let payables = 8;
let netWorkingCapital = recievables - payable;
console.log(`Net working capital is: ${netWorkingCapital}`);
// SOLUTION
let receivables = 10;
let payables = 8;
let netWorkingCapital = receivables - payables;
console.log(`Net working capital is: ${netWorkingCapital}`);
```
---
---
## Debugging: Catch Unclosed Parentheses, Brackets, Braces and Quotes
```js
//Fix the two pair errors in the code.
/*Fix the two pair errors in the code.*/
let myArray = [1, 2, 3;
let arraySum = myArray.reduce((previous, current =>  previous + current);
console.log(`Sum of array values is: ${arraySum}`);
// SOLUTION
let myArray = [1, 2, 3];
let arraySum = myArray.reduce((previous, current) =>  previous + current);
console.log(`Sum of array values is: ${arraySum}`);
```
---
---
## Debugging: Catch Mixed Usage of Single and Double Quotes
```js
/*Fix the string so it either uses different quotes for the href value, or escape the existing ones. Keep the double quote marks around the entire string. */
"use strict"

let innerHtml = "<p>Click here to <a href="#Home">return home.</a></p>"
console.log(innerHtml);
// SOLUTION
let innerHtml = "<p>Click here to <a href='#Home'>return home.</a></p>"
console.log(innerHtml);
//
let innerHtml = "<p>Click here to <a href=\"#Home\">return home</a></p>";
console.log(innerHtml);
```
---
---
## Debugging: Catch Use of Assignment Operator Instead of Equality Operator
```js
// Fix the condition so the program runs the right branch, and the appropriate value is assigned to result.
/*Your code should fix the condition so it checks for equality, instead of using assignment.
Passed
The condition can use either == or === to test for equality.*/
let x = 7;
let y = 9;
let result = "to come";

if(x = y) {
  result = "Equal!";
} else {
  result = "Not equal!";
}

console.log(result);
// SOLUTION
let x = 7;
let y = 9;
let result = "to come";

if(x === y) {
  result = "Equal!";
} else {
  result = "Not equal!";
}

console.log(result);
```
---
---
## Debugging: Catch Missing Open and Closing Parenthesis After a Function Call
```js
//Fix the code so the variable result is set to the value returned from calling the function getNine.
/*Your code should fix the variable result so it is set to the number that the function getNine returns.
Your code should call the getNine function.*/
function getNine() {
  let x = 6;
  let y = 3;
  return x + y;
}

let result = getNine;
console.log(result);
//SOLUTION
function getNine() {
  let x = 6;
  let y = 3;
  return x + y;
}

let result = getNine();
console.log(result);
```
---
---
## Debugging: Catch Arguments Passed in the Wrong Order When Calling a Function
```js
//The function raiseToPower raises a base to an exponent. Unfortunately, it's not called properly - fix the code so the value of power is the expected 8.
/*Your code should fix the variable power so it equals 2 raised to the 3rd power, not 3 raised to the 2nd power.
Your code should use the correct order of the arguments for the raiseToPower function call.*/
function raiseToPower(b, e) {
  return Math.pow(b, e);
}

let base = 2;
let exp = 3;
let power = raiseToPower(exp, base);
console.log(power);
// SOLUTION
function raiseToPower(b, e) {
  return Math.pow(b, e);
}

let base = 2;
let exp = 3;
let power = raiseToPower(base, exp);
console.log(power);
```
---
---
## Debugging: Catch Off By One Errors When Using Indexing
```js
// Fix the two indexing errors in the following function so all the numbers 1 through 5 are printed to the console.
/*Your code should set the initial condition of the loop so it starts at the first index.
Your code should fix the initial condition of the loop so that the index starts at 0.
Your code should set the terminal condition of the loop so it stops at the last index.
Your code should fix the terminal condition of the loop so that it stops at 1 before the length.*/
function countToFive() {
  let firstFive = "12345";
  let len = firstFive.length;
  // Fix the line below
  for (let i = 1; i <= len; i++) {
  //Do not alter code below this line
    console.log(firstFive[i]);
  }
}

countToFive();
// SOLUTION
 function countToFive() {
  let firstFive = "12345";
  let len = firstFive.length;
  // Fix the line below
  for (let i = 0; i < len; i++) {
  // Do not alter code below this line
    console.log(firstFive[i]);
  }
}

countToFive();

```
---
---
## Debugging: Use Caution When Reinitializing Variables Inside a Loop
```js
/*The following function is supposed to create a two-dimensional array with m rows and n columns of zeroes. Unfortunately, it's not producing the expected output because the row variable isn't being reinitialized (set back to an empty array) in the outer loop. Fix the code so it returns a correct 3x2 array of zeroes, which looks like [[0, 0], [0, 0], [0, 0]].
Your code should set the matrix variable to an array holding 3 rows of 2 columns of zeroes each.
The matrix variable should have 3 rows.
The matrix variable should have 2 columns in each row.*/
function zeroArray(m, n) {
  // Creates a 2-D array with m rows and n columns of zeroes
  let newArray = [];
  let row = [];
  for (let i = 0; i < m; i++) {
    // Adds the m-th row into newArray
    
    for (let j = 0; j < n; j++) {
      // Pushes n zeroes into the current row to create the columns
      row.push(0);
    }
    // Pushes the current row, which now has n zeroes in it, to the array
    newArray.push(row);
  }
  return newArray;
}

let matrix = zeroArray(3, 2);
console.log(matrix);
// SOLUTION
function zeroArray(m, n) {
  // Creates a 2-D array with m rows and n columns of zeroes
  let newArray = [];
 
  for (let i = 0; i < m; i++) {
    // Adds the m-th row into newArray
     let row = [];
    for (let j = 0; j < n; j++) {
      // Pushes n zeroes into the current row to create the columns
      row.push(0);
    }
    // Pushes the current row, which now has n zeroes in it, to the array
    newArray.push(row);
  }
  return newArray;
}

let matrix = zeroArray(3, 2);
console.log(matrix);
```
---
---
## Debugging: Prevent Infinite Loops with a Valid Terminal Condition
```js
/*The myFunc() function contains an infinite loop because the terminal condition i != 4 will never evaluate to false (and break the looping) - i will increment by 2 each pass, and jump right over 4 since i is odd to start. Fix the comparison operator in the terminal condition so the loop only runs for i less than or equal to 4.
Your code should change the comparison operator in the terminal condition (the middle part) of the for loop.
Your code should fix the comparison operator in the terminal condition of the loop.*/

function myFunc() {
  for (let i = 1; i != 4; i += 2) {
    console.log("Still going!");
  }
}

// SOLUTION

function myFunc() {
  for (let i = 1; i <= 4; i += 2) {
    console.log("Still going!");
  }
}
```
