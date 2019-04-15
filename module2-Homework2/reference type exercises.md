[TOP](#reference-type-exercises)

---

## Reference Exercises

__Swap the Object & the Array__  

```js
let obj = [];
let arr = {};
let _ = null;

// --- swap below here ---

```
1 [on pytut exercise 1](http://www.pythontutor.com/javascript.html#code=let%20obj%20%3D%20%5B%5D%3B%0Alet%20arr%20%3D%20%7B%7D%3B%0Alet%20_%20%3D%20null%3B%0A%0A//%20swap%20the%20object%20and%20the%20array%0A_%20%3D%20obj%3B%0Aobj%20%3D%20arr%3B%0Aarr%20%3D%20_%3B&curInstr=0&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
let obj = [];
let arr = {};
let _ = null;

// --- swap below here ---
_ = obj;
obj = arr;
arr = _;

```
_Complete this code__  


```js
let value_1 = 5;
let reference_1 = [];

let value_2 = value_1;
console.assert(value_2 /* === or !== ? */ value_1);

let reference_2 = reference_1;
console.assert(reference_2 /* === or !== ? */ reference_1);

    ; // write this line
console.assert(value_1 !== value_2);  

    ; // write this line
console.assert(reference_1[0] === reference_2[0]);

// remove the array from memory
    ; // write this line
    ; // write this line
```
2 [on pytut exercise 2](http://www.pythontutor.com/javascript.html#code=%20%20let%20value_1%20%3D%205%3B%0A%20%20let%20reference_1%20%3D%20%5B%5D%3B%0A%0A%20%20let%20value_2%20%3D%20value_1%3B%0A%20%20console.assert%28value_2%20%20%3D%3D%3D%20%20value_1%29%3B%0A%0A%20%20let%20reference_2%20%3D%20reference_1%3B%0A%20%20console.assert%28reference_2%20%20%3D%3D%3D%20reference_1%29%3B%0A%0A%20value_1%20%3D%208%3B%20//%20write%20this%20line%0A%20%20console.assert%28value_1%20!%3D%3D%20value_2%29%3B%20%20%0A%20%20%20%20%0A%20%20reference_1%3D%5B0%5D,%20reference_2%20%3D%20%5B0%5D%20%3B%20//%20write%20this%20line%0A%20%20console.assert%28reference_1%5B0%5D%20%3D%3D%3D%20reference_2%5B0%5D%29%3B%0A%0A%20%20//%20remove%20the%20array%20from%20memory%0A%20%20%20%20%20reference_1%20%3D%20null%20%3B%20//%20write%20this%20line%0A%20%20%20%20reference_2%20%3D%20null%20%20%3B%20//%20write%20this%20line&curInstr=12&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
 let value_1 = 5;
  let reference_1 = [];

  let value_2 = value_1;
  console.assert(value_2  ===  value_1);

  let reference_2 = reference_1;
  console.assert(reference_2  === reference_1);

 value_1 = 8; // write this line
  console.assert(value_1 !== value_2);  
    
  reference_1=[0], reference_2 = [0] ; // write this line
  console.assert(reference_1[0] === reference_2[0]);

  // remove the array from memory
     reference_1 = null ; // write this line
    reference_2 = null  ; // write this line
```
## Array Exercises

__Complete the Assertions__  

```js
let a_1 = [];
let a_2 = a_1;
console.assert(a_1 /* === or !== ? */ a_2);

let b_1 = [];
let b_2 = [];
console.assert(b_1 /* === or !== ? */ b_2);

// ---

let a_1.push(3);
let a_2.push(3);
console.assert(a_1 /* === or !== ? */ a_2);

let b_1.push(5);
let b_2.push(5);
console.assert(b_1 /* === or !== ? */ b_2);
```
3 [on pytut exercise 3](http://www.pythontutor.com/javascript.html#code=let%20a_1%20%3D%20%5B%5D%3B%0Alet%20a_2%20%3D%20a_1%3B%0Aconsole.assert%28a_1%20%20%3D%3D%3D%20%20a_2%29%3B%0A%0Alet%20b_1%20%3D%20%5B%5D%3B%0Alet%20b_2%20%3D%20%5B%5D%3B%0Aconsole.assert%28b_1%20%20!%3D%3D%20%20b_2%29%3B%0A%0A//%20---%0A%0A%20a_1.push%283%29%3B%0A%20a_2.push%283%29%3B%0Aconsole.assert%28a_1%20%20%3D%3D%3D%20%20%20a_2%29%3B%0A%0A%20b_1.push%285%29%3B%0A%20b_2.push%285%29%3B%0Aconsole.assert%28b_1%20!%3D%3D%20b_2%29%3B&curInstr=12&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
let a_1 = [];
let a_2 = a_1;
console.assert(a_1  ===  a_2);

let b_1 = [];
let b_2 = [];
console.assert(b_1  !==  b_2);

// ---

 a_1.push(3);
 a_2.push(3);
console.assert(a_1  ===   a_2);

 b_1.push(5);
 b_2.push(5);
console.assert(b_1 !== b_2);
```
Complete the Assertions__  

```js
let a_1 = [];
let a_2 = a_1;
console.assert(a_1 /* === or !== ? */ a_2);

let b_1 = [];
let b_2 = [];
console.assert(b_1 /* === or !== ? */ b_2);

// ---

const index = 0;

let a_1[index] = 3;
let a_2[index] = 3;
console.assert(a_1 /* === or !== ? */ a_2);

let b_1[index] = 5;
let b_2[index] = 5;
console.assert(b_1 /* === or !== ? */ b_2);
```
4 [on pytut exercise 4](http://www.pythontutor.com/javascript.html#code=let%20a_1%20%3D%20%5B%5D%3B%0Alet%20a_2%20%3D%20a_1%3B%0Aconsole.assert%28a_1%20%3D%3D%3D%20%20a_2%29%3B%0A%0Alet%20b_1%20%3D%20%5B%5D%3B%0Alet%20b_2%20%3D%20%5B%5D%3B%0Aconsole.assert%28b_1%20!%3D%3D%20b_2%29%3B%0A%0A//%20---%0A%0Aconst%20index%20%3D%200%3B%0A%0A%20a_1%5Bindex%5D%20%3D%203%3B%0A%20a_2%5Bindex%5D%20%3D%203%3B%0Aconsole.assert%28a_1%20%3D%3D%3D%20a_2%29%3B%0A%0A%20b_1%5Bindex%5D%20%3D%205%3B%0A%20b_2%5Bindex%5D%20%3D%205%3B%0Aconsole.assert%28b_1%20%20!%3D%3D%20%20b_2%29%3B&curInstr=13&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
let a_1 = [];
let a_2 = a_1;
console.assert(a_1 ===  a_2);

let b_1 = [];
let b_2 = [];
console.assert(b_1 !== b_2);

// ---

const index = 0;

 a_1[index] = 3;
 a_2[index] = 3;
console.assert(a_1 === a_2);

 b_1[index] = 5;
 b_2[index] = 5;
console.assert(b_1  !==  b_2);
```
__Fill in the Blanks__  

```js
    ; // write this line
    ; // write this line
console.assert(arr_1 !== arr_2);
console.assert(arr_1[1] === arr_2[1]);

let key = 0;
console.assert(arr_1[key] === arr_2[key]);

    ; // write this line
    ; // write this line
console.assert(arr_1[arr_2[2]] === arr_2[arr_1[2]]);

    ; // write this line
    ; // write this line
console.assert(arr_1 === arr_2);
console.assert(arr_3 !== arr_1);
console.assert(arr_3 !== arr_2);
console.assert(arr_3[key] === arr_1[0]);

    ; // write this line
console.assert(obj_3[1] === obj_2[key]);
```
5 [on pytut exercise 5](http://www.pythontutor.com/javascript.html#code=let%20arr_1%20%3D%20%5B1%5D%20%3B%20//%20write%20this%20line%0Alet%20arr_2%20%3D%20arr_1%20%20%3B%20//%20write%20this%20line%0A%0Aconsole.assert%28arr_1%5B1%5D%20%3D%3D%3D%20arr_2%5B1%5D%29%3B%0A%0Alet%20key%20%3D%200%3B%0Aarr_1%5Bkey%5D%3B%0Aarr_2%5Bkey%5D%3B%0Aconsole.assert%28arr_1%5Bkey%5D%20%3D%3D%3D%20arr_2%5Bkey%5D%29%3B%0A%0Aarr_1%20%3D%20%5B2,2,2%5D%20%3B%20//%20write%20this%20line%0Aarr_2%20%3D%20%5B2,2,2%5D%20%3B%20//%20write%20this%20line%0Aconsole.assert%28arr_1%5Barr_2%5B2%5D%5D%20%3D%3D%3D%20arr_2%5Barr_1%5B2%5D%5D%29%3B%0Aconsole.log%28arr_1%5Barr_2%5B2%5D%5D%29%3B%0Alet%20arr_3%20%3D%20%5B2,3,3%5D%20%3B%20//%20write%20this%20line%0A%20arr_1%3Darr_2%20%20%20%3B%20//%20write%20this%20line%0Aconsole.assert%28arr_1%20%3D%3D%3D%20arr_2%29%3B%0Aconsole.assert%28arr_3%20!%3D%3D%20arr_1%29%3B%0Aconsole.assert%28arr_3%20!%3D%3D%20arr_2%29%3B%0Aconsole.assert%28arr_3%5Bkey%5D%20%3D%3D%3D%20arr_1%5B0%5D%29%3B%0A%0A%20let%20obj_2%20%3D%20%5B1,%202%5D%3B%0A%20let%20obj_3%20%3D%20%5B0,%201%5D%3B%20//%20write%20this%20line%0Aconsole.assert%28obj_3%5B1%5D%20%3D%3D%3D%20obj_2%5Bkey%5D%29%3B&curInstr=20&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
let arr_1 = [1] ; // write this line
let arr_2 = arr_1  ; // write this line

console.assert(arr_1[1] === arr_2[1]);

let key = 0;
arr_1[key];
arr_2[key];
console.assert(arr_1[key] === arr_2[key]);

arr_1 = [2,2,2] ; // write this line
arr_2 = [2,2,2] ; // write this line
console.assert(arr_1[arr_2[2]] === arr_2[arr_1[2]]);
console.log(arr_1[arr_2[2]]);
let arr_3 = [2,3,3] ; // write this line
 arr_1=arr_2   ; // write this line
console.assert(arr_1 === arr_2);
console.assert(arr_3 !== arr_1);
console.assert(arr_3 !== arr_2);
console.assert(arr_3[key] === arr_1[0]);

 let obj_2 = [1, 2];
 let obj_3 = [0, 1]; // write this line
console.assert(obj_3[1] === obj_2[key]);
```
[TOP](#reference-type-exercises)

---

## Object Exercises

__Complete the Assertions__  

```js
let a_1 = {};
let a_2 = a_1;
console.assert(a_1 /* === or !== ? */ a_2);

let b_1 = {};
let b_2 = {};
console.assert(b_1 /* === or !== ? */ b_2);

// ---

let a_1.x = 3;
let a_2.x = 3;
console.assert(a_1 /* === or !== ? */ a_2);

let b_1.x = 5;
let b_2.x = 5;
console.assert(b_1 /* === or !== ? */ b_2);
```
6 [on pytut exercise 6](http://www.pythontutor.com/javascript.html#code=let%20a_1%20%3D%20%7B%7D%3B%0Alet%20a_2%20%3D%20a_1%3B%0Aconsole.assert%28a_1%20%3D%3D%3D%20a_2%29%3B%0A%0Alet%20b_1%20%3D%20%7B%7D%3B%0Alet%20b_2%20%3D%20%7B%7D%3B%0Aconsole.assert%28b_1%20!%3D%3D%20b_2%29%3B%0A%0A//%20---%0A%0Aa_1.x%20%3D%203%3B%0Aa_2.x%20%3D%203%3B%0Aconsole.assert%28a_1%20%3D%3D%3D%20a_2%29%3B%0A%0Ab_1.x%20%3D%205%3B%0Ab_2.x%20%3D%205%3B%0Aconsole.assert%28b_1%20!%3D%3D%20%20b_2%29%3B&curInstr=12&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
let a_1 = {};
let a_2 = a_1;
console.assert(a_1 === a_2);

let b_1 = {};
let b_2 = {};
console.assert(b_1 !== b_2);

// ---

a_1.x = 3;
a_2.x = 3;
console.assert(a_1 === a_2);

b_1.x = 5;
b_2.x = 5;
console.assert(b_1 !==  b_2);
```
_Complete the Assertions__  

```js
let a_1 = {};
let a_2 = a_1;
console.assert(a_1 /* === or !== ? */ a_2);

let b_1 = {};
let b_2 = {};
console.assert(b_1 /* === or !== ? */ b_2);

// ---

const key = "x";

let a_1[key] = 3;
let a_2[key] = 3;
console.assert(a_1 /* === or !== ? */ a_2);

let b_1[key] = 5;
let b_2[key] = 5;
console.assert(b_1 /* === or !== ? */ b_2);
```
7[on pytut exercise 7](http://www.pythontutor.com/javascript.html#code=%20%20let%20a_1%20%3D%20%7B%7D%3B%0A%20%20let%20a_2%20%3D%20a_1%3B%0A%20%20console.assert%28a_1%20%3D%3D%3D%20a_2%29%3B%0A%0A%20%20let%20b_1%20%3D%20%7B%7D%3B%0A%20%20let%20b_2%20%3D%20%7B%7D%3B%0A%20%20console.assert%28b_1%20!%3D%3D%20b_2%29%3B%0A%0A%20%20//%20---%0A%20%20%0A%20%20const%20key%20%3D%20%22x%22%3B%0A%0A%20%20%20a_1%5Bkey%5D%20%3D%203%3B%0A%20%20%20a_2%5Bkey%5D%20%3D%203%3B%0A%20%20console.assert%28a_1%20%3D%3D%3D%20a_2%29%3B%0A%0A%20%20b_1%5Bkey%5D%20%3D%205%3B%0A%20%20b_2%5Bkey%5D%20%3D%205%3B%0A%20%20console.assert%28b_1%20!%3D%3D%20b_2%29%3B&curInstr=13&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
 let a_1 = {};
  let a_2 = a_1;
  console.assert(a_1 === a_2);

  let b_1 = {};
  let b_2 = {};
  console.assert(b_1 !== b_2);

  // ---
  
  const key = "x";

   a_1[key] = 3;
   a_2[key] = 3;
  console.assert(a_1 === a_2);

  b_1[key] = 5;
  b_2[key] = 5;
  console.assert(b_1 !== b_2);
```
_Fill in the Blanks__  

```js
    ; // write this line
    ; // write this line
console.assert(obj_1 !== obj_2);
console.assert(obj_1.x === obj_2.x);

let key = "y";
console.assert(obj_1[key] === obj_2[key]);

    ; // write this line
    ; // write this line
console.assert(obj_1[obj_2.y] === obj_2[obj_1.y]);

    ; // write this line
    ; // write this line
console.assert(obj_1 === obj_2);
console.assert(obj_3 !== obj_1);
console.assert(obj_3 !== obj_2);
console.assert(obj_3[key] === obj_1.y);

    ; // write this line
console.assert(obj_3.x === obj_2[key]);
```
8 [on pytut exercise 8](http://www.pythontutor.com/javascript.html#code=let%20obj_1%20%3D%20%7Bx%3A1,y%3A3,%20z%3A5,%20a%3A7%7D%20%3B%0Alet%20obj_2%20%3D%20%7Bx%3A1,%20y%3A3,%20z%3A6,%20a%3A7%7D%3B%20//%20write%20this%20line%0Aobj_1.x%20%3D%20obj_2.x%3B//%20write%20this%20line%0Aconsole.assert%28obj_1%20!%3D%3D%20obj_2%29%3B%0Aconsole.assert%28obj_1.x%20%3D%3D%3D%20obj_2.x%29%3B%0A%0Alet%20key%20%3D%20%22y%22%3B%0Aconsole.assert%28obj_1%5Bkey%5D%20%3D%3D%3D%20obj_2%5Bkey%5D%29%3B%0A%0Aobj_1%20%3D%20%7Bx%3A1,%20y%3A3,%20z%3A5,%20a%3A%5B7,2%5D%7D%3B%20//%20write%20this%20line%0Aobj_2%20%3D%20%7Bx%3A1,%20y%3A3,%20z%3A6,%20a%3A%5B7,2%5D%7D%20%3B%20//%20write%20this%20line%0Aconsole.assert%28obj_1%5Bobj_2.y%5D%20%3D%3D%3D%20obj_2%5Bobj_1.y%5D%29%3B%0Aconsole.log%28obj_1%5Bobj_2.y%5D%29%3B%0A%20%20let%20obj_3%20%3D%20%7Bx%3A3,%20y%3A3%7D%3B%20//%20write%20this%20line%0A%20%20obj_1%20%3D%20obj_2%3B%20//%20write%20this%20line%0Aconsole.assert%28obj_1%20%3D%3D%3D%20obj_2%29%3B%0Aconsole.assert%28obj_3%20!%3D%3D%20obj_1%29%3B%0Aconsole.assert%28obj_3%20!%3D%3D%20obj_2%29%3B%0Aconsole.assert%28obj_3%5Bkey%5D%20%3D%3D%3D%20obj_1.y%29%3B%0Aconsole.log%28obj_3%5Bkey%5D%29%3B%0A%0A%20%20%20%20%3B%20//%20write%20this%20line%0Aconsole.assert%28obj_3.x%20%3D%3D%3D%20obj_2%5Bkey%5D%29%3B&curInstr=19&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
let obj_1 = {x:1,y:3, z:5, a:7} ;
let obj_2 = {x:1, y:3, z:6, a:7}; // write this line
obj_1.x = obj_2.x;// write this line
console.assert(obj_1 !== obj_2);
console.assert(obj_1.x === obj_2.x);

let key = "y";
console.assert(obj_1[key] === obj_2[key]);

obj_1 = {x:1, y:3, z:5, a:[7,2]}; // write this line
obj_2 = {x:1, y:3, z:6, a:[7,2]} ; // write this line
console.assert(obj_1[obj_2.y] === obj_2[obj_1.y]);
console.log(obj_1[obj_2.y]);
  let obj_3 = {x:3, y:3}; // write this line
  obj_1 = obj_2; // write this line
console.assert(obj_1 === obj_2);
console.assert(obj_3 !== obj_1);
console.assert(obj_3 !== obj_2);
console.assert(obj_3[key] === obj_1.y);
console.log(obj_3[key]);

    ; // write this line
console.assert(obj_3.x === obj_2[key]);
```

[TOP](#reference-type-exercises)

---

## Comparison Exercises

__Swap 'em__  

```js
const obj = {prop: "array"};
const arr = ["object"];
let _ = null;

// swap the values stored in each structure
//  using dot notation for the object
//  using direct access for the array
```
9 [on pytut exercise 9](http://www.pythontutor.com/javascript.html#code=const%20obj%20%3D%20%7Bprop%3A%20%22array%22%7D%3B%0Aconst%20arr%20%3D%20%5B%22object%22%5D%3B%0Alet%20_%20%3D%20null%3B%0A%0A//%20swap%20the%20values%20stored%20in%20each%20structure%0A//%20%20using%20dot%20notation%20for%20the%20object%0A//%20%20using%20direct%20access%20for%20the%20array%0A_%20%3D%20obj.prop%3B%0Aobj.prop%20%3D%20arr%3B%0A%20arr%5B0%5D%20%3D%20_%3B%0A&curInstr=6&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
const obj = {prop: "array"};
const arr = ["object"];
let _ = null;

// swap the values stored in each structure
//  using dot notation for the object
//  using direct access for the array
_ = obj.prop;
obj.prop = arr;
 arr[0] = _;
```
__Swap 'em__  

```js
const obj = {prop: "array"};
const arr = ["object"];
let _ = null;

// swap the values stored in each structure
//  using bracket notation for the object
//  using variable access for the array
const obj_key = ;
const arr_index = ;
```
10 [on pytut exercise 10](http://www.pythontutor.com/javascript.html#code=const%20obj%20%3D%20%7Bprop%3A%20%22array%22%7D%3B%0Aconst%20arr%20%3D%20%5B%22object%22%5D%3B%0Alet%20_%20%3D%20null%3B%0A%0A//%20swap%20the%20values%20stored%20in%20each%20structure%0A//%20%20using%20bracket%20notation%20for%20the%20object%0A//%20%20using%20variable%20access%20for%20the%20array%0Aconst%20obj_key%20%3D%20%3B%0Aconst%20arr_index%20%3D%20%3B&mode=edit&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)  
```js

```
