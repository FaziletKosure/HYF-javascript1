[TOP](#reference-type-exercises)

---

## Reference Exercises

__Swap the Object & the Array__  
1 [on pytut exercise 1](http://www.pythontutor.com/javascript.html#code=let%20obj%20%3D%20%5B%5D%3B%0Alet%20arr%20%3D%20%7B%7D%3B%0Alet%20_%20%3D%20null%3B%0A%0A//%20swap%20the%20object%20and%20the%20array%0A_%20%3D%20obj%3B%0Aobj%20%3D%20arr%3B%0Aarr%20%3D%20_%3B&curInstr=0&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
let obj = [];
let arr = {};
let _ = null;

// --- swap below here ---

```
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

2 [on pytut exercise 2](http://www.pythontutor.com/javascript.html#code=%20%20let%20value_1%20%3D%205%3B%0A%20%20let%20reference_1%20%3D%20%5B%5D%3B%0A%0A%20%20let%20value_2%20%3D%20value_1%3B%0A%20%20console.assert%28value_2%20%20%3D%3D%3D%20%20value_1%29%3B%0A%0A%20%20let%20reference_2%20%3D%20reference_1%3B%0A%20%20console.assert%28reference_2%20%20%3D%3D%3D%20reference_1%29%3B%0A%0A%20value_1%20%3D%208%3B%20//%20write%20this%20line%0A%20%20console.assert%28value_1%20!%3D%3D%20value_2%29%3B%20%20%0A%20%20%20%20%0A%20%20reference_1%3D%5B0%5D,%20reference_2%20%3D%20%5B0%5D%20%3B%20//%20write%20this%20line%0A%20%20console.assert%28reference_1%5B0%5D%20%3D%3D%3D%20reference_2%5B0%5D%29%3B%0A%0A%20%20//%20remove%20the%20array%20from%20memory%0A%20%20%20%20%20reference_1%20%3D%20null%20%3B%20//%20write%20this%20line%0A%20%20%20%20reference_2%20%3D%20null%20%20%3B%20//%20write%20this%20line&curInstr=12&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
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
3 [on pytut exercise 3](http://www.pythontutor.com/javascript.html#code=let%20a_1%20%3D%20%5B%5D%3B%0Alet%20a_2%20%3D%20a_1%3B%0Aconsole.assert%28a_1%20%20%3D%3D%3D%20%20a_2%29%3B%0A%0Alet%20b_1%20%3D%20%5B%5D%3B%0Alet%20b_2%20%3D%20%5B%5D%3B%0Aconsole.assert%28b_1%20%20!%3D%3D%20%20b_2%29%3B%0A%0A//%20---%0A%0A%20a_1.push%283%29%3B%0A%20a_2.push%283%29%3B%0Aconsole.assert%28a_1%20%20%3D%3D%3D%20%20%20a_2%29%3B%0A%0A%20b_1.push%285%29%3B%0A%20b_2.push%285%29%3B%0Aconsole.assert%28b_1%20!%3D%3D%20b_2%29%3B&curInstr=12&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
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
4 [on pytut exercise 4](http://www.pythontutor.com/javascript.html#code=let%20a_1%20%3D%20%5B%5D%3B%0Alet%20a_2%20%3D%20a_1%3B%0Aconsole.assert%28a_1%20%3D%3D%3D%20%20a_2%29%3B%0A%0Alet%20b_1%20%3D%20%5B%5D%3B%0Alet%20b_2%20%3D%20%5B%5D%3B%0Aconsole.assert%28b_1%20!%3D%3D%20b_2%29%3B%0A%0A//%20---%0A%0Aconst%20index%20%3D%200%3B%0A%0A%20a_1%5Bindex%5D%20%3D%203%3B%0A%20a_2%5Bindex%5D%20%3D%203%3B%0Aconsole.assert%28a_1%20%3D%3D%3D%20a_2%29%3B%0A%0A%20b_1%5Bindex%5D%20%3D%205%3B%0A%20b_2%5Bindex%5D%20%3D%205%3B%0Aconsole.assert%28b_1%20%20!%3D%3D%20%20b_2%29%3B&curInstr=13&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
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
