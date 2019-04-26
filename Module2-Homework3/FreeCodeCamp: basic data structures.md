## Introduction to the Basic Data Structure Challenges
---
## Basic Data Structures: Use an Array to Store a Collection of Data
```js
/*We have defined a variable called yourArray. Complete the statement by assigning an array of at least 5 elements in length to the yourArray variable. Your array should contain at least one string, one number, and one boolean.

yourArray is an array
yourArray is at least 5 elements long
yourArray contains at least one boolean
yourArray contains at least one number
yourArray contains at least one string*/

let yourArray; // change this line

// SOLUTION
let yourArray = ["1", 2, true, undefined, null]; // change this line
```
---
---
## Basic Data Structures: Access an Array's Contents Using Bracket Notation
```js
//In order to complete this challenge, set the 2nd position (index 1) of myArray to anything you want, besides "b".
/*myArray[0] is equal to "a"
myArray[1] is no longer set to "b"
myArray[2] is equal to "c"
myArray[3] is equal to "d"*/

let myArray = ["a", "b", "c", "d"];
// change code below this line

//change code above this line
console.log(myArray);

// SOLUTION

let myArray = ["a", "b", "c", "d"];
// change code below this line
myArray[1] = "e"
//change code above this line
console.log(myArray);


```
---
---
## Basic Data Structures: Add Items to an Array with push() and unshift()
```js
/*We have defined a function, mixedNumbers, which we are passing an array as an argument. Modify the function by using push() and unshift() to add 'I', 2, 'three' to the beginning of the array and 7, 'VIII', 9 to the end so that the returned array contains representations of the numbers 1-9 in order.*/

function mixedNumbers(arr) {
  // change code below this line

  // change code above this line
  return arr;
}

// do not change code below this line
console.log(mixedNumbers(['IV', 5, 'six']));

// SOLUTION

function mixedNumbers(arr) {
  // change code below this line
 /*arr.unshift("three");
  arr.unshift(2);
  arr.unshift("I");
  arr.push(7);
  arr.push("VIII");
  arr.push(9);*/
  arr.unshift('I', 2, 'three');
  arr.push(7, 'VIII', 9);
  // change code above this line
  return arr;
}

// do not change code below this line
console.log(mixedNumbers(['IV', 5, 'six']));
```
---
---
## Basic Data Structures: Remove Items from an Array with pop() and shift()
```js
/*We have defined a function, popShift, which takes an array as an argument and returns a new array. Modify the function, using pop() and shift(), to remove the first and last elements of the argument array, and assign the removed elements to their corresponding variables, so that the returned array contains their values.
popShift(["challenge", "is", "not", "complete"]) should return ["challenge", "complete"]
The popShift function should utilize the pop() method
The popShift function should utilize the shift() method
*/
function popShift(arr) {
  let popped; // change this line
  let shifted; // change this line
  return [shifted, popped];
}

// do not change code below this line
console.log(popShift(['challenge', 'is', 'not', 'complete']));

// SOLUTION

function popShift(arr) {
  let popped = arr.pop(); // change this line
  let shifted = arr.shift(); // change this line
  return [shifted, popped];
}

// do not change code below this line
console.log(popShift(['challenge', 'is', 'not', 'complete']));
```
---
---
## Basic Data Structures: Remove Items Using splice()
```js
/*We've defined a function, sumOfTen, which takes an array as an argument and returns the sum of that array's elements. Modify the function, using splice(), so that it returns a value of 10.
sumOfTen should return 10
The sumOfTen function should utilize the splice() method*/

// do not change code below this lineconsole.log(sumOfTen([2, 5, 1, 5, 2, 1]));}     // change code above this line  return arr.reduce((a, b) => a + b);function sumOfTen(arr) {  // change code below this line
function sumOfTen(arr) {
  // change code below this line
  
  // change code above this line
  return arr.reduce((a, b) => a + b);
}

// do not change code below this line
console.log(sumOfTen([2, 5, 1, 5, 2, 1]));

// SOLUTION

function sumOfTen(arr) {
  // change code below this line
  arr.splice(1,2);
  // change code above this line
  return arr.reduce((a, b) => a + b);
}

// do not change code below this line
console.log(sumOfTen([2, 5, 1, 5, 2, 1]));

```
---
---
## Basic Data Structures: Add Items Using splice()
```js
/*We have defined a function, htmlColorNames, which takes an array of HTML colors as an argument. Modify the function using splice() to remove the first two elements of the array and add 'DarkSalmon' and 'BlanchedAlmond' in their respective places.
htmlColorNames should return ["DarkSalmon", "BlanchedAlmond", "LavenderBlush", "PaleTurqoise", "FireBrick"]
Passed
The htmlColorNames function should utilize the splice() method
Passed
You should not use shift() or unshift().
Passed
You should not use array bracket notation.*/
// SOLUTION
function htmlColorNames(arr) {
  // change code below this line
  arr.splice(0, 2, 'DarkSalmon', 'BlanchedAlmond');
  // change code above this line
  return arr;
} 
 
// do not change code below this line
console.log(htmlColorNames(['DarkGoldenRod', 'WhiteSmoke', 'LavenderBlush', 'PaleTurqoise', 'FireBrick']));
```
---
---
## Basic Data Structures: Copy Array Items Using slice()
```js
/*We have defined a function, forecast, that takes an array as an argument. Modify the function using slice() to extract information from the argument array and return a new array that contains the elements 'warm' and 'sunny'.
forecast should return ["warm", "sunny"]
The forecast function should utilize the slice() method*/

function forecast(arr) {
  // change code below this line
  
  return arr;
}

// do not change code below this line
console.log(forecast(['cold', 'rainy', 'warm', 'sunny', 'cool', 'thunderstorms']));

// SOLUTION

function forecast(arr) {
  // change code below this line
  var newArr = arr.slice(2, 4);
  return newArr;
}

// do not change code below this line
console.log(forecast(['cold', 'rainy', 'warm', 'sunny', 'cool', 'thunderstorms']));
```
---
---
## Basic Data Structures: Copy an Array with the Spread Operator
```js
/*We have defined a function, copyMachine which takes arr (an array) and num (a number) as arguments. The function is supposed to return a new array made up of num copies of arr. We have done most of the work for you, but it doesn't work quite right yet. Modify the function using spread syntax so that it works correctly (hint: another method we have already covered might come in handy here!).*/
/*
copyMachine([true, false, true], 2) should return [[true, false, true], [true, false, true]]
copyMachine([1, 2, 3], 5) should return [[1, 2, 3], [1, 2, 3], [1, 2, 3], [1, 2, 3], [1, 2, 3]]
copyMachine([true, true, null], 1) should return [[true, true, null]]
copyMachine(["it works"], 3) should return [["it works"], ["it works"], ["it works"]]
The copyMachine function should utilize the spread operator with array arr
*/

function copyMachine(arr, num) {  let newArr = [];  while (num >= 1) {    // change code below this line     // change code above this line    num--;  }  return newArr;} // change code here to test different cases:console.log(copyMachine([true, false, true], 2));

// change code here to test different cases:
console.log(copyMachine([true, false, true], 2));

// SOLUTION

function copyMachine(arr, num) {
  
  let myArr = [];
  let newArr = [...arr];
  while (num >= 1) {
    // change code below this line
myArr.push(newArr);
    // change code above this line
    num--;
  }
  newArr = [...myArr];
  return newArr;
}

// change code here to test different cases:
console.log(copyMachine([true, false, true], 2));

//
function copyMachine(arr, num) {
  let newArr = [];
  while (num >= 1) {
    // change code below this line
newArr.push([...arr]);
    // change code above this line
    num--;
  }
  return newArr;
}

// change code here to test different cases:
console.log(copyMachine([true, false, true], 2));

```
---
---
## Basic Data Structures: Combine Arrays with the Spread Operator
```js
/*We have defined a function spreadOut that returns the variable sentence, modify the function using the spread operator so that it returns the array ['learning', 'to', 'code', 'is', 'fun'].

spreadOut should return ["learning", "to", "code", "is", "fun"]
Passed
The spreadOut function should utilize spread syntax*/

function spreadOut() {
  let fragment = ['to', 'code'];
  let sentence = ["learning", ...fragment, "is", "fun"]; // change this line
  return sentence;
}

// do not change code below this line
console.log(spreadOut());
```

