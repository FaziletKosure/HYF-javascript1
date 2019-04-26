# Truthiness

Truthiness is very simple to understand.  Does a value convert to _true_ or _false_ when cast to boolean?

Paste this in the console to learn about truthiness, or study it [on python tutor](https://goo.gl/7tBTj3):
```js
{
  const x = ; // experiment with different values 
  const truthiness_x = Boolean(x);

  if (truthiness_x) {
    console.log("truthy: " + typeof x + ", " + x);
  } else {
    console.log("falsey: " + typeof x + ", " + x);
  };
};
```  
values to try:
```js
a: true       --> ?
a: false      --> ?
a: 0          --> ?
a: 1           --> ?
a: null       --> ?
a: undefined  --> ?
a: ''         --> ?
a: ' '        --> ?
a: 'tiil'     --> ?
a: 2          --> ?
a: 345        --> ?
a: NaN        --> ?
a: Infinity   --> ?
a: -Infinity  --> ?
a: -3         --> ?
a: -0.0       --> ?
```
* # My solution[on pytut](http://www.pythontutor.com/javascript.html#code=/*%0Aa%3A%20true%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%200%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%201%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20null%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20undefined%20%20--%3E%20%3F%0Aa%3A%20''%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'%20'%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'tiil'%20%20%20%20%20--%3E%20%3F%0Aa%3A%202%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20345%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20NaN%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20Infinity%20%20%20--%3E%20%3F%0Aa%3A%20-Infinity%20%20--%3E%20%3F%0Aa%3A%20-3%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20-0.0%20%20%20%20%20%20%20--%3E%20%3F%0A*/%0Aconst%20x%20%3D%20true%20%3B%20//%20experiment%20with%20different%20values%20%0Aconst%20truthiness_x%20%3D%20Boolean%28x%29%3B%0A%0Alet%20result%3B%0Aif%20%28truthiness_x%29%20%7B%0A%20%20result%20%3D%20%22truthy%3A%20%22%20%2B%20typeof%20x%20%2B%20%22,%20%22%20%2B%20x%3B%0A%7D%20else%20%7B%0A%20%20result%20%3D%20%22falsey%3A%20%22%20%2B%20typeof%20x%20%2B%20%22,%20%22%20%2B%20x%3B%0A%7D%3B&curInstr=5&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: true       --> ? *  true

const x = true ; // experiment with different values 
const truthiness_x = Boolean(x);

let result;
if (truthiness_x) {
  result = "truthy: " + typeof x + ", " + x;
} else {
  result = "falsey: " + typeof x + ", " + x;
};
// ---
* Global frame
x	true
truthiness_x	true
result	"truthy: boolean, true"
---
a: false      --> ? * false
const x = false ; // experiment with different values 
const truthiness_x = Boolean(x);

let result;
if (truthiness_x) {
  result = "truthy: " + typeof x + ", " + x;
} else {
  result = "falsey: " + typeof x + ", " + x;
  //
};
//---
* Global frame
x	false
truthiness_x	false
result	"falsey: boolean, false"

---
a: 0          --> ? * false

const x = 0 ; // experiment with different values 
const truthiness_x = Boolean(x);

let result;
if (truthiness_x) {
  result = "truthy: " + typeof x + ", " + x;
} else {
  result = "falsey: " + typeof x + ", " + x;
};

// ---
* Global frame
x	0
truthiness_x	false
result	"falsey: number, 0"


---

a: 1           --> ? * true
const x = 1 ; // experiment with different values 
const truthiness_x = Boolean(x);

let result;
if (truthiness_x) {
  result = "truthy: " + typeof x + ", " + x;
} else {
  result = "falsey: " + typeof x + ", " + x;
};
//---
* Global frame
x	1
truthiness_x	true
result	"truthy: number, 1"

---
a: null       --> ? * false
const x = null ; // experiment with different values 
const truthiness_x = Boolean(x);

let result;
if (truthiness_x) {
  result = "truthy: " + typeof x + ", " + x;
} else {
  result = "falsey: " + typeof x + ", " + x;
};
// ---
* Global frame
x	null
truthiness_x	false
result	"falsey: object, null"

---
a: undefined  --> ? * false

const x = undefined ; // experiment with different values 
const truthiness_x = Boolean(x);

let result;
if (truthiness_x) {
  result = "truthy: " + typeof x + ", " + x;
} else {
  result = "falsey: " + typeof x + ", " + x;
};
//---
* Global frame
x	undefined
truthiness_x	false
result	"falsey: undefined, undefined"
---
a: ''         --> ? * false
const x = '' ; // experiment with different values 
const truthiness_x = Boolean(x);

let result;
if (truthiness_x) {
  result = "truthy: " + typeof x + ", " + x;
} else {
  result = "falsey: " + typeof x + ", " + x;
};
//---
* Global frame
x	""
truthiness_x	false
result	"falsey: string, "

---
a: ' '        --> ? true

const x = ' ' ; // experiment with different values 
const truthiness_x = Boolean(x);

let result;
if (truthiness_x) {
  result = "truthy: " + typeof x + ", " + x;
} else {
  result = "falsey: " + typeof x + ", " + x;
};
//---
* Global frame
x	" "
truthiness_x	true
result	"truthy: string,  "


---
a: 'tiil'     --> ? * true
const x = 'tiil' ; // experiment with different values 
const truthiness_x = Boolean(x);

let result;
if (truthiness_x) {
  result = "truthy: " + typeof x + ", " + x;
} else {
  result = "falsey: " + typeof x + ", " + x;
};
//---
* Global frame
x	"tiil"
truthiness_x	true
result	"truthy: string, tiil"

---
a: 2          --> ? * true
const x = 2 ; // experiment with different values 
const truthiness_x = Boolean(x);

let result;
if (truthiness_x) {
  result = "truthy: " + typeof x + ", " + x;
} else {
  result = "falsey: " + typeof x + ", " + x;
};
//---
* Global frame
x	2
truthiness_x	true
result	"truthy: number, 2"

---
a: 345        --> ? * true
const x = 345 ; // experiment with different values 
const truthiness_x = Boolean(x);

let result;
if (truthiness_x) {
  result = "truthy: " + typeof x + ", " + x;
} else {
  result = "falsey: " + typeof x + ", " + x;
};
//---
* Global frame
x	345
truthiness_x	true
result	"truthy: number, 345"

---
a: NaN        --> ? * false
const x = NaN ; // experiment with different values 
const truthiness_x = Boolean(x);

let result;
if (truthiness_x) {
  result = "truthy: " + typeof x + ", " + x;
} else {
  result = "falsey: " + typeof x + ", " + x;
};
//---
* Global frame
x	NaN
truthiness_x	false
result	"falsey: number, NaN"

---
a: Infinity   --> ? * true
const x = Infinity ; // experiment with different values 
const truthiness_x = Boolean(x);

let result;
if (truthiness_x) {
  result = "truthy: " + typeof x + ", " + x;
} else {
  result = "falsey: " + typeof x + ", " + x;
};
//---
* Global frame
x	Infinity
truthiness_x	true
result	"truthy: number, Infinity"

---
a: -Infinity  --> ? * true
const x = -Infinity ; // experiment with different values 
const truthiness_x = Boolean(x);

let result;
if (truthiness_x) {
  result = "truthy: " + typeof x + ", " + x;
} else {
  result = "falsey: " + typeof x + ", " + x;
};
//---
* Global frame
x	-Infinity
truthiness_x	true
result	"truthy: number, -Infinity"
---
a: -3         --> ? * true
const x = -3 ; // experiment with different values 
const truthiness_x = Boolean(x);

let result;
if (truthiness_x) {
  result = "truthy: " + typeof x + ", " + x;
} else {
  result = "falsey: " + typeof x + ", " + x;
};
//---
* Global frame
x	-3
truthiness_x	true
result	"truthy: number, -3"

---
a: -0.0       --> ? * false
const x = true ; // experiment with different values 
const truthiness_x = Boolean(x);

let result;
if (truthiness_x) {
  result = "truthy: " + typeof x + ", " + x;
} else {
  result = "falsey: " + typeof x + ", " + x;
};
//---
* Global frame
x	0
truthiness_x	false
result	"falsey: number, 0"


```

This repo covers 4 important operators who's behavior is dependant on the _truthiness_ of their arguments.

### Index
* [falsey values](#falsey-values)
* [() ? : ;](#ternary-operator)
* [&&](#and-operator)
* [||](#or-operator)
* [!](#not-operator)
* [resources](#resources)


---
---

## Falsey Values

JavaScript has only 6 falsey primitive values.  All other values are truthy.

[on pytut](https://goo.gl/urDfWG)

```js
{
  const a = ;
  
  const truthiness = Boolean(a);
  
  console.log(typeof a + ", " + a + ", " + truthiness + "y");
};
```
the values:
```js
1: false      --> ?

2: null       --> ?

3: undefined  --> ?

4: ''         --> ?
4: ""         --> ?
4: ``         --> ?

5: NaN        --> ?

6: 0          --> ?
6: 0.0        --> ?
6: +0         --> ?
6: -0         --> ?
```


[TOP](#truthiness)

---

## Ternary Operator

The ternary operator evaluates the _truthiness_ of a value and returns either the first option or the second 

[pytut link](https://goo.gl/xK4GcW)

Paste this in the console to learn about the ternary operator:
```js
{ 
  const x = ; // experiment with different values 

  const coerce_truthiness = Boolean(x);
  const ternary_truthiness = (x) ? "truthy" : "falsey" ;
  
  const tern_option = (x) ? "first" : "second" ;
  const tern_numbers = (x) ? 1 : 2 ;
  const tern_boolean = (x) ? true : false ;

  console.log("x: " + typeof x + ", " + x);
  console.log("coerced: " + coerce_truthiness);
  console.log("ternaried: " + ternary_truthiness);
  console.log("option: " + tern_option);
  console.log("numbers: " + tern_numbers);
  console.log("booleans: " + tern_boolean);
};
```
Ternary operators can only have two options.  

### values to try:  a: true 
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=const%20x%20%3D%20true%20%3B%20//%20experiment%20with%20different%20values%20%0Aconst%20tern_value%20%3D%20%28x%29%20%3F%20%22truthy%22%20%3A%20%22falsey%22%20%3B%0A%0Aconst%20truthiness_x%20%3D%20Boolean%28x%29%3B%0A%0Aconst%20tern_truthiness%20%3D%20%28truthiness_x%29%20%3F%20%22truthy%22%20%3A%20%22falsey%22%20%3B%0Aconst%20tern_option%20%3D%20%28truthiness_x%29%20%3F%20%22first%22%20%3A%20%22second%22%20%3B%0Aconst%20tern_numbers%20%3D%20%28truthiness_x%29%20%3F%201%20%3A%202%20%3B%0A%20console.log%28%22x%3A%20%22%20%2B%20typeof%20x%20%2B%20%22,%20%22%20%2B%20x%29%3B%0A%20//%20console.log%28%22coerced%3A%20%22%20%2B%20coerce_truthiness%29%3B%0A%20%20//console.log%28%22ternaried%3A%20%22%20%2B%20ternary_truthiness%29%3B%0A%20%20console.log%28%22option%3A%20%22%20%2B%20tern_option%29%3B%0A%20%20console.log%28%22numbers%3A%20%22%20%2B%20tern_numbers%29%3B%0A%20%20console.log%28%22truthiness%3A%20%22%20%2B%20tern_truthiness%29%3B&curInstr=10&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: true       --> ?
const x = true ; // experiment with different values 
const tern_value = (x) ? "truthy" : "falsey" ;

const truthiness_x = Boolean(x);

const tern_truthiness = (truthiness_x) ? "truthy" : "falsey" ;
const tern_option = (truthiness_x) ? "first" : "second" ;
const tern_numbers = (truthiness_x) ? 1 : 2 ;
 console.log("x: " + typeof x + ", " + x);
 // console.log("coerced: " + coerce_truthiness);
  //console.log("ternaried: " + ternary_truthiness);
  console.log("option: " + tern_option);
  console.log("numbers: " + tern_numbers);
  console.log("truthiness: " + tern_truthiness);
//---
* Global frame
x	true
tern_value	"truthy"
truthiness_x	true
tern_truthiness	"truthy"
tern_option	"first"
tern_numbers	1


```
---
### values to try:  a: false
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=const%20x%20%3D%20false%20%3B%20//%20experiment%20with%20different%20values%20%0Aconst%20tern_value%20%3D%20%28x%29%20%3F%20%22truthy%22%20%3A%20%22falsey%22%20%3B%0A%0Aconst%20truthiness_x%20%3D%20Boolean%28x%29%3B%0A%0Aconst%20tern_truthiness%20%3D%20%28truthiness_x%29%20%3F%20%22truthy%22%20%3A%20%22falsey%22%20%3B%0Aconst%20tern_option%20%3D%20%28truthiness_x%29%20%3F%20%22first%22%20%3A%20%22second%22%20%3B%0Aconst%20tern_numbers%20%3D%20%28truthiness_x%29%20%3F%201%20%3A%202%20%3B%0A%20console.log%28%22x%3A%20%22%20%2B%20typeof%20x%20%2B%20%22,%20%22%20%2B%20x%29%3B%0A%20//%20console.log%28%22coerced%3A%20%22%20%2B%20coerce_truthiness%29%3B%0A%20%20//console.log%28%22ternaried%3A%20%22%20%2B%20ternary_truthiness%29%3B%0A%20%20console.log%28%22option%3A%20%22%20%2B%20tern_option%29%3B%0A%20%20console.log%28%22numbers%3A%20%22%20%2B%20tern_numbers%29%3B%0A%20%20console.log%28%22truthiness%3A%20%22%20%2B%20tern_truthiness%29%3B&curInstr=10&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: false      --> ?
const x = false ; // experiment with different values 
const tern_value = (x) ? "truthy" : "falsey" ;

const truthiness_x = Boolean(x);

const tern_truthiness = (truthiness_x) ? "truthy" : "falsey" ;
const tern_option = (truthiness_x) ? "first" : "second" ;
const tern_numbers = (truthiness_x) ? 1 : 2 ;
 console.log("x: " + typeof x + ", " + x);
 // console.log("coerced: " + coerce_truthiness);
  //console.log("ternaried: " + ternary_truthiness);
  console.log("option: " + tern_option);
  console.log("numbers: " + tern_numbers);
  console.log("truthiness: " + tern_truthiness);
 
```
---
### values to try:  a: 0 
* My solution [on pytut](ttp://www.pythontutor.com/javascript.html#code=const%20x%20%3D%200%20%3B%20//%20experiment%20with%20different%20values%20%0Aconst%20tern_value%20%3D%20%28x%29%20%3F%20%22truthy%22%20%3A%20%22falsey%22%20%3B%0A%0Aconst%20truthiness_x%20%3D%20Boolean%28x%29%3B%0A%0Aconst%20tern_truthiness%20%3D%20%28truthiness_x%29%20%3F%20%22truthy%22%20%3A%20%22falsey%22%20%3B%0Aconst%20tern_option%20%3D%20%28truthiness_x%29%20%3F%20%22first%22%20%3A%20%22second%22%20%3B%0Aconst%20tern_numbers%20%3D%20%28truthiness_x%29%20%3F%201%20%3A%202%20%3B%0A%20console.log%28%22x%3A%20%22%20%2B%20typeof%20x%20%2B%20%22,%20%22%20%2B%20x%29%3B%0A%20//%20console.log%28%22coerced%3A%20%22%20%2B%20coerce_truthiness%29%3B%0A%20%20//console.log%28%22ternaried%3A%20%22%20%2B%20ternary_truthiness%29%3B%0A%20%20console.log%28%22option%3A%20%22%20%2B%20tern_option%29%3B%0A%20%20console.log%28%22numbers%3A%20%22%20%2B%20tern_numbers%29%3B%0A%20%20console.log%28%22truthiness%3A%20%22%20%2B%20tern_truthiness%29%3B&curInstr=10&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: 0          --> ?
const x = 0 ; // experiment with different values 
const tern_value = (x) ? "truthy" : "falsey" ;

const truthiness_x = Boolean(x);

const tern_truthiness = (truthiness_x) ? "truthy" : "falsey" ;
const tern_option = (truthiness_x) ? "first" : "second" ;
const tern_numbers = (truthiness_x) ? 1 : 2 ;
 console.log("x: " + typeof x + ", " + x);
 // console.log("coerced: " + coerce_truthiness);
  //console.log("ternaried: " + ternary_truthiness);
  console.log("option: " + tern_option);
  console.log("numbers: " + tern_numbers);
  console.log("truthiness: " + tern_truthiness);

```
---
### values to try:  a: 1
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=const%20x%20%3D%201%20%3B%20//%20experiment%20with%20different%20values%20%0Aconst%20tern_value%20%3D%20%28x%29%20%3F%20%22truthy%22%20%3A%20%22falsey%22%20%3B%0A%0Aconst%20truthiness_x%20%3D%20Boolean%28x%29%3B%0A%0Aconst%20tern_truthiness%20%3D%20%28truthiness_x%29%20%3F%20%22truthy%22%20%3A%20%22falsey%22%20%3B%0Aconst%20tern_option%20%3D%20%28truthiness_x%29%20%3F%20%22first%22%20%3A%20%22second%22%20%3B%0Aconst%20tern_numbers%20%3D%20%28truthiness_x%29%20%3F%201%20%3A%202%20%3B%0A%20console.log%28%22x%3A%20%22%20%2B%20typeof%20x%20%2B%20%22,%20%22%20%2B%20x%29%3B%0A%20//%20console.log%28%22coerced%3A%20%22%20%2B%20coerce_truthiness%29%3B%0A%20%20//console.log%28%22ternaried%3A%20%22%20%2B%20ternary_truthiness%29%3B%0A%20%20console.log%28%22option%3A%20%22%20%2B%20tern_option%29%3B%0A%20%20console.log%28%22numbers%3A%20%22%20%2B%20tern_numbers%29%3B%0A%20%20console.log%28%22truthiness%3A%20%22%20%2B%20tern_truthiness%29%3B&curInstr=10&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: 1          --> ?
const x = 1 ; // experiment with different values 
const tern_value = (x) ? "truthy" : "falsey" ;

const truthiness_x = Boolean(x);

const tern_truthiness = (truthiness_x) ? "truthy" : "falsey" ;
const tern_option = (truthiness_x) ? "first" : "second" ;
const tern_numbers = (truthiness_x) ? 1 : 2 ;
 console.log("x: " + typeof x + ", " + x);
 // console.log("coerced: " + coerce_truthiness);
  //console.log("ternaried: " + ternary_truthiness);
  console.log("option: " + tern_option);
  console.log("numbers: " + tern_numbers);
  console.log("truthiness: " + tern_truthiness);
```
---
### values to try:  a: null
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=const%20x%20%3D%20null%20%3B%20//%20experiment%20with%20different%20values%20%0Aconst%20tern_value%20%3D%20%28x%29%20%3F%20%22truthy%22%20%3A%20%22falsey%22%20%3B%0A%0Aconst%20truthiness_x%20%3D%20Boolean%28x%29%3B%0A%0Aconst%20tern_truthiness%20%3D%20%28truthiness_x%29%20%3F%20%22truthy%22%20%3A%20%22falsey%22%20%3B%0Aconst%20tern_option%20%3D%20%28truthiness_x%29%20%3F%20%22first%22%20%3A%20%22second%22%20%3B%0Aconst%20tern_numbers%20%3D%20%28truthiness_x%29%20%3F%201%20%3A%202%20%3B%0A%20console.log%28%22x%3A%20%22%20%2B%20typeof%20x%20%2B%20%22,%20%22%20%2B%20x%29%3B%0A%20//%20console.log%28%22coerced%3A%20%22%20%2B%20coerce_truthiness%29%3B%0A%20%20//console.log%28%22ternaried%3A%20%22%20%2B%20ternary_truthiness%29%3B%0A%20%20console.log%28%22option%3A%20%22%20%2B%20tern_option%29%3B%0A%20%20console.log%28%22numbers%3A%20%22%20%2B%20tern_numbers%29%3B%0A%20%20console.log%28%22truthiness%3A%20%22%20%2B%20tern_truthiness%29%3B&curInstr=10&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: null       --> ? * FALSE

```
---
### values to try:  a: undefined
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=const%20x%20%3D%20undefined%20%3B%20//%20experiment%20with%20different%20values%20%0Aconst%20tern_value%20%3D%20%28x%29%20%3F%20%22truthy%22%20%3A%20%22falsey%22%20%3B%0A%0Aconst%20truthiness_x%20%3D%20Boolean%28x%29%3B%0A%0Aconst%20tern_truthiness%20%3D%20%28truthiness_x%29%20%3F%20%22truthy%22%20%3A%20%22falsey%22%20%3B%0Aconst%20tern_option%20%3D%20%28truthiness_x%29%20%3F%20%22first%22%20%3A%20%22second%22%20%3B%0Aconst%20tern_numbers%20%3D%20%28truthiness_x%29%20%3F%201%20%3A%202%20%3B%0A%20console.log%28%22x%3A%20%22%20%2B%20typeof%20x%20%2B%20%22,%20%22%20%2B%20x%29%3B%0A%20//%20console.log%28%22coerced%3A%20%22%20%2B%20coerce_truthiness%29%3B%0A%20%20//console.log%28%22ternaried%3A%20%22%20%2B%20ternary_truthiness%29%3B%0A%20%20console.log%28%22option%3A%20%22%20%2B%20tern_option%29%3B%0A%20%20console.log%28%22numbers%3A%20%22%20%2B%20tern_numbers%29%3B%0A%20%20console.log%28%22truthiness%3A%20%22%20%2B%20tern_truthiness%29%3B&curInstr=10&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: undefined  --> ? * FALSE

```
---
### values to try:  a: ''
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=const%20x%20%3D%20''%20%3B%20//%20experiment%20with%20different%20values%20%0Aconst%20tern_value%20%3D%20%28x%29%20%3F%20%22truthy%22%20%3A%20%22falsey%22%20%3B%0A%0Aconst%20truthiness_x%20%3D%20Boolean%28x%29%3B%0A%0Aconst%20tern_truthiness%20%3D%20%28truthiness_x%29%20%3F%20%22truthy%22%20%3A%20%22falsey%22%20%3B%0Aconst%20tern_option%20%3D%20%28truthiness_x%29%20%3F%20%22first%22%20%3A%20%22second%22%20%3B%0Aconst%20tern_numbers%20%3D%20%28truthiness_x%29%20%3F%201%20%3A%202%20%3B%0A%20console.log%28%22x%3A%20%22%20%2B%20typeof%20x%20%2B%20%22,%20%22%20%2B%20x%29%3B%0A%20//%20console.log%28%22coerced%3A%20%22%20%2B%20coerce_truthiness%29%3B%0A%20%20//console.log%28%22ternaried%3A%20%22%20%2B%20ternary_truthiness%29%3B%0A%20%20console.log%28%22option%3A%20%22%20%2B%20tern_option%29%3B%0A%20%20console.log%28%22numbers%3A%20%22%20%2B%20tern_numbers%29%3B%0A%20%20console.log%28%22truthiness%3A%20%22%20%2B%20tern_truthiness%29%3B&curInstr=10&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: ''         --> ? * FALSE
```
---
### values to try:  a: ' ' 
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=const%20x%20%3D%20'%20'%20%3B%20//%20experiment%20with%20different%20values%20%0Aconst%20tern_value%20%3D%20%28x%29%20%3F%20%22truthy%22%20%3A%20%22falsey%22%20%3B%0A%0Aconst%20truthiness_x%20%3D%20Boolean%28x%29%3B%0A%0Aconst%20tern_truthiness%20%3D%20%28truthiness_x%29%20%3F%20%22truthy%22%20%3A%20%22falsey%22%20%3B%0Aconst%20tern_option%20%3D%20%28truthiness_x%29%20%3F%20%22first%22%20%3A%20%22second%22%20%3B%0Aconst%20tern_numbers%20%3D%20%28truthiness_x%29%20%3F%201%20%3A%202%20%3B%0A%20console.log%28%22x%3A%20%22%20%2B%20typeof%20x%20%2B%20%22,%20%22%20%2B%20x%29%3B%0A%20//%20console.log%28%22coerced%3A%20%22%20%2B%20coerce_truthiness%29%3B%0A%20%20//console.log%28%22ternaried%3A%20%22%20%2B%20ternary_truthiness%29%3B%0A%20%20console.log%28%22option%3A%20%22%20%2B%20tern_option%29%3B%0A%20%20console.log%28%22numbers%3A%20%22%20%2B%20tern_numbers%29%3B%0A%20%20console.log%28%22truthiness%3A%20%22%20%2B%20tern_truthiness%29%3B&curInstr=10&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: ' '        --> ? * TRUE
```
---
### values to try:  a: 'tiil'
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=const%20x%20%3D%20'tiil'%20%3B%20//%20experiment%20with%20different%20values%20%0Aconst%20tern_value%20%3D%20%28x%29%20%3F%20%22truthy%22%20%3A%20%22falsey%22%20%3B%0A%0Aconst%20truthiness_x%20%3D%20Boolean%28x%29%3B%0A%0Aconst%20tern_truthiness%20%3D%20%28truthiness_x%29%20%3F%20%22truthy%22%20%3A%20%22falsey%22%20%3B%0Aconst%20tern_option%20%3D%20%28truthiness_x%29%20%3F%20%22first%22%20%3A%20%22second%22%20%3B%0Aconst%20tern_numbers%20%3D%20%28truthiness_x%29%20%3F%201%20%3A%202%20%3B%0A%20console.log%28%22x%3A%20%22%20%2B%20typeof%20x%20%2B%20%22,%20%22%20%2B%20x%29%3B%0A%20//%20console.log%28%22coerced%3A%20%22%20%2B%20coerce_truthiness%29%3B%0A%20%20//console.log%28%22ternaried%3A%20%22%20%2B%20ternary_truthiness%29%3B%0A%20%20console.log%28%22option%3A%20%22%20%2B%20tern_option%29%3B%0A%20%20console.log%28%22numbers%3A%20%22%20%2B%20tern_numbers%29%3B%0A%20%20console.log%28%22truthiness%3A%20%22%20%2B%20tern_truthiness%29%3B&curInstr=10&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: 'tiil'     --> ? * TRUE

```
---
### values to try:  a: 2
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=const%20x%20%3D%202%20%3B%20//%20experiment%20with%20different%20values%20%0Aconst%20tern_value%20%3D%20%28x%29%20%3F%20%22truthy%22%20%3A%20%22falsey%22%20%3B%0A%0Aconst%20truthiness_x%20%3D%20Boolean%28x%29%3B%0A%0Aconst%20tern_truthiness%20%3D%20%28truthiness_x%29%20%3F%20%22truthy%22%20%3A%20%22falsey%22%20%3B%0Aconst%20tern_option%20%3D%20%28truthiness_x%29%20%3F%20%22first%22%20%3A%20%22second%22%20%3B%0Aconst%20tern_numbers%20%3D%20%28truthiness_x%29%20%3F%201%20%3A%202%20%3B%0A%20console.log%28%22x%3A%20%22%20%2B%20typeof%20x%20%2B%20%22,%20%22%20%2B%20x%29%3B%0A%20//%20console.log%28%22coerced%3A%20%22%20%2B%20coerce_truthiness%29%3B%0A%20%20//console.log%28%22ternaried%3A%20%22%20%2B%20ternary_truthiness%29%3B%0A%20%20console.log%28%22option%3A%20%22%20%2B%20tern_option%29%3B%0A%20%20console.log%28%22numbers%3A%20%22%20%2B%20tern_numbers%29%3B%0A%20%20console.log%28%22truthiness%3A%20%22%20%2B%20tern_truthiness%29%3B&curInstr=10&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: 2          --> ? * TRUE

```
---
### values to try:  a: 345
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=const%20x%20%3D%20345%20%3B%20//%20experiment%20with%20different%20values%20%0Aconst%20tern_value%20%3D%20%28x%29%20%3F%20%22truthy%22%20%3A%20%22falsey%22%20%3B%0A%0Aconst%20truthiness_x%20%3D%20Boolean%28x%29%3B%0A%0Aconst%20tern_truthiness%20%3D%20%28truthiness_x%29%20%3F%20%22truthy%22%20%3A%20%22falsey%22%20%3B%0Aconst%20tern_option%20%3D%20%28truthiness_x%29%20%3F%20%22first%22%20%3A%20%22second%22%20%3B%0Aconst%20tern_numbers%20%3D%20%28truthiness_x%29%20%3F%201%20%3A%202%20%3B%0A%20console.log%28%22x%3A%20%22%20%2B%20typeof%20x%20%2B%20%22,%20%22%20%2B%20x%29%3B%0A%20//%20console.log%28%22coerced%3A%20%22%20%2B%20coerce_truthiness%29%3B%0A%20%20//console.log%28%22ternaried%3A%20%22%20%2B%20ternary_truthiness%29%3B%0A%20%20console.log%28%22option%3A%20%22%20%2B%20tern_option%29%3B%0A%20%20console.log%28%22numbers%3A%20%22%20%2B%20tern_numbers%29%3B%0A%20%20console.log%28%22truthiness%3A%20%22%20%2B%20tern_truthiness%29%3B&curInstr=10&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: 345        --> ? * TRUE

```
---
### values to try:  a: NaN
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=const%20x%20%3D%20NaN%20%3B%20//%20experiment%20with%20different%20values%20%0Aconst%20tern_value%20%3D%20%28x%29%20%3F%20%22truthy%22%20%3A%20%22falsey%22%20%3B%0A%0Aconst%20truthiness_x%20%3D%20Boolean%28x%29%3B%0A%0Aconst%20tern_truthiness%20%3D%20%28truthiness_x%29%20%3F%20%22truthy%22%20%3A%20%22falsey%22%20%3B%0Aconst%20tern_option%20%3D%20%28truthiness_x%29%20%3F%20%22first%22%20%3A%20%22second%22%20%3B%0Aconst%20tern_numbers%20%3D%20%28truthiness_x%29%20%3F%201%20%3A%202%20%3B%0A%20console.log%28%22x%3A%20%22%20%2B%20typeof%20x%20%2B%20%22,%20%22%20%2B%20x%29%3B%0A%20//%20console.log%28%22coerced%3A%20%22%20%2B%20coerce_truthiness%29%3B%0A%20%20//console.log%28%22ternaried%3A%20%22%20%2B%20ternary_truthiness%29%3B%0A%20%20console.log%28%22option%3A%20%22%20%2B%20tern_option%29%3B%0A%20%20console.log%28%22numbers%3A%20%22%20%2B%20tern_numbers%29%3B%0A%20%20console.log%28%22truthiness%3A%20%22%20%2B%20tern_truthiness%29%3B&curInstr=10&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: NaN        --> ? * FALSE

```
---
### values to try:  a: Infinity 
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=const%20x%20%3D%20Infinity%20%3B%20//%20experiment%20with%20different%20values%20%0Aconst%20tern_value%20%3D%20%28x%29%20%3F%20%22truthy%22%20%3A%20%22falsey%22%20%3B%0A%0Aconst%20truthiness_x%20%3D%20Boolean%28x%29%3B%0A%0Aconst%20tern_truthiness%20%3D%20%28truthiness_x%29%20%3F%20%22truthy%22%20%3A%20%22falsey%22%20%3B%0Aconst%20tern_option%20%3D%20%28truthiness_x%29%20%3F%20%22first%22%20%3A%20%22second%22%20%3B%0Aconst%20tern_numbers%20%3D%20%28truthiness_x%29%20%3F%201%20%3A%202%20%3B%0A%20console.log%28%22x%3A%20%22%20%2B%20typeof%20x%20%2B%20%22,%20%22%20%2B%20x%29%3B%0A%20//%20console.log%28%22coerced%3A%20%22%20%2B%20coerce_truthiness%29%3B%0A%20%20//console.log%28%22ternaried%3A%20%22%20%2B%20ternary_truthiness%29%3B%0A%20%20console.log%28%22option%3A%20%22%20%2B%20tern_option%29%3B%0A%20%20console.log%28%22numbers%3A%20%22%20%2B%20tern_numbers%29%3B%0A%20%20console.log%28%22truthiness%3A%20%22%20%2B%20tern_truthiness%29%3B&curInstr=10&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: Infinity   --> ? * TRUE

```
---
### values to try:  a: -Infinity
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=const%20x%20%3D%20-Infinity%20%3B%20//%20experiment%20with%20different%20values%20%0Aconst%20tern_value%20%3D%20%28x%29%20%3F%20%22truthy%22%20%3A%20%22falsey%22%20%3B%0A%0Aconst%20truthiness_x%20%3D%20Boolean%28x%29%3B%0A%0Aconst%20tern_truthiness%20%3D%20%28truthiness_x%29%20%3F%20%22truthy%22%20%3A%20%22falsey%22%20%3B%0Aconst%20tern_option%20%3D%20%28truthiness_x%29%20%3F%20%22first%22%20%3A%20%22second%22%20%3B%0Aconst%20tern_numbers%20%3D%20%28truthiness_x%29%20%3F%201%20%3A%202%20%3B%0A%20console.log%28%22x%3A%20%22%20%2B%20typeof%20x%20%2B%20%22,%20%22%20%2B%20x%29%3B%0A%20//%20console.log%28%22coerced%3A%20%22%20%2B%20coerce_truthiness%29%3B%0A%20%20//console.log%28%22ternaried%3A%20%22%20%2B%20ternary_truthiness%29%3B%0A%20%20console.log%28%22option%3A%20%22%20%2B%20tern_option%29%3B%0A%20%20console.log%28%22numbers%3A%20%22%20%2B%20tern_numbers%29%3B%0A%20%20console.log%28%22truthiness%3A%20%22%20%2B%20tern_truthiness%29%3B&curInstr=10&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: -Infinity  --> ? * TRUE

```
---
### values to try:  a: -3
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=const%20x%20%3D%20-3%20%3B%20//%20experiment%20with%20different%20values%20%0Aconst%20tern_value%20%3D%20%28x%29%20%3F%20%22truthy%22%20%3A%20%22falsey%22%20%3B%0A%0Aconst%20truthiness_x%20%3D%20Boolean%28x%29%3B%0A%0Aconst%20tern_truthiness%20%3D%20%28truthiness_x%29%20%3F%20%22truthy%22%20%3A%20%22falsey%22%20%3B%0Aconst%20tern_option%20%3D%20%28truthiness_x%29%20%3F%20%22first%22%20%3A%20%22second%22%20%3B%0Aconst%20tern_numbers%20%3D%20%28truthiness_x%29%20%3F%201%20%3A%202%20%3B%0A%20console.log%28%22x%3A%20%22%20%2B%20typeof%20x%20%2B%20%22,%20%22%20%2B%20x%29%3B%0A%20//%20console.log%28%22coerced%3A%20%22%20%2B%20coerce_truthiness%29%3B%0A%20%20//console.log%28%22ternaried%3A%20%22%20%2B%20ternary_truthiness%29%3B%0A%20%20console.log%28%22option%3A%20%22%20%2B%20tern_option%29%3B%0A%20%20console.log%28%22numbers%3A%20%22%20%2B%20tern_numbers%29%3B%0A%20%20console.log%28%22truthiness%3A%20%22%20%2B%20tern_truthiness%29%3B&curInstr=10&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: -3         --> ? * TRUE

```
---
### values to try:  a: -0.0
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=const%20x%20%3D%20-0.0%20%3B%20//%20experiment%20with%20different%20values%20%0Aconst%20tern_value%20%3D%20%28x%29%20%3F%20%22truthy%22%20%3A%20%22falsey%22%20%3B%0A%0Aconst%20truthiness_x%20%3D%20Boolean%28x%29%3B%0A%0Aconst%20tern_truthiness%20%3D%20%28truthiness_x%29%20%3F%20%22truthy%22%20%3A%20%22falsey%22%20%3B%0Aconst%20tern_option%20%3D%20%28truthiness_x%29%20%3F%20%22first%22%20%3A%20%22second%22%20%3B%0Aconst%20tern_numbers%20%3D%20%28truthiness_x%29%20%3F%201%20%3A%202%20%3B%0A%20console.log%28%22x%3A%20%22%20%2B%20typeof%20x%20%2B%20%22,%20%22%20%2B%20x%29%3B%0A%20//%20console.log%28%22coerced%3A%20%22%20%2B%20coerce_truthiness%29%3B%0A%20%20//console.log%28%22ternaried%3A%20%22%20%2B%20ternary_truthiness%29%3B%0A%20%20console.log%28%22option%3A%20%22%20%2B%20tern_option%29%3B%0A%20%20console.log%28%22numbers%3A%20%22%20%2B%20tern_numbers%29%3B%0A%20%20console.log%28%22truthiness%3A%20%22%20%2B%20tern_truthiness%29%3B&curInstr=10&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: -0.0       --> ? * FALSE
```


[TOP](#truthiness)

---

## And Operator

The and operator will return the first value if it's falsey, and the second value if the first is truthy.

[pytut link](https://goo.gl/G4mp9N)

Paste this in the console to learn about &&:
```js
{ 
  const a = ; // experiment with different values 
  const b = ; // experiment with different values 

  const and = a && b;
  const replication = (a) ? b : a ;
  
  console.log("a: "+typeof a+", "+a+", "+!!a+"y");
  console.log("b: "+typeof b+", "+b+", "+!!b+"y");
  
  console.log("and: " + and);
  console.log("replication: " + replication);
};
```
values to try:
```js
a: true, b:false      --> ?
a: false, b:true      --> ?
a: 0, b:1             --> ?
a: 1, b:0             --> ?
a: null, b:false      --> ?
a: false, b:null      --> ?
a: '', b:' '          --> ?
a: ' ', b:''          --> ?
a: 2, b:3             --> ?
a: 3, b:2             --> ?
```
---
### values to try:  a: true, b:false      
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=/*%0Aa%3A%20true,%20b%3Afalse%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false,%20b%3Atrue%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%200,%20b%3A1%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%201,%20b%3A0%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20null,%20b%3Afalse%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false,%20b%3Anull%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'',%20b%3A'%20'%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'%20',%20b%3A''%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%202,%20b%3A3%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%203,%20b%3A2%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0A*/%0A%0Aconst%20a%20%3D%20true%20%3B%20//%20experiment%20with%20different%20values%20%0Aconst%20b%20%3D%20false%3B%20//%20experiment%20with%20different%20values%20%0A%0Aconst%20a_truthiness%20%3D%20Boolean%28a%29%20%2B%20%22y%22%3B%0Aconst%20b_truthiness%20%3D%20Boolean%28b%29%20%2B%20%22y%22%3B%0A%0Aconst%20and%20%3D%20a%20%26%26%20b%3B%0Aconst%20replication%20%3D%20%28a%29%20%3F%20b%20%3A%20a%20%3B&curInstr=6&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: true, b:false      --> ? *FALSE
const a = true ; // experiment with different values 
const b = false; // experiment with different values 

const a_truthiness = Boolean(a) + "y";
const b_truthiness = Boolean(b) + "y";

const and = a && b;
const replication = (a) ? b : a ;

```
---
---
### values to try:  a: false, b:true      
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=/*%0Aa%3A%20true,%20b%3Afalse%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false,%20b%3Atrue%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%200,%20b%3A1%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%201,%20b%3A0%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20null,%20b%3Afalse%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false,%20b%3Anull%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'',%20b%3A'%20'%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'%20',%20b%3A''%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%202,%20b%3A3%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%203,%20b%3A2%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0A*/%0A%0Aconst%20a%20%3D%20false%20%3B%20//%20experiment%20with%20different%20values%20%0Aconst%20b%20%3D%20true%3B%20//%20experiment%20with%20different%20values%20%0A%0Aconst%20a_truthiness%20%3D%20Boolean%28a%29%20%2B%20%22y%22%3B%0Aconst%20b_truthiness%20%3D%20Boolean%28b%29%20%2B%20%22y%22%3B%0A%0Aconst%20and%20%3D%20a%20%26%26%20b%3B%0Aconst%20replication%20%3D%20%28a%29%20%3F%20b%20%3A%20a%20%3B&curInstr=6&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: false, b:true      --> ? * FALSE
const a = false ; // experiment with different values 
const b = true; // experiment with different values 

const a_truthiness = Boolean(a) + "y";
const b_truthiness = Boolean(b) + "y";

const and = a && b;
const replication = (a) ? b : a ;

```
---
---
### values to try:  a: 0, b:1             
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=/*%0Aa%3A%20true,%20b%3Afalse%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false,%20b%3Atrue%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%200,%20b%3A1%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%201,%20b%3A0%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20null,%20b%3Afalse%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false,%20b%3Anull%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'',%20b%3A'%20'%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'%20',%20b%3A''%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%202,%20b%3A3%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%203,%20b%3A2%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0A*/%0A%0Aconst%20a%20%3D%200%20%3B%20//%20experiment%20with%20different%20values%20%0Aconst%20b%20%3D%201%3B%20//%20experiment%20with%20different%20values%20%0A%0Aconst%20a_truthiness%20%3D%20Boolean%28a%29%20%2B%20%22y%22%3B%0Aconst%20b_truthiness%20%3D%20Boolean%28b%29%20%2B%20%22y%22%3B%0A%0Aconst%20and%20%3D%20a%20%26%26%20b%3B%0Aconst%20replication%20%3D%20%28a%29%20%3F%20b%20%3A%20a%20%3B&curInstr=6&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: 0, b:1             --> ? * 0
const a = 0 ; // experiment with different values 
const b = 1; // experiment with different values 

const a_truthiness = Boolean(a) + "y";
const b_truthiness = Boolean(b) + "y";

const and = a && b;
const replication = (a) ? b : a ;
```
---
---
### values to try:  a: 1, b:0             
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=/*%0Aa%3A%20true,%20b%3Afalse%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false,%20b%3Atrue%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%200,%20b%3A1%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%201,%20b%3A0%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20null,%20b%3Afalse%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false,%20b%3Anull%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'',%20b%3A'%20'%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'%20',%20b%3A''%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%202,%20b%3A3%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%203,%20b%3A2%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0A*/%0A%0Aconst%20a%20%3D%201%20%3B%20//%20experiment%20with%20different%20values%20%0Aconst%20b%20%3D%200%3B%20//%20experiment%20with%20different%20values%20%0A%0Aconst%20a_truthiness%20%3D%20Boolean%28a%29%20%2B%20%22y%22%3B%0Aconst%20b_truthiness%20%3D%20Boolean%28b%29%20%2B%20%22y%22%3B%0A%0Aconst%20and%20%3D%20a%20%26%26%20b%3B%0Aconst%20replication%20%3D%20%28a%29%20%3F%20b%20%3A%20a%20%3B&curInstr=6&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: 1, b:0             --> ? * 0
const a = 1 ; // experiment with different values 
const b = 0; // experiment with different values 

const a_truthiness = Boolean(a) + "y";
const b_truthiness = Boolean(b) + "y";

const and = a && b;
const replication = (a) ? b : a ;
```
---
---
### values to try:  a: null, b:false     
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=/*%0Aa%3A%20true,%20b%3Afalse%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false,%20b%3Atrue%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%200,%20b%3A1%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%201,%20b%3A0%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20null,%20b%3Afalse%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false,%20b%3Anull%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'',%20b%3A'%20'%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'%20',%20b%3A''%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%202,%20b%3A3%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%203,%20b%3A2%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0A*/%0A%0Aconst%20a%20%3D%20null%20%3B%20//%20experiment%20with%20different%20values%20%0Aconst%20b%20%3D%20false%3B%20//%20experiment%20with%20different%20values%20%0A%0Aconst%20a_truthiness%20%3D%20Boolean%28a%29%20%2B%20%22y%22%3B%0Aconst%20b_truthiness%20%3D%20Boolean%28b%29%20%2B%20%22y%22%3B%0A%0Aconst%20and%20%3D%20a%20%26%26%20b%3B%0Aconst%20replication%20%3D%20%28a%29%20%3F%20b%20%3A%20a%20%3B&curInstr=6&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: null, b:false      --> ? * null
const a = null ; // experiment with different values 
const b = false; // experiment with different values 

const a_truthiness = Boolean(a) + "y";
const b_truthiness = Boolean(b) + "y";

const and = a && b;
const replication = (a) ? b : a ;
```
---
---
### values to try:  a: false, b:null      
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=/*%0Aa%3A%20true,%20b%3Afalse%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false,%20b%3Atrue%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%200,%20b%3A1%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%201,%20b%3A0%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20null,%20b%3Afalse%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false,%20b%3Anull%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'',%20b%3A'%20'%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'%20',%20b%3A''%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%202,%20b%3A3%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%203,%20b%3A2%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0A*/%0A%0Aconst%20a%20%3D%20false%20%3B%20//%20experiment%20with%20different%20values%20%0Aconst%20b%20%3D%20null%3B%20//%20experiment%20with%20different%20values%20%0A%0Aconst%20a_truthiness%20%3D%20Boolean%28a%29%20%2B%20%22y%22%3B%0Aconst%20b_truthiness%20%3D%20Boolean%28b%29%20%2B%20%22y%22%3B%0A%0Aconst%20and%20%3D%20a%20%26%26%20b%3B%0Aconst%20replication%20%3D%20%28a%29%20%3F%20b%20%3A%20a%20%3B&curInstr=6&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: false, b:null      --> ? * false
const a = false ; // experiment with different values 
const b = null; // experiment with different values 

const a_truthiness = Boolean(a) + "y";
const b_truthiness = Boolean(b) + "y";

const and = a && b;
const replication = (a) ? b : a ;
```
---
---
### values to try:  a: '', b:' '          
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=/*%0Aa%3A%20true,%20b%3Afalse%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false,%20b%3Atrue%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%200,%20b%3A1%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%201,%20b%3A0%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20null,%20b%3Afalse%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false,%20b%3Anull%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'',%20b%3A'%20'%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'%20',%20b%3A''%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%202,%20b%3A3%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%203,%20b%3A2%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0A*/%0A%0Aconst%20a%20%3D%20''%20%3B%20//%20experiment%20with%20different%20values%20%0Aconst%20b%20%3D%20'%20'%3B%20//%20experiment%20with%20different%20values%20%0A%0Aconst%20a_truthiness%20%3D%20Boolean%28a%29%20%2B%20%22y%22%3B%0Aconst%20b_truthiness%20%3D%20Boolean%28b%29%20%2B%20%22y%22%3B%0A%0Aconst%20and%20%3D%20a%20%26%26%20b%3B%0Aconst%20replication%20%3D%20%28a%29%20%3F%20b%20%3A%20a%20%3B&curInstr=6&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: '', b:' '          --> ? * ''
const a = '' ; // experiment with different values 
const b = ' '; // experiment with different values 

const a_truthiness = Boolean(a) + "y";
const b_truthiness = Boolean(b) + "y";

const and = a && b;
const replication = (a) ? b : a ;
```
---
---
### values to try:  a: ' ', b:''          
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=/*%0Aa%3A%20true,%20b%3Afalse%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false,%20b%3Atrue%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%200,%20b%3A1%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%201,%20b%3A0%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20null,%20b%3Afalse%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false,%20b%3Anull%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'',%20b%3A'%20'%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'%20',%20b%3A''%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%202,%20b%3A3%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%203,%20b%3A2%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0A*/%0A%0Aconst%20a%20%3D%20'%20'%20%3B%20//%20experiment%20with%20different%20values%20%0Aconst%20b%20%3D%20''%3B%20//%20experiment%20with%20different%20values%20%0A%0Aconst%20a_truthiness%20%3D%20Boolean%28a%29%20%2B%20%22y%22%3B%0Aconst%20b_truthiness%20%3D%20Boolean%28b%29%20%2B%20%22y%22%3B%0A%0Aconst%20and%20%3D%20a%20%26%26%20b%3B%0Aconst%20replication%20%3D%20%28a%29%20%3F%20b%20%3A%20a%20%3B&curInstr=6&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: ' ', b:''          --> ? * ''
const a = ' ' ; // experiment with different values 
const b = ''; // experiment with different values 

const a_truthiness = Boolean(a) + "y";
const b_truthiness = Boolean(b) + "y";

const and = a && b;
const replication = (a) ? b : a ;
```
---

---
### values to try:  a: 2, b:3             
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=/*%0Aa%3A%20true,%20b%3Afalse%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false,%20b%3Atrue%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%200,%20b%3A1%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%201,%20b%3A0%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20null,%20b%3Afalse%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false,%20b%3Anull%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'',%20b%3A'%20'%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'%20',%20b%3A''%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%202,%20b%3A3%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%203,%20b%3A2%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0A*/%0A%0Aconst%20a%20%3D%202%20%3B%20//%20experiment%20with%20different%20values%20%0Aconst%20b%20%3D%203%3B%20//%20experiment%20with%20different%20values%20%0A%0Aconst%20a_truthiness%20%3D%20Boolean%28a%29%20%2B%20%22y%22%3B%0Aconst%20b_truthiness%20%3D%20Boolean%28b%29%20%2B%20%22y%22%3B%0A%0Aconst%20and%20%3D%20a%20%26%26%20b%3B%0Aconst%20replication%20%3D%20%28a%29%20%3F%20b%20%3A%20a%20%3B&curInstr=6&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: 2, b:3             --> ? * 3
const a = 2 ; // experiment with different values 
const b = 3; // experiment with different values 

const a_truthiness = Boolean(a) + "y";
const b_truthiness = Boolean(b) + "y";

const and = a && b;
const replication = (a) ? b : a ;
```
---
---
### values to try:  a: 3, b:2             
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=/*%0Aa%3A%20true,%20b%3Afalse%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false,%20b%3Atrue%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%200,%20b%3A1%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%201,%20b%3A0%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20null,%20b%3Afalse%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false,%20b%3Anull%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'',%20b%3A'%20'%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'%20',%20b%3A''%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%202,%20b%3A3%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%203,%20b%3A2%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0A*/%0A%0Aconst%20a%20%3D%203%20%3B%20//%20experiment%20with%20different%20values%20%0Aconst%20b%20%3D%202%3B%20//%20experiment%20with%20different%20values%20%0A%0Aconst%20a_truthiness%20%3D%20Boolean%28a%29%20%2B%20%22y%22%3B%0Aconst%20b_truthiness%20%3D%20Boolean%28b%29%20%2B%20%22y%22%3B%0A%0Aconst%20and%20%3D%20a%20%26%26%20b%3B%0Aconst%20replication%20%3D%20%28a%29%20%3F%20b%20%3A%20a%20%3B&curInstr=6&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: 3, b:2             --> ? * 2
const a = 3 ; // experiment with different values 
const b = 2; // experiment with different values 

const a_truthiness = Boolean(a) + "y";
const b_truthiness = Boolean(b) + "y";

const and = a && b;
const replication = (a) ? b : a ;
```
---
[TOP](#truthiness)

---

## Or Operator

The or operator will return the first value if it's truthy, and the second value if the first is falsey.

[pytut link](https://goo.gl/gEztXo)

Paste this in the console to learn about ||:
```js
{ 
  const a = ; // experiment with different values 
  const b = ; // experiment with different values 

  const or = a || b;
  const replication = (a) ? a : b ;
  
  console.log("a: "+typeof a+", "+a+", "+!!a+"y");
  console.log("b: "+typeof b+", "+b+", "+!!b+"y");
  
  console.log("or: " + or);
  console.log("replication: " + replication);
};
```
values to try:
```js
a: true, b:false      --> ?
a: false, b:true      --> ?
a: 0, b:1             --> ?
a: 1, b:0             --> ?
a: null, b:false      --> ?
a: false, b:null      --> ?
a: '', b:' '          --> ?
a: ' ', b:''          --> ?
a: 2, b:3             --> ?
a: 3, b:2             --> ?
```
---
### values to try:  a: true, b:false      
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=/*%0Aa%3A%20true,%20b%3Afalse%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false,%20b%3Atrue%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%200,%20b%3A1%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%201,%20b%3A0%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20null,%20b%3Afalse%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false,%20b%3Anull%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'',%20b%3A'%20'%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'%20',%20b%3A''%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%202,%20b%3A3%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%203,%20b%3A2%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0A*/%0A%0Aconst%20a%20%3D%20true%3B%20//%20experiment%20with%20different%20values%20%0Aconst%20b%20%3D%20false%3B%20//%20experiment%20with%20different%20values%20%0A%0Aconst%20a_truthiness%20%3D%20Boolean%28a%29%20%2B%20%22y%22%3B%0Aconst%20b_truthiness%20%3D%20Boolean%28b%29%20%2B%20%22y%22%3B%0A%0Aconst%20and%20%3D%20a%20%7C%7C%20b%3B%0Aconst%20replication%20%3D%20%28a%29%20%3F%20a%20%3A%20b%20%3B&curInstr=6&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: true, b:false      --> ? *TRUE
const a = true ; // experiment with different values 
  const b = false ; // experiment with different values 

  const or = a || b;
  const replication = (a) ? a : b ;
  
  console.log("a: "+typeof a+", "+a+", "+!!a+"y");
  console.log("b: "+typeof b+", "+b+", "+!!b+"y");
  
  console.log("or: " + or);
  console.log("replication: " + replication);

```
---
---
### values to try:  a: false, b:true      
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=/*%0Aa%3A%20true,%20b%3Afalse%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false,%20b%3Atrue%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%200,%20b%3A1%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%201,%20b%3A0%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20null,%20b%3Afalse%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false,%20b%3Anull%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'',%20b%3A'%20'%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'%20',%20b%3A''%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%202,%20b%3A3%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%203,%20b%3A2%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0A*/%0A%0Aconst%20a%20%3D%20false%3B%20//%20experiment%20with%20different%20values%20%0Aconst%20b%20%3D%20true%3B%20//%20experiment%20with%20different%20values%20%0A%0Aconst%20a_truthiness%20%3D%20Boolean%28a%29%20%2B%20%22y%22%3B%0Aconst%20b_truthiness%20%3D%20Boolean%28b%29%20%2B%20%22y%22%3B%0A%0Aconst%20and%20%3D%20a%20%7C%7C%20b%3B%0Aconst%20replication%20%3D%20%28a%29%20%3F%20a%20%3A%20b%20%3B&curInstr=6&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: false, b:true      --> ? * TRUE

const a = false ; // experiment with different values 
  const b = true ; // experiment with different values 

  const or = a || b;
  const replication = (a) ? a : b ;
  
  console.log("a: "+typeof a+", "+a+", "+!!a+"y");
  console.log("b: "+typeof b+", "+b+", "+!!b+"y");
  
  console.log("or: " + or);
  console.log("replication: " + replication);
```
---
---
### values to try:  a: 0, b:1             
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=/*%0Aa%3A%20true,%20b%3Afalse%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false,%20b%3Atrue%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%200,%20b%3A1%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%201,%20b%3A0%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20null,%20b%3Afalse%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false,%20b%3Anull%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'',%20b%3A'%20'%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'%20',%20b%3A''%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%202,%20b%3A3%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%203,%20b%3A2%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0A*/%0A%0Aconst%20a%20%3D%200%3B%20//%20experiment%20with%20different%20values%20%0Aconst%20b%20%3D%201%3B%20//%20experiment%20with%20different%20values%20%0A%0Aconst%20a_truthiness%20%3D%20Boolean%28a%29%20%2B%20%22y%22%3B%0Aconst%20b_truthiness%20%3D%20Boolean%28b%29%20%2B%20%22y%22%3B%0A%0Aconst%20and%20%3D%20a%20%7C%7C%20b%3B%0Aconst%20replication%20%3D%20%28a%29%20%3F%20a%20%3A%20b%20%3B&curInstr=6&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: 0, b:1             --> ? * 1
const a = 0; // experiment with different values 
  const b = 1 ; // experiment with different values 

  const or = a || b;
  const replication = (a) ? a : b ;
  
  console.log("a: "+typeof a+", "+a+", "+!!a+"y");
  console.log("b: "+typeof b+", "+b+", "+!!b+"y");
  
  console.log("or: " + or);
  console.log("replication: " + replication);
```
---
---
### values to try:  a: 1, b:0             
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=/*%0Aa%3A%20true,%20b%3Afalse%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false,%20b%3Atrue%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%200,%20b%3A1%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%201,%20b%3A0%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20null,%20b%3Afalse%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false,%20b%3Anull%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'',%20b%3A'%20'%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'%20',%20b%3A''%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%202,%20b%3A3%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%203,%20b%3A2%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0A*/%0A%0Aconst%20a%20%3D%201%3B%20//%20experiment%20with%20different%20values%20%0Aconst%20b%20%3D%200%3B%20//%20experiment%20with%20different%20values%20%0A%0Aconst%20a_truthiness%20%3D%20Boolean%28a%29%20%2B%20%22y%22%3B%0Aconst%20b_truthiness%20%3D%20Boolean%28b%29%20%2B%20%22y%22%3B%0A%0Aconst%20and%20%3D%20a%20%7C%7C%20b%3B%0Aconst%20replication%20%3D%20%28a%29%20%3F%20a%20%3A%20b%20%3B&curInstr=6&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: 1, b:0             --> ? * 1
const a = 1 ; // experiment with different values 
  const b = 0 ; // experiment with different values 

  const or = a || b;
  const replication = (a) ? a : b ;
  
  console.log("a: "+typeof a+", "+a+", "+!!a+"y");
  console.log("b: "+typeof b+", "+b+", "+!!b+"y");
  
  console.log("or: " + or);
  console.log("replication: " + replication);
```
---
---
### values to try:  a: null, b:false     
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=/*%0Aa%3A%20true,%20b%3Afalse%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false,%20b%3Atrue%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%200,%20b%3A1%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%201,%20b%3A0%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20null,%20b%3Afalse%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false,%20b%3Anull%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'',%20b%3A'%20'%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'%20',%20b%3A''%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%202,%20b%3A3%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%203,%20b%3A2%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0A*/%0A%0Aconst%20a%20%3D%20null%3B%20//%20experiment%20with%20different%20values%20%0Aconst%20b%20%3D%20false%3B%20//%20experiment%20with%20different%20values%20%0A%0Aconst%20a_truthiness%20%3D%20Boolean%28a%29%20%2B%20%22y%22%3B%0Aconst%20b_truthiness%20%3D%20Boolean%28b%29%20%2B%20%22y%22%3B%0A%0Aconst%20and%20%3D%20a%20%7C%7C%20b%3B%0Aconst%20replication%20%3D%20%28a%29%20%3F%20a%20%3A%20b%20%3B&curInstr=6&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: null, b:false      --> ? * FALSE
const a = null ; // experiment with different values 
  const b = false; // experiment with different values 

  const or = a || b;
  const replication = (a) ? a : b ;
  
  console.log("a: "+typeof a+", "+a+", "+!!a+"y");
  console.log("b: "+typeof b+", "+b+", "+!!b+"y");
  
  console.log("or: " + or);
  console.log("replication: " + replication);
```
---
---
### values to try:  a: false, b:null      
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=/*%0Aa%3A%20true,%20b%3Afalse%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false,%20b%3Atrue%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%200,%20b%3A1%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%201,%20b%3A0%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20null,%20b%3Afalse%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false,%20b%3Anull%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'',%20b%3A'%20'%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'%20',%20b%3A''%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%202,%20b%3A3%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%203,%20b%3A2%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0A*/%0A%0Aconst%20a%20%3D%20false%3B%20//%20experiment%20with%20different%20values%20%0Aconst%20b%20%3D%20null%3B%20//%20experiment%20with%20different%20values%20%0A%0Aconst%20a_truthiness%20%3D%20Boolean%28a%29%20%2B%20%22y%22%3B%0Aconst%20b_truthiness%20%3D%20Boolean%28b%29%20%2B%20%22y%22%3B%0A%0Aconst%20and%20%3D%20a%20%7C%7C%20b%3B%0Aconst%20replication%20%3D%20%28a%29%20%3F%20a%20%3A%20b%20%3B&curInstr=6&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: false, b:null      --> ? * Null
const a = false; // experiment with different values 
  const b = null ; // experiment with different values 

  const or = a || b;
  const replication = (a) ? a : b ;
  
  console.log("a: "+typeof a+", "+a+", "+!!a+"y");
  console.log("b: "+typeof b+", "+b+", "+!!b+"y");
  
  console.log("or: " + or);
  console.log("replication: " + replication);
```
---
---
### values to try:  a: '', b:' '          
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=/*%0Aa%3A%20true,%20b%3Afalse%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false,%20b%3Atrue%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%200,%20b%3A1%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%201,%20b%3A0%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20null,%20b%3Afalse%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false,%20b%3Anull%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'',%20b%3A'%20'%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'%20',%20b%3A''%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%202,%20b%3A3%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%203,%20b%3A2%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0A*/%0A%0Aconst%20a%20%3D%20''%3B%20//%20experiment%20with%20different%20values%20%0Aconst%20b%20%3D%20'%20'%3B%20//%20experiment%20with%20different%20values%20%0A%0Aconst%20a_truthiness%20%3D%20Boolean%28a%29%20%2B%20%22y%22%3B%0Aconst%20b_truthiness%20%3D%20Boolean%28b%29%20%2B%20%22y%22%3B%0A%0Aconst%20and%20%3D%20a%20%7C%7C%20b%3B%0Aconst%20replication%20%3D%20%28a%29%20%3F%20a%20%3A%20b%20%3B&curInstr=6&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: '', b:' '          --> ? * ' '
const a = ''; // experiment with different values 
  const b = ' '; // experiment with different values 

  const or = a || b;
  const replication = (a) ? a : b ;
  
  console.log("a: "+typeof a+", "+a+", "+!!a+"y");
  console.log("b: "+typeof b+", "+b+", "+!!b+"y");
  
  console.log("or: " + or);
  console.log("replication: " + replication);
```
---
---
### values to try:  a: ' ', b:''          
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=/*%0Aa%3A%20true,%20b%3Afalse%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false,%20b%3Atrue%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%200,%20b%3A1%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%201,%20b%3A0%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20null,%20b%3Afalse%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false,%20b%3Anull%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'',%20b%3A'%20'%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'%20',%20b%3A''%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%202,%20b%3A3%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%203,%20b%3A2%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0A*/%0A%0Aconst%20a%20%3D%20'%20'%3B%20//%20experiment%20with%20different%20values%20%0Aconst%20b%20%3D%20''%3B%20//%20experiment%20with%20different%20values%20%0A%0Aconst%20a_truthiness%20%3D%20Boolean%28a%29%20%2B%20%22y%22%3B%0Aconst%20b_truthiness%20%3D%20Boolean%28b%29%20%2B%20%22y%22%3B%0A%0Aconst%20and%20%3D%20a%20%7C%7C%20b%3B%0Aconst%20replication%20%3D%20%28a%29%20%3F%20a%20%3A%20b%20%3B&curInstr=6&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: ' ', b:''          --> ? * ' '
const a = ' '; // experiment with different values 
  const b = ''; // experiment with different values 

  const or = a || b;
  const replication = (a) ? a : b ;
  
  console.log("a: "+typeof a+", "+a+", "+!!a+"y");
  console.log("b: "+typeof b+", "+b+", "+!!b+"y");
  
  console.log("or: " + or);
  console.log("replication: " + replication);
```
---

---
### values to try:  a: 2, b:3             
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=/*%0Aa%3A%20true,%20b%3Afalse%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false,%20b%3Atrue%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%200,%20b%3A1%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%201,%20b%3A0%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20null,%20b%3Afalse%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false,%20b%3Anull%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'',%20b%3A'%20'%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'%20',%20b%3A''%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%202,%20b%3A3%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%203,%20b%3A2%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0A*/%0A%0Aconst%20a%20%3D%202%3B%20//%20experiment%20with%20different%20values%20%0Aconst%20b%20%3D%203%3B%20//%20experiment%20with%20different%20values%20%0A%0Aconst%20a_truthiness%20%3D%20Boolean%28a%29%20%2B%20%22y%22%3B%0Aconst%20b_truthiness%20%3D%20Boolean%28b%29%20%2B%20%22y%22%3B%0A%0Aconst%20and%20%3D%20a%20%7C%7C%20b%3B%0Aconst%20replication%20%3D%20%28a%29%20%3F%20a%20%3A%20b%20%3B&curInstr=6&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: 2, b:3             --> ? * 2
const a = 2; // experiment with different values 
  const b =3 ; // experiment with different values 

  const or = a || b;
  const replication = (a) ? a : b ;
  
  console.log("a: "+typeof a+", "+a+", "+!!a+"y");
  console.log("b: "+typeof b+", "+b+", "+!!b+"y");
  
  console.log("or: " + or);
  console.log("replication: " + replication);
```
---
---
### values to try:  a: 3, b:2             
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=/*%0Aa%3A%20true,%20b%3Afalse%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false,%20b%3Atrue%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%200,%20b%3A1%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%201,%20b%3A0%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20null,%20b%3Afalse%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false,%20b%3Anull%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'',%20b%3A'%20'%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'%20',%20b%3A''%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%202,%20b%3A3%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%203,%20b%3A2%20%20%20%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0A*/%0A%0Aconst%20a%20%3D%203%3B%20//%20experiment%20with%20different%20values%20%0Aconst%20b%20%3D%202%3B%20//%20experiment%20with%20different%20values%20%0A%0Aconst%20a_truthiness%20%3D%20Boolean%28a%29%20%2B%20%22y%22%3B%0Aconst%20b_truthiness%20%3D%20Boolean%28b%29%20%2B%20%22y%22%3B%0A%0Aconst%20and%20%3D%20a%20%7C%7C%20b%3B%0Aconst%20replication%20%3D%20%28a%29%20%3F%20a%20%3A%20b%20%3B&curInstr=6&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: 3, b:2             --> ? * 3
const a = 3; // experiment with different values 
  const b = 2; // experiment with different values 

  const or = a || b;
  const replication = (a) ? a : b ;
  
  console.log("a: "+typeof a+", "+a+", "+!!a+"y");
  console.log("b: "+typeof b+", "+b+", "+!!b+"y");
  
  console.log("or: " + or);
  console.log("replication: " + replication);
```
---
[TOP](#truthiness)

---

## Not Operator

The or operator will return the first value if it's truthy, and the second value if the first is falsey.

pytut links: [the snippet below](https://goo.gl/abjq1R), [! expanded](https://goo.gl/ej3y5j)  

Paste this in the console to learn about !:
```js
{ 
  const a = ; // experiment with different values 

  const not = !a;
  const coercion_replication = !Boolean(a);
  const ternary_replication = (a) ? false : true ;

  console.log("a: "+typeof a+", "+a+", "+!!a+"y");
  console.log("not operator: " + not);
  console.log("with coercion: " + coercion_replication);  
  console.log("with ternary: " + ternary_replication);  
};
```  
values to try:
```js
a: true       --> ?
a: false      --> ?
a: 0          --> ?
a: 1          --> ?
a: null       --> ?
a: undefined  --> ?
a: ''         --> ?
a: ' '        --> ?
a: 'tiil'     --> ?
a: 2          --> ?
a: 345        --> ?
a: NaN        --> ?
a: Infinity   --> ?
a: -Infinity  --> ?
a: -3         --> ?
a: -0.0       --> ?
```
---
---
### values to try:  a: true 
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=/*%0Aa%3A%20true%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%200%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%201%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20null%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20undefined%20%20--%3E%20%3F%0Aa%3A%20''%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'%20'%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'tiil'%20%20%20%20%20--%3E%20%3F%0Aa%3A%202%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20345%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20NaN%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20Infinity%20%20%20--%3E%20%3F%0Aa%3A%20-Infinity%20%20--%3E%20%3F%0Aa%3A%20-3%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20-0.0%20%20%20%20%20%20%20--%3E%20%3F%0A*/%0A%0A%0Aconst%20a%20%3D%20true%20%3B%20//%20experiment%20with%20different%20values%20%0A%0Aconst%20truthiness%20%3D%20Boolean%28a%29%20%2B%20%22y%22%3B%0A%0Aconst%20not%20%3D%20!a%3B%0Aconst%20coercion_replication%20%3D%20!Boolean%28a%29%3B%0Aconst%20ternary_replication%20%3D%20%28a%29%20%3F%20false%20%3A%20true%20%3B&curInstr=5&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: true       --> ? * false

const a = true ; // experiment with different values 

const truthiness = Boolean(a) + "y";

const not = !a;
const coercion_replication = !Boolean(a);
const ternary_replication = (a) ? false : true ;
```
---
---
### values to try:  a: false
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=/*%0Aa%3A%20true%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%200%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%201%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20null%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20undefined%20%20--%3E%20%3F%0Aa%3A%20''%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'%20'%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'tiil'%20%20%20%20%20--%3E%20%3F%0Aa%3A%202%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20345%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20NaN%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20Infinity%20%20%20--%3E%20%3F%0Aa%3A%20-Infinity%20%20--%3E%20%3F%0Aa%3A%20-3%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20-0.0%20%20%20%20%20%20%20--%3E%20%3F%0A*/%0A%0A%0Aconst%20a%20%3D%20false%20%3B%20//%20experiment%20with%20different%20values%20%0A%0Aconst%20truthiness%20%3D%20Boolean%28a%29%20%2B%20%22y%22%3B%0A%0Aconst%20not%20%3D%20!a%3B%0Aconst%20coercion_replication%20%3D%20!Boolean%28a%29%3B%0Aconst%20ternary_replication%20%3D%20%28a%29%20%3F%20false%20%3A%20true%20%3B&curInstr=5&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: false      --> ? * true

 const a = false ; // experiment with different values 

const truthiness = Boolean(a) + "y";

const not = !a;
const coercion_replication = !Boolean(a);
const ternary_replication = (a) ? false : true ;
```
---
---
### values to try:  a: 0 
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=/*%0Aa%3A%20true%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%200%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%201%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20null%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20undefined%20%20--%3E%20%3F%0Aa%3A%20''%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'%20'%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'tiil'%20%20%20%20%20--%3E%20%3F%0Aa%3A%202%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20345%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20NaN%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20Infinity%20%20%20--%3E%20%3F%0Aa%3A%20-Infinity%20%20--%3E%20%3F%0Aa%3A%20-3%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20-0.0%20%20%20%20%20%20%20--%3E%20%3F%0A*/%0A%0A%0Aconst%20a%20%3D%20false%20%3B%20//%20experiment%20with%20different%20values%20%0A%0Aconst%20truthiness%20%3D%20Boolean%28a%29%20%2B%20%22y%22%3B%0A%0Aconst%20not%20%3D%20!a%3B%0Aconst%20coercion_replication%20%3D%20!Boolean%28a%29%3B%0Aconst%20ternary_replication%20%3D%20%28a%29%20%3F%20false%20%3A%20true%20%3B&curInstr=5&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: 0          --> ? * true
const a = 0 ; // experiment with different values 

const truthiness = Boolean(a) + "y";

const not = !a;
const coercion_replication = !Boolean(a);
const ternary_replication = (a) ? false : true ;

```
---
---
### values to try:  a: 1
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=/*%0Aa%3A%20true%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%200%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%201%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20null%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20undefined%20%20--%3E%20%3F%0Aa%3A%20''%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'%20'%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'tiil'%20%20%20%20%20--%3E%20%3F%0Aa%3A%202%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20345%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20NaN%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20Infinity%20%20%20--%3E%20%3F%0Aa%3A%20-Infinity%20%20--%3E%20%3F%0Aa%3A%20-3%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20-0.0%20%20%20%20%20%20%20--%3E%20%3F%0A*/%0A%0A%0Aconst%20a%20%3D%20false%20%3B%20//%20experiment%20with%20different%20values%20%0A%0Aconst%20truthiness%20%3D%20Boolean%28a%29%20%2B%20%22y%22%3B%0A%0Aconst%20not%20%3D%20!a%3B%0Aconst%20coercion_replication%20%3D%20!Boolean%28a%29%3B%0Aconst%20ternary_replication%20%3D%20%28a%29%20%3F%20false%20%3A%20true%20%3B&curInstr=5&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: 1          --> ? * false
const a = 1; // experiment with different values 

const truthiness = Boolean(a) + "y";

const not = !a;
const coercion_replication = !Boolean(a);
const ternary_replication = (a) ? false : true ;
```
---
---
### values to try:  a: null
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=/*%0Aa%3A%20true%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%200%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%201%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20null%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20undefined%20%20--%3E%20%3F%0Aa%3A%20''%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'%20'%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'tiil'%20%20%20%20%20--%3E%20%3F%0Aa%3A%202%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20345%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20NaN%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20Infinity%20%20%20--%3E%20%3F%0Aa%3A%20-Infinity%20%20--%3E%20%3F%0Aa%3A%20-3%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20-0.0%20%20%20%20%20%20%20--%3E%20%3F%0A*/%0A%0A%0Aconst%20a%20%3D%20null%20%3B%20//%20experiment%20with%20different%20values%20%0A%0Aconst%20truthiness%20%3D%20Boolean%28a%29%20%2B%20%22y%22%3B%0A%0Aconst%20not%20%3D%20!a%3B%0Aconst%20coercion_replication%20%3D%20!Boolean%28a%29%3B%0Aconst%20ternary_replication%20%3D%20%28a%29%20%3F%20false%20%3A%20true%20%3B&curInstr=5&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: null       --> ? * true
const a = null; // experiment with different values 

const truthiness = Boolean(a) + "y";

const not = !a;
const coercion_replication = !Boolean(a);
const ternary_replication = (a) ? false : true ;
```
---
---
### values to try:  a: undefined
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=/*%0Aa%3A%20true%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%200%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%201%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20null%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20undefined%20%20--%3E%20%3F%0Aa%3A%20''%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'%20'%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'tiil'%20%20%20%20%20--%3E%20%3F%0Aa%3A%202%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20345%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20NaN%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20Infinity%20%20%20--%3E%20%3F%0Aa%3A%20-Infinity%20%20--%3E%20%3F%0Aa%3A%20-3%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20-0.0%20%20%20%20%20%20%20--%3E%20%3F%0A*/%0A%0A%0Aconst%20a%20%3D%20undefined%20%3B%20//%20experiment%20with%20different%20values%20%0A%0Aconst%20truthiness%20%3D%20Boolean%28a%29%20%2B%20%22y%22%3B%0A%0Aconst%20not%20%3D%20!a%3B%0Aconst%20coercion_replication%20%3D%20!Boolean%28a%29%3B%0Aconst%20ternary_replication%20%3D%20%28a%29%20%3F%20false%20%3A%20true%20%3B&curInstr=5&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: undefined  --> ? * true
const a = undefined; // experiment with different values 

const truthiness = Boolean(a) + "y";

const not = !a;
const coercion_replication = !Boolean(a);
const ternary_replication = (a) ? false : true ;
```
---
### values to try:  a: ''
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=/*%0Aa%3A%20true%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%200%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%201%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20null%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20undefined%20%20--%3E%20%3F%0Aa%3A%20''%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'%20'%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'tiil'%20%20%20%20%20--%3E%20%3F%0Aa%3A%202%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20345%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20NaN%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20Infinity%20%20%20--%3E%20%3F%0Aa%3A%20-Infinity%20%20--%3E%20%3F%0Aa%3A%20-3%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20-0.0%20%20%20%20%20%20%20--%3E%20%3F%0A*/%0A%0A%0Aconst%20a%20%3D%20%22%22%20%3B%20//%20experiment%20with%20different%20values%20%0A%0Aconst%20truthiness%20%3D%20Boolean%28a%29%20%2B%20%22y%22%3B%0A%0Aconst%20not%20%3D%20!a%3B%0Aconst%20coercion_replication%20%3D%20!Boolean%28a%29%3B%0Aconst%20ternary_replication%20%3D%20%28a%29%20%3F%20false%20%3A%20true%20%3B&curInstr=5&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: ''         --> ? * true
const a = '' ; // experiment with different values 

const truthiness = Boolean(a) + "y";

const not = !a;
const coercion_replication = !Boolean(a);
const ternary_replication = (a) ? false : true ;
```
---
### values to try:  a: ' ' 
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=/*%0Aa%3A%20true%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%200%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%201%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20null%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20undefined%20%20--%3E%20%3F%0Aa%3A%20''%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'%20'%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'tiil'%20%20%20%20%20--%3E%20%3F%0Aa%3A%202%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20345%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20NaN%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20Infinity%20%20%20--%3E%20%3F%0Aa%3A%20-Infinity%20%20--%3E%20%3F%0Aa%3A%20-3%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20-0.0%20%20%20%20%20%20%20--%3E%20%3F%0A*/%0A%0A%0Aconst%20a%20%3D%20%22%20%22%20%3B%20//%20experiment%20with%20different%20values%20%0A%0Aconst%20truthiness%20%3D%20Boolean%28a%29%20%2B%20%22y%22%3B%0A%0Aconst%20not%20%3D%20!a%3B%0Aconst%20coercion_replication%20%3D%20!Boolean%28a%29%3B%0Aconst%20ternary_replication%20%3D%20%28a%29%20%3F%20false%20%3A%20true%20%3B&curInstr=4&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: ' '        --> ? * false
const a = ' '; // experiment with different values 

const truthiness = Boolean(a) + "y";

const not = !a;
const coercion_replication = !Boolean(a);
const ternary_replication = (a) ? false : true ;
```
---
### values to try:  a: 'tiil'
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=/*%0Aa%3A%20true%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%200%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%201%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20null%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20undefined%20%20--%3E%20%3F%0Aa%3A%20''%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'%20'%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'tiil'%20%20%20%20%20--%3E%20%3F%0Aa%3A%202%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20345%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20NaN%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20Infinity%20%20%20--%3E%20%3F%0Aa%3A%20-Infinity%20%20--%3E%20%3F%0Aa%3A%20-3%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20-0.0%20%20%20%20%20%20%20--%3E%20%3F%0A*/%0A%0A%0Aconst%20a%20%3D%20%22tiil%22%20%3B%20//%20experiment%20with%20different%20values%20%0A%0Aconst%20truthiness%20%3D%20Boolean%28a%29%20%2B%20%22y%22%3B%0A%0Aconst%20not%20%3D%20!a%3B%0Aconst%20coercion_replication%20%3D%20!Boolean%28a%29%3B%0Aconst%20ternary_replication%20%3D%20%28a%29%20%3F%20false%20%3A%20true%20%3B&curInstr=5&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: 'tiil'     --> ? * false
const a = 'tiil'; // experiment with different values 

const truthiness = Boolean(a) + "y";

const not = !a;
const coercion_replication = !Boolean(a);
const ternary_replication = (a) ? false : true ;
```
---
---
### values to try:  a: 2
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=/*%0Aa%3A%20true%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%200%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%201%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20null%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20undefined%20%20--%3E%20%3F%0Aa%3A%20''%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'%20'%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'tiil'%20%20%20%20%20--%3E%20%3F%0Aa%3A%202%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20345%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20NaN%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20Infinity%20%20%20--%3E%20%3F%0Aa%3A%20-Infinity%20%20--%3E%20%3F%0Aa%3A%20-3%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20-0.0%20%20%20%20%20%20%20--%3E%20%3F%0A*/%0A%0A%0Aconst%20a%20%3D%202%3B%20//%20experiment%20with%20different%20values%20%0A%0Aconst%20truthiness%20%3D%20Boolean%28a%29%20%2B%20%22y%22%3B%0A%0Aconst%20not%20%3D%20!a%3B%0Aconst%20coercion_replication%20%3D%20!Boolean%28a%29%3B%0Aconst%20ternary_replication%20%3D%20%28a%29%20%3F%20false%20%3A%20true%20%3B&curInstr=5&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: 2          --> ? * false
const a = 2; // experiment with different values 

const truthiness = Boolean(a) + "y";

const not = !a;
const coercion_replication = !Boolean(a);
const ternary_replication = (a) ? false : true ;
```
---
### values to try:  a: 345
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=/*%0Aa%3A%20true%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%200%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%201%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20null%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20undefined%20%20--%3E%20%3F%0Aa%3A%20''%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'%20'%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'tiil'%20%20%20%20%20--%3E%20%3F%0Aa%3A%202%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20345%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20NaN%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20Infinity%20%20%20--%3E%20%3F%0Aa%3A%20-Infinity%20%20--%3E%20%3F%0Aa%3A%20-3%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20-0.0%20%20%20%20%20%20%20--%3E%20%3F%0A*/%0A%0A%0Aconst%20a%20%3D%20345%3B%20//%20experiment%20with%20different%20values%20%0A%0Aconst%20truthiness%20%3D%20Boolean%28a%29%20%2B%20%22y%22%3B%0A%0Aconst%20not%20%3D%20!a%3B%0Aconst%20coercion_replication%20%3D%20!Boolean%28a%29%3B%0Aconst%20ternary_replication%20%3D%20%28a%29%20%3F%20false%20%3A%20true%20%3B&curInstr=5&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: 345        --> ? * false
const a = 345; // experiment with different values 

const truthiness = Boolean(a) + "y";

const not = !a;
const coercion_replication = !Boolean(a);
const ternary_replication = (a) ? false : true ;
```
---
### values to try:  a: NaN
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=/*%0Aa%3A%20true%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%200%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%201%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20null%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20undefined%20%20--%3E%20%3F%0Aa%3A%20''%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'%20'%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'tiil'%20%20%20%20%20--%3E%20%3F%0Aa%3A%202%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20345%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20NaN%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20Infinity%20%20%20--%3E%20%3F%0Aa%3A%20-Infinity%20%20--%3E%20%3F%0Aa%3A%20-3%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20-0.0%20%20%20%20%20%20%20--%3E%20%3F%0A*/%0A%0A%0Aconst%20a%20%3D%20NaN%3B%20//%20experiment%20with%20different%20values%20%0A%0Aconst%20truthiness%20%3D%20Boolean%28a%29%20%2B%20%22y%22%3B%0A%0Aconst%20not%20%3D%20!a%3B%0Aconst%20coercion_replication%20%3D%20!Boolean%28a%29%3B%0Aconst%20ternary_replication%20%3D%20%28a%29%20%3F%20false%20%3A%20true%20%3B&curInstr=5&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: NaN        --> ? * true
const a = NaN; // experiment with different values 

const truthiness = Boolean(a) + "y";

const not = !a;
const coercion_replication = !Boolean(a);
const ternary_replication = (a) ? false : true ;
```
---
### values to try:  a: Infinity 
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=/*%0Aa%3A%20true%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%200%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%201%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20null%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20undefined%20%20--%3E%20%3F%0Aa%3A%20''%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'%20'%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'tiil'%20%20%20%20%20--%3E%20%3F%0Aa%3A%202%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20345%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20NaN%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20Infinity%20%20%20--%3E%20%3F%0Aa%3A%20-Infinity%20%20--%3E%20%3F%0Aa%3A%20-3%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20-0.0%20%20%20%20%20%20%20--%3E%20%3F%0A*/%0A%0A%0Aconst%20a%20%3D%20Infinity%3B%20//%20experiment%20with%20different%20values%20%0A%0Aconst%20truthiness%20%3D%20Boolean%28a%29%20%2B%20%22y%22%3B%0A%0Aconst%20not%20%3D%20!a%3B%0Aconst%20coercion_replication%20%3D%20!Boolean%28a%29%3B%0Aconst%20ternary_replication%20%3D%20%28a%29%20%3F%20false%20%3A%20true%20%3B&curInstr=5&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: Infinity   --> ? * false
const a = Infinity; // experiment with different values 

const truthiness = Boolean(a) + "y";

const not = !a;
const coercion_replication = !Boolean(a);
const ternary_replication = (a) ? false : true ;
```
---
---
### values to try:  a: -Infinity
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=/*%0Aa%3A%20true%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%200%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%201%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20null%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20undefined%20%20--%3E%20%3F%0Aa%3A%20''%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'%20'%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'tiil'%20%20%20%20%20--%3E%20%3F%0Aa%3A%202%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20345%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20NaN%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20Infinity%20%20%20--%3E%20%3F%0Aa%3A%20-Infinity%20%20--%3E%20%3F%0Aa%3A%20-3%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20-0.0%20%20%20%20%20%20%20--%3E%20%3F%0A*/%0A%0A%0Aconst%20a%20%3D%20-Infinity%3B%20//%20experiment%20with%20different%20values%20%0A%0Aconst%20truthiness%20%3D%20Boolean%28a%29%20%2B%20%22y%22%3B%0A%0Aconst%20not%20%3D%20!a%3B%0Aconst%20coercion_replication%20%3D%20!Boolean%28a%29%3B%0Aconst%20ternary_replication%20%3D%20%28a%29%20%3F%20false%20%3A%20true%20%3B&curInstr=5&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: -Infinity  --> ? * FALSE
const a = -Infinity; // experiment with different values 

const truthiness = Boolean(a) + "y";

const not = !a;
const coercion_replication = !Boolean(a);
const ternary_replication = (a) ? false : true ;
```
---
---
### values to try:  a: -3
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=/*%0Aa%3A%20true%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%200%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%201%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20null%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20undefined%20%20--%3E%20%3F%0Aa%3A%20''%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'%20'%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'tiil'%20%20%20%20%20--%3E%20%3F%0Aa%3A%202%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20345%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20NaN%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20Infinity%20%20%20--%3E%20%3F%0Aa%3A%20-Infinity%20%20--%3E%20%3F%0Aa%3A%20-3%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20-0.0%20%20%20%20%20%20%20--%3E%20%3F%0A*/%0A%0A%0Aconst%20a%20%3D%20-3%3B%20//%20experiment%20with%20different%20values%20%0A%0Aconst%20truthiness%20%3D%20Boolean%28a%29%20%2B%20%22y%22%3B%0A%0Aconst%20not%20%3D%20!a%3B%0Aconst%20coercion_replication%20%3D%20!Boolean%28a%29%3B%0Aconst%20ternary_replication%20%3D%20%28a%29%20%3F%20false%20%3A%20true%20%3B&curInstr=5&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: -3         --> ? * FALSE
const a = -3; // experiment with different values 

const truthiness = Boolean(a) + "y";

const not = !a;
const coercion_replication = !Boolean(a);
const ternary_replication = (a) ? false : true ;
```
---
---
### values to try:  a: -0.0
* My solution [on pytut](http://www.pythontutor.com/javascript.html#code=/*%0Aa%3A%20true%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20false%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%200%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%201%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20null%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20undefined%20%20--%3E%20%3F%0Aa%3A%20''%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'%20'%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20'tiil'%20%20%20%20%20--%3E%20%3F%0Aa%3A%202%20%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20345%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20NaN%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20Infinity%20%20%20--%3E%20%3F%0Aa%3A%20-Infinity%20%20--%3E%20%3F%0Aa%3A%20-3%20%20%20%20%20%20%20%20%20--%3E%20%3F%0Aa%3A%20-0.0%20%20%20%20%20%20%20--%3E%20%3F%0A*/%0A%0A%0Aconst%20a%20%3D%20-0.0%3B%20//%20experiment%20with%20different%20values%20%0A%0Aconst%20truthiness%20%3D%20Boolean%28a%29%20%2B%20%22y%22%3B%0A%0Aconst%20not%20%3D%20!a%3B%0Aconst%20coercion_replication%20%3D%20!Boolean%28a%29%3B%0Aconst%20ternary_replication%20%3D%20%28a%29%20%3F%20false%20%3A%20true%20%3B&curInstr=5&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
a: -0.0       --> ? * true
const a = -0.0; // experiment with different values 

const truthiness = Boolean(a) + "y";

const not = !a;
const coercion_replication = !Boolean(a);
const ternary_replication = (a) ? false : true ;
```

---

[TOP](#truthiness)

---

## Resources

__study tools__:
* [PythonTutor for JavaScript](http://pythontutor.com/javascript.html#)
* [the Parsonizer](https://janke-learning.github.io/parsonizer/)

__helpful links__:
* pytut snippets:
    * [truthy & falsey values](https://goo.gl/jBTLFD) 
    * [&& vs. ||](https://goo.gl/BBXea6)  
* [javascript.info](http://javascript.info/logical-operators)  
* mdn: [logicals](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Logical_Operators), [ternary](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Conditional_Operator)
* [truthiness & comparisons](https://dorey.github.io/JavaScript-Equality-Table/) - click on the "if()" tab for truthiness
* from __boolean by example__: 
    * [truthiness for the console](https://github.com/janke-learning/boolean-by-example/blob/master/README.md#truthiness) 
    * [&&, || for the console](https://github.com/janke-learning/boolean-by-example#and-or-operators)
    * [! for the console](https://github.com/janke-learning/boolean-by-example#not)
    * [live in devtools](https://janke-learning.github.io/boolean-by-example/)
* mdn: 
    * [boolean](https://developer.mozilla.org/en-US/docs/Glossary/Boolean)  
    * [truthy](https://developer.mozilla.org/en-US/docs/Glossary/Truthy)  
    * [falsey](https://developer.mozilla.org/en-US/docs/Glossary/Falsy)  
* [a codepen](https://codepen.io/philipwalton/pen/nufrk) 

[TOP](#truthiness)

___
___
### <a href="http://janke-learning.org" target="_blank"><img src="https://user-images.githubusercontent.com/18554853/50098409-22575780-021c-11e9-99e1-962787adaded.png" width="40" height="40"></img> Janke Learning</a>
