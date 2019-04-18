## Exercises

### malformed while loop

broken code:
```js
let value = 0;
while (value < 9) 
  value++;
};
```
error message:
```
Uncaught SyntaxError: Unexpected token }
```
classification:
* creation phase
* syntax

the fix:
```js
let value = 0;
while (value < 9) {
  value++;
};
```
### missing variable name
broken code:
```js
var = 5;
```
error message:
```js
SyntaxError: Unexpected token =
```
classification:
* creation phase
* syntax 

the fix:
```js
var a = 5;

```
### access property directly
broken code:
```js
let x = {b:'e'};
let y = b.e;
```
error message:
ReferenceError: b is not defined
```
```
classification:
* execution phase 
* semanitc 

the fix:
```js
let x = {b:'e'};
let y = x.b;
```
### improper multi-line string
broken code:
```js
let a = 'this is 
two lines';
```
error message:
```
SyntaxError: Unexpected token ILLEGAL
```
classification:
* creation phase
* syntax

the fix:
```js
let a = 'this is two lines';
```
### improper end of statement
broken code:
```js
let a = 1:
```
error message:
```
SyntaxError: Unexpected token :
```
classification:
* creation phase
* syntax

the fix:
```js
1	let a = 1;

```
### malformed array
broken code:
```js
let myArray = [1, 2, 3;
```
error message:
```
SyntaxError: Unexpected token ;
```
classification:
* creation phase 
* syntax

the fix:
```js
let myArray = [1, 2, 3];

```
### missing arguments
broken code:
```js
function getNine {
  let x = 6;
  let y = 3;
  return x + y;
}
let result = getNine();
```
error message:
```
SyntaxError: Unexpected token {
```
classification:
* creation phase
* syntax

the fix:
```js
function getNine() {
  let x = 6;
  let y = 3;
  return x + y;
}
let result = getNine();
```
### improper nested quotes 1
broken code:
```js
let innerHtml = "<p>Click here to <a href="#Home">return home</a></p>";
```
error message:
```
SyntaxError: Unexpected token ILLEGAL
```
classification:
* creation phase 
* syntax

the fix:
```js
let innerHtml = "<p>Click here to <a href=\"#Home\">return home</a></p>";
```
### improper nested quotes 2 
broken code:
```js
let nested_messages = 'remind yourself ''i can do this!'' at least once a day';
```
error message:
```
SyntaxError: Unexpected string
```
classification:
* creation phas
* syntax 

the fix:
```js
let nested_messages = "remind yourself 'i can do this!' at least once a day";
```
### reassigning to constant
broken code:
```js
const a = 9;
a = 0;
```
error message:
```
TypeError: Assignment to constant variable.
```
classification:
* execution phase 
* semanitc 

the fix:
```js
const a = 9;
const b = 0;
```
### unassigned const declaration
broken code:
```js
const a;
a = 0;
```
error message:
```
SyntaxError: Missing initializer in const declaration
```
classification:
* creation phase 
* syntax 

the fix:
```js
const a = 0;
```
### is not a function
broken code:
```js
let array = [];
array.length()
```
error message:
```
TypeError: array.length is not a function
```
classification:
* execution phase 
* semanitc 

the fix:
```js
let array = [];
array.length
```