---
---
## Basic Data Structures: Check For The Presence of an Element With indexOf()
```js
/*indexOf() can be incredibly useful for quickly checking for the presence of an element on an array. We have defined a function, quickCheck, that takes an array and an element as arguments. Modify the function using indexOf() so that it returns true if the passed element exists on the array, and false if it does not.

quickCheck(["squash", "onions", "shallots"], "mushrooms") should return false
quickCheck(["squash", "onions", "shallots"], "onions") should return true
quickCheck([3, 5, 9, 125, 45, 2], 125) should return true
quickCheck([true, false, false], undefined) should return false
The quickCheck function should utilize the indexOf() method*/


function quickCheck(arr, elem) {
  // change code below this line
return arr.indexOf(elem)!==-1;
  // change code above this line
}

// change code here to test different cases:
console.log(quickCheck(['squash', 'onions', 'shallots'], 'mushrooms'));

```
---
---
## Basic Data Structures: Iterate Through All an Array's Items Using For Loops
```js
// SOLUTION

function filteredArray(arr, elem) {
  let newArr = [];
  // change code below this line
  
 for (let i = 0; i < arr.length; i++) { 
    if (arr[i].indexOf(elem)==-1){ //Checks every parameter for the element and if is NOT there continues the code
          newArr.push(arr[i]); //Inserts the element of the array in the new filtered array
            };
          };

  // change code above this line
  return newArr;
};
// change code here to test different cases:
console.log(filteredArray([[3, 2, 3], [1, 6, 3], [3, 13, 26], [19, 3, 9]], 3));
```
---
---
##
```js
```
---
---
##
```js
```
---
---
##
```js
```
---
---
##
```js
```
---
---
##
```js
```
---
---
##
```js
```
---
---
##
```js
```
---
---
##
```js
```
---
---
##
```js
```
---
---
##
```js
```
