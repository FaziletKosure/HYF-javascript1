## exercise1
```js
// This is an in-line comment.
/* This is a
multi-line comment */
```
## exercise2 
```js
//Variable names can be made up of numbers, letters, and $ or _, but may not contain spaces or start with a number.
var myName;
```
 ## exercise3
 
```js
/*In JavaScript, you can store a value in a variable with the assignment operator.

myVariable = 5;

This assigns the Number value 5 to myVariable.

Assignment always goes from right to left. Everything to the right of the = operator is resolved before the value is assigned to the variable to the left of the operator.

myVar = 5;
myNum = myVar;
This assigns 5 to myVar and then resolves myVar to 5 again and assigns it to myNum.*/

//Assign the value 7 to variable a. Assign the contents of a to variable b.
var a = 7;
var b = a;
```
## exercise4 
```js
/*It is common to initialize a variable to an initial value in the same line as it is declared.

var myVar = 0;

Creates a new variable called myVar and assigns it an initial value of 0.*/
//Define a variable a with var and initialize it to a value of 9.
var a = 9;
```
## exercise5 
```js
/*When JavaScript variables are declared, they have an initial value of undefined. If you do a mathematical operation on an undefined variable your result will be NaN which means "Not a Number". If you concatenate a string with an undefined variable, you will get a literal string of "undefined".*/
//Initialize the three variables a, b, and c with 5, 10, and "I am a" respectively so that they will not be undefined.
var a = 5;
var b = 10;
var c = "I am a";
```
## exercise6 
```js
/*In JavaScript all variables and function names are case sensitive. This means that capitalization matters.

MYVAR is not the same as MyVar nor myvar. It is possible to have multiple distinct variables with the same name but different casing. It is strongly recommended that for the sake of clarity, you do not use this language feature.

Best Practice
Write variable names in JavaScript in camelCase. In camelCase, multi-word variable names have the first word in lowercase and the first letter of each subsequent word is capitalized.

Examples:

var someVariable;
var anotherVariableName;
var thisVariableNameIsSoLong;*/
//Modify the existing declarations and assignments so their names use camelCase.
//Do not create any new variables.
// Declarations
var studlyCapVar;
var properCamelCase;
var titleCaseOver;

// Assignments
studlyCapVar = 10;
properCamelCase = "A String";
titleCaseOver = 9000;
```
## exercise7 
```js
/*Number is a data type in JavaScript which represents numeric data.

Now let's try to add two numbers using JavaScript.

JavaScript uses the + symbol as addition operation when placed between two numbers.

Example

myVar = 5 + 10; // assigned 15*/
//Change the 0 so that sum will equal 20.
var sum = 10 + 10;
```
## exercise8 
```js
/*We can also subtract one number from another.

JavaScript uses the - symbol for subtraction.

Example

myVar = 12 - 6; // assigned 6*/
//Change the 0 so the difference is 12.
var difference = 45 - 33;
```
## exercise9 
```js
/*We can also multiply one number by another.

JavaScript uses the * symbol for multiplication of two numbers.

Example

myVar = 13 * 13; // assigned 169*/
//Change the 0 so that product will equal 80
var product = 8 * 10;
```
## exercise10 
```js
/*We can also divide one number by another.

JavaScript uses the / symbol for division.

Example

myVar = 16 / 2; // assigned 8*/
//Change the 0 so that the quotient is equal to 2.
var quotient = 66 / 33;
```
## exercise11 
```js
/*You can easily increment or add one to a variable with the ++ operator.

i++;

is the equivalent of

i = i + 1;

Note
The entire line becomes i++;, eliminating the need for the equal sign.*/
//Change the code to use the ++ operator on myVar.Hint
//Learn more about Arithmetic operators - Increment (++).
var myVar = 87;

// Only change code below this line
myVar ++;
```
## exercise12 
```js
/*You can easily decrement or decrease a variable by one with the -- operator.

i--;

is the equivalent of

i = i - 1;

Note
The entire line becomes i--;, eliminating the need for the equal sign.*/
//Change the code to use the ++ operator on myVar.Hint
//Learn more about Arithmetic operators - Increment (++).
var myVar = 87;

// Change the code to use the -- operator on myVar.
/*myVar should equal 10
myVar = myVar - 1; should be changed
Use the -- operator on myVar
Do not change code above the line*/
var myVar = 11;

// Only change code below this line
myVar --;
myVar --;
```
## exercise13 
```js
/*We can store decimal numbers in variables too. Decimal numbers are sometimes referred to as floating point numbers or floats.

Note
Not all real numbers can accurately be represented in floating point. This can lead to rounding errors. Details Here.*/
//Create a variable myDecimal and give it a decimal value with a fractional part (e.g. 5.7).
var ourDecimal = 5.7;
// Only change code below this line
var myDecimal = 6.2;

```
## exercise14 
```js
/*In JavaScript, you can also perform calculations with decimal numbers, just like whole numbers.

Let's multiply two decimals together to get their product.*/
//Change the 0.0 so that product will equal 5.0.
var product = 2.0 * 0.0;
var product = 2.0 * 2.5;
```
## exercise15 
```js
/*Now let's divide one decimal by another.*/
//Change the 0.0 so that quotient will equal to 2.2.
var quotient = 0.0 / 2.0; // Fix this line
var quotient = 4.4 / 2.0; // Fix this line
```
## exercise16 
```js
/*The remainder operator % gives the remainder of the division of two numbers.

Example

5 % 2 = 1 because
Math.floor(5 / 2) = 2 (Quotient)
2 * 2 = 4
5 - 4 = 1 (Remainder)
Usage
In mathematics, a number can be checked to be even or odd by checking the remainder of the division of the number by 2.

17 % 2 = 1 (17 is Odd)
48 % 2 = 0 (48 is Even)
Note
The remainder operator is sometimes incorrectly referred to as the "modulus" operator. It is very similar to modulus, but does not work properly with negative numbers.*/
//Set remainder equal to the remainder of 11 divided by 3 using the remainder (%) operator.
var remainder;
remainder=11%3;
```
## exercise17 
```js
/*In programming, it is common to use assignments to modify the contents of a variable. Remember that everything to the right of the equals sign is evaluated first, so we can say:

myVar = myVar + 5;

to add 5 to myVar. Since this is such a common pattern, there are operators which do both a mathematical operation and assignment in one step.

One such operator is the += operator.

var myVar = 1;
myVar += 5;
console.log(myVar); // Returns 6*/
//Convert the assignments for a, b, and c to use the += operator.
/*a should equal 15
b should equal 26
c should equal 19
You should use the += operator for each variable
Do not modify the code above the line*/
var a = 3;
var b = 17;
var c = 12;

// Only modify code below this line

a = a + 12;
b = 9 + b;
c = c + 7;
a += 12;
b += 9;
c += 7;
```
## exercise18 
```js
/*Like the += operator, -= subtracts a number from a variable.

myVar = myVar - 5;

will subtract 5 from myVar. This can be rewritten as:

myVar -= 5;*/
//Convert the assignments for a, b, and c to use the -= operator.
/*a should equal 5
b should equal -6
c should equal 2
You should use the -= operator for each variable
Do not modify the code above the lin*/
var a = 11;
var b = 9;
var c = 3;

// Only modify code below this line

a = a - 6;
b = b - 15;
c = c - 1;
a -=  6;
b -= 15;
c -= 1;
```
## exercise19 
```js
/*The *= operator multiplies a variable by a number.

myVar = myVar * 5;

will multiply myVar by 5. This can be rewritten as:

myVar *= 5;*/
//Convert the assignments for a, b, and c to use the *= operator.
/*a should equal 25
b should equal 36
c should equal 46
You should use the *= operator for each variable
Do not modify the code above the line*/
var a = 5;
var b = 12;
var c = 4.6;

// Only modify code below this line

a = a * 5;
b = 3 * b;
c = c * 10;
a *= 5;
b *= 3;
c *= 10;
```
## exercise20 
```js
/*The /= operator divides a variable by another number.

myVar = myVar / 5;

Will divide myVar by 5. This can be rewritten as:

myVar /= 5;*/
//Convert the assignments for a, b, and c to use the /= operator.
/*a should equal 4
b should equal 27
c should equal 3
You should use the /= operator for each variable
Do not modify the code above the line*/
var a = 48;
var b = 108;
var c = 33;

// Only modify code below this line

a = a / 12;
b = b / 4;
c = c / 11;
a /= 12;
b /= 4;
c /= 11;
```
## exercise21 
```js
/*Previously we have used the code

var myName = "your name";

"your name" is called a string literal. It is a string because it is a series of zero or more characters enclosed in single or double quotes.*/
//Create two new string variables: myFirstName and myLastName and assign them the values of your first and last name, respectively.
/*myFirstName should be a string with at least one character in it.
myLastName should be a string with at least one character in it.*/
// Example
var firstName = "Alan";
var lastName = "Turing";

// Only change code below this line
var myFirstName = "Fazilet";
var myLastName = "Kosure";
```
## exercise22 
```js
/*When you are defining a string you must start and end with a single or double quote. What happens when you need a literal quote: " or ' inside of your string?

In JavaScript, you can escape a quote from considering it as an end of string quote by placing a backslash (\) in front of the quote.

var sampleStr = "Alan said, \"Peter is learning JavaScript\".";

This signals to JavaScript that the following quote is not the end of the string, but should instead appear inside the string. So if you were to print this to the console, you would get:

Alan said, "Peter is learning JavaScript".*/
//Use backslashes to assign a string to the myStr variable so that if you were to print it to the console, you would see:
/*You should use two double quotes (") and four escaped double quotes (\").
Variable myStr should contain the string: I am a "double quoted" string inside "double quotes".*/
var myStr = "I am a \"double quoted\" string inside \"double quotes\"."; // Change this line
```
## exercise23 
```js
/*String values in JavaScript may be written with single or double quotes, as long as you start and end with the same type of quote. Unlike some other programming languages, single and double quotes work the same in JavaScript.

doubleQuoteStr = "This is a string"; 
singleQuoteStr = 'This is also a string';
The reason why you might want to use one type of quote over the other is if you want to use both in a string. This might happen if you want to save a conversation in a string and have the conversation in quotes. Another use for it would be saving an <a> tag with various attributes in quotes, all within a string.

conversation = 'Finn exclaims to Jake, "Algebraic!"';
However, this becomes a problem if you need to use the outermost quotes within it. Remember, a string has the same kind of quote at the beginning and end. But if you have that same quote somewhere in the middle, the string will stop early and throw an error.

goodStr = 'Jake asks Finn, "Hey, let\'s go on an adventure?"'; 
badStr = 'Finn responds, "Let's go!"'; // Throws an error
In the goodStr above, you can use both quotes safely by using the backslash \ as an escape character.

Note
The backslash \ should not be be confused with the forward slash /. They do not do the same thing.*/
//Change the provided string to a string with single quotes at the beginning and end and no escape characters.

/*Right now, the <a> tag in the string uses double quotes everywhere. You will need to change the outer quotes to single quotes so you can remove the escape characters.*/
/*Remove all the backslashes (\)
You should have two single quotes ' and four double quotes "*/
var myStr = '<a href="http://www.example.com" target="_blank">Link</a>';
```
## exercise24 
```js
/*Quotes are not the only characters that can be escaped inside a string. There are two reasons to use escaping characters: First is to allow you to use characters you might not otherwise be able to type out, such as a backspace. Second is to allow you to represent multiple quotes in a string without JavaScript misinterpreting what you mean. We learned this in the previous challenge.

Code	Output
\'	single quote
\"	double quote
\\	backslash
\n	newline
\r	carriage return
\t	tab
\b	backspace
\f	form feed
Note that the backslash itself must be escaped in order to display as a backslash.*/
//Change the provided string to a string with single quotes at the beginning and end and no escape characters.

/*myStr should not contain any spaces
myStr should contain the strings FirstLine, SecondLine and ThirdLine (remember case sensitivity)
FirstLine should be followed by the newline character \n
myStr should contain a tab character \t which follows a newline character
SecondLine should be preceded by the backslash character \\
There should be a newline character between SecondLine and ThirdLine*/
var myStr = 'FirstLine\n\t\\SecondLine\nThirdLine'
```
## exercise25 
```js
/*In JavaScript, when the + operator is used with a String value, it is called the concatenation operator. You can build a new string out of other strings by concatenating them together.

Example

'My name is Alan,' + ' I concatenate.'
Note
Watch out for spaces. Concatenation does not add spaces between concatenated strings, so you'll need to add them yourself.

*/
//Build myStr from the strings "This is the start. " and "This is the end." using the + operator.

/*myStr should have a value of This is the start. This is the end.
Use the + operator to build myStr*/
// Example
var ourStr = "I come first. " + "I come second.";

// Only change code below this line

var myStr =  "This is the start. " + "This is the end.";
```
## exercise26 
```js
/*We can also use the += operator to concatenate a string onto the end of an existing string variable. This can be very helpful to break a long string over several lines.

Note
Watch out for spaces. Concatenation does not add spaces between concatenated strings, so you'll need to add them yourself.
*/
/*Build myStr over several lines by concatenating these two strings: "This is the first sentence. " and "This is the second sentence." using the += operator. Use the += operator similar to how it is shown in the editor. Start by assigning the first string to myStr, then add on the second string.*/

/myStr should have a value of This is the first sentence. This is the second sentence.
Use the += operator to build myStr*/
// Example
var ourStr = "I come first. ";
ourStr += "I come second.";

// Only change code below this line

var myStr ="This is the first sentence. ";
myStr +="This is the second sentence.";

```
## exercise27 
```js
/*Sometimes you will need to build a string, Mad Libs style. By using the concatenation operator (+), you can insert one or more variables into a string you're building.
*/
/*Set myName to a string equal to your name and build myStr with myName between the strings "My name is " and " and I am well!"*/

/*myName should be set to a string at least 3 characters long
Passed
Use two + operators to build myStr with myName inside it*/
// Example
var ourName = "freeCodeCamp";
var ourStr = "Hello, our name is " + ourName + ", how are you?";

// Only change code below this line
var myName="Fazilet";
var myStr = "My name is " + myName +" and I am well";
```
## exercise28 
```js
/*Just as we can build a string over multiple lines out of string literals, we can also append variables to a string using the plus equals (+=) operator.
*/
//Set someAdjective and append it to myStr using the += operator.
/*someAdjective should be set to a string at least 3 characters long
Passed
Append someAdjective to myStr using the += operator*/
// Example
var anAdjective = "awesome!";
var ourStr = "freeCodeCamp is ";
ourStr += anAdjective;

// Only change code below this line

var someAdjective="cool and easy";
var myStr = "Learning to code is ";
myStr+=someAdjective;
```
## exercise29 
```js
/*You can find the length of a String value by writing .length after the string variable or string literal.

"Alan Peter".length; // 10
For example, if we created a variable var firstName = "Charles", we could find out how long the string "Charles" is by using the firstName.length property.
*/
//Use the .length property to count the number of characters in the lastName variable and assign it to lastNameLength..
/*lastNameLength should be equal to eight.
You should be getting the length of lastName by using .length like this: lastName.length.*/
// Example
var firstNameLength = 0;
var firstName = "Ada";

firstNameLength = firstName.length;

// Setup
var lastNameLength = 0;
var lastName = "Lovelace";

// Only change code below this line.
var lastNameLength = 8;
lastNameLength = lastName;
lastNameLength = lastName.length;
```
## exercise30 
```js
/*Bracket notation is a way to get a character at a specific index within a string.

Most modern programming languages, like JavaScript, don't start counting at 1 like humans do. They start at 0. This is referred to as Zero-based indexing.

For example, the character at index 0 in the word "Charles" is "C". So if var firstName = "Charles", you can get the value of the first letter of the string by using firstName[0].
*/
//Use bracket notation to find the first character in the lastName variable and assign it to firstLetterOfLastName.

/*Hint
Try looking at the firstLetterOfFirstName variable declaration if you get stuck.*/
// Example
var firstLetterOfFirstName = "";
var firstName = "Ada";

firstLetterOfFirstName = firstName[0];

// Setup
var firstLetterOfLastName = "";
var lastName = "Lovelace";

// Only change code below this line
firstLetterOfLastName = lastName[0];
```
## exercise31 
```js
/*In JavaScript, String values are immutable, which means that they cannot be altered once created.

For example, the following code:

var myStr = "Bob";
myStr[0] = "J";
cannot change the value of myStr to "Job", because the contents of myStr cannot be altered. Note that this does not mean that myStr cannot be changed, just that the individual characters of a string literal cannot be changed. The only way to change myStr would be to assign it with a new string, like this:

var myStr = "Bob";
myStr = "Job";*/
//Correct the assignment to myStr so it contains the string value of Hello World using the approach shown in the example above.
/*Correct the assignment to myStr so it contains the string value of Hello World using the approach shown in the example above.*/
/ Setup
var myStr = "Jello World";

// Only change code below this line
myStr = "Hello World"; // Fix Me
```
## exercise32 
```js
/*You can also use bracket notation to get the character at other positions within a string.

Remember that computers start counting at 0, so the first character is actually the zeroth character.

Let's try to set thirdLetterOfLastName to equal the third letter of the lastName variable using bracket notation.*/
//Try looking at the secondLetterOfFirstName variable declaration if you get stuck.
/*The thirdLetterOfLastName variable should have the value of v.
You should use bracket notation.*/
// Example
var firstName = "Ada";
var secondLetterOfFirstName = firstName[1];

// Setup
var lastName = "Lovelace";

// Only change code below this line.
var thirdLetterOfLastName = lastName[2];
```
## exercise33 
```js
/*In order to get the last letter of a string, you can subtract one from the string's length.

For example, if var firstName = "Charles", you can get the value of the last letter of the string by using firstName[firstName.length - 1].*/
//Use bracket notation to find the last character in the lastName variable.
/*Try looking at the lastLetterOfFirstName variable declaration if you get stuck.lastLetterOfLastName should be "e".
You have to use .length to get the last letter.*/
// Example
var firstName = "Ada";
var lastLetterOfFirstName = firstName[firstName.length - 1];

// Setup
var lastName = "Lovelace";

// Only change code below this line.
var lastLetterOfLastName = lastName[lastName.length -1];
```
## exercise34 
```js
/*You can use the same principle we just used to retrieve the last character in a string to retrieve the Nth-to-last character.

For example, you can get the value of the third-to-last letter of the var firstName = "Charles" string by using firstName[firstName.length - 3]*/
//Use bracket notation to find the second-to-last character in the lastName string.
/*Try looking at the thirdToLastLetterOfFirstName variable declaration if you get stuck.secondToLastLetterOfLastName should be "c".
Passed
You have to use .length to get the second last letter.*/
// Example
var firstName = "Ada";
var thirdToLastLetterOfFirstName = firstName[firstName.length - 3];

// Setup
var lastName = "Lovelace";

// Only change code below this line
var secondToLastLetterOfLastName = lastName[lastName.length -2];
```
## exercise35 
```js
/*We will now use our knowledge of strings to build a "Mad Libs" style word game we're calling "Word Blanks". You will create an (optionally humorous) "Fill in the Blanks" style sentence.

In a "Mad Libs" game, you are provided sentences with some missing words, like nouns, verbs, adjectives and adverbs. You then fill in the missing pieces with words of your choice in a way that the completed sentence makes sense.

Consider this sentence - "It was really ____, and we ____ ourselves ____". This sentence has three missing pieces- an adjective, a verb and an adverb, and we can add words of our choice to complete it. We can then assign the completed sentence to a variable as follows:

var sentence = "It was really" + "hot" + ", and we" + "laughed" + "ourselves" + "silly.";
*/
//Use bracket notation to find the second-to-last character in the lastName string.
/*wordBlanks("","","","") should return a string.
Passed
wordBlanks("dog", "big", "ran", "quickly") should contain all of the passed in words separated by non-word characters (and any additional words in your madlib).
Passed
wordBlanks("cat", "little", "hit", "slowly") should contain all of the passed in words separated by non-word characters (and any additional words in your madlib).*/
function wordBlanks(myNoun, myAdjective, myVerb, myAdverb) {
  // Your code below this line
  var result = "";
  result= "My "+myNoun+" is "+myAdjective+" and it "+myVerb+" "+myAdverb+".";
   result=`My ${myNoun} is ${myAdjective} and it ${myVerb} ${myAdverb}.`;

  // Your code above this line
  return result;
}

// Change the words here to test your function
wordBlanks("cat", "little", "hit", "slowly");
```
## exercise36 
```js
/*With JavaScript array variables, we can store several pieces of data in one place.

You start an array declaration with an opening square bracket, end it with a closing square bracket, and put a comma between each entry, like this:

var sandwich = ["peanut butter", "jelly", "bread"].
*/
//Modify the new array myArray so that it contains both a string and a number (in that order).
/*myArray should be an array.
The first item in myArray should be a string.
The second item in myArray should be a number.*/
function wordBlanks(myNoun, myAdjective, myVerb, myAdverb) {
  // Example
var ourArray = ["John", 23];

// Only change code below this line.
var myArray = ["Fazilet", 34];
```
## exercise37 
```js
/*You can also nest arrays within other arrays, like this: [["Bulls", 23], ["White Sox", 45]]. This is also called a Multi-dimensional Array.
*/
//Create a nested array called myArray.
/*myArray should have at least one array nested within another array.*/
  // Example
var ourArray = [["the universe", 42], ["everything", 101010]];

// Only change code below this line.
var myArray = [["Bulls", 23], ["White Sox", 45]];

```
## exercise38 
```js
/*We can access the data inside arrays using indexes.

Array indexes are written in the same bracket notation that strings use, except that instead of specifying a character, they are specifying an entry in the array. Like strings, arrays use zero-based indexing, so the first element in an array is element 0.

Example

var array = [50,60,70];
array[0]; // equals 50
var data = array[1]; // equals 60
Note
There shouldn't be any spaces between the array name and the square brackets, like array [0]. Although JavaScript is able to process this correctly, this may confuse other programmers reading your code.

*/
//Create a variable called myData and set it to equal the first value of myArray using bracket notation.
/*The variable myData should equal the first value of myArray.
The data in variable myArray should be accessed using bracket notation.*/
 // Example
var ourArray = [50,60,70];
var ourData = ourArray[0]; // equals 50

// Setup
var myArray = [50,60,70];

// Only change code below this line.
var myData = myArray[0];

```
## exercise39 
```js
/*Unlike strings, the entries of arrays are mutable and can be changed freely.

Example

var ourArray = [50,40,30];
ourArray[0] = 15; // equals [15,40,30]
Note
There shouldn't be any spaces between the array name and the square brackets, like array [0]. Although JavaScript is able to process this correctly, this may confuse other programmers reading your code.
*/
//Modify the data stored at index 0 of myArray to a value of 45.
/*myArray should now be [45,64,99].
Passed
You should be using correct index to modify the value in myArray.*/
 // Example
var ourArray = [18,64,99];
ourArray[1] = 45; // ourArray now equals [18,45,99].

// Setup
var myArray = [18,64,99];

// Only change code below this line.
myArray[0] = 45;
```
## exercise40 
```js
/*One way to think of a multi-dimensional array, is as an array of arrays. When you use brackets to access your array, the first set of brackets refers to the entries in the outer-most (the first level) array, and each additional pair of brackets refers to the next level of entries inside.

Example

var arr = [
  [1,2,3],
  [4,5,6],
  [7,8,9],
  [[10,11,12], 13, 14]
];
arr[3]; // equals [[10,11,12], 13, 14]
arr[3][0]; // equals [10,11,12]
arr[3][0][1]; // equals 11
Note
There shouldn't be any spaces between the array name and the square brackets, like array [0][0] and even this array [0] [0] is not allowed. Although JavaScript is able to process this correctly, this may confuse other programmers reading your code.
*/
//Using bracket notation select an element from myArray such that myData is equal to 8.
/*myData should be equal to 8.
You should be using bracket notation to read the correct value from myArray.*/
// Setup
var myArray = [[1,2,3], [4,5,6], [7,8,9], [[10,11,12], 13, 14]];

// Only change code below this line.
var myData = myArray[2][1];

```
## exercise41 
```js
/*An easy way to append data to the end of an array is via the push() function.

.push() takes one or more parameters and "pushes" them onto the end of the array.

var arr = [1,2,3];
arr.push(4);
// arr is now [1,2,3,4]
*/
//Push ["dog", 3] onto the end of the myArray variable.
/*myArray should now equal [["John", 23], ["cat", 2], ["dog", 3]].*/
// Example
var ourArray = ["Stimpson", "J", "cat"];
ourArray.push(["happy", "joy"]); 
// ourArray now equals ["Stimpson", "J", "cat", ["happy", "joy"]]

// Setup
var myArray = [["John", 23], ["cat", 2]];

// Only change code below this line.

myArray.push (["dog", 3]);

```
## exercise42 
```js
/*Another way to change the data in an array is with the .pop() function.

.pop() is used to "pop" a value off of the end of an array. We can store this "popped off" value by assigning it to a variable. In other words, .pop() removes the last element from an array and returns that element.

Any type of entry can be "popped" off of an array - numbers, strings, even nested arrays.

var threeArr = [1, 4, 6];
var oneDown = threeArr.pop();
console.log(oneDown); // Returns 6
console.log(threeArr); // Returns [1, 4]
*/
//Use the .pop() function to remove the last item from myArray, assigning the "popped off" value to removedFromMyArray.
/*myArray should only contain [["John", 23]].
Use pop() on myArray
removedFromMyArray should only contain ["cat", 2].*/
// Example
var ourArray = [1,2,3];
var removedFromOurArray = ourArray.pop(); 
// removedFromOurArray now equals 3, and ourArray now equals [1,2]

// Setup
var myArray = [["John", 23], ["cat", 2]];

// Only change code below this line.
var removedFromMyArray = myArray.pop();

```
## exercise43 
```js
/*pop() always removes the last element of an array. What if you want to remove the first?

That's where .shift() comes in. It works just like .pop(), except it removes the first element instead of the last.
*/
//Use the .shift() function to remove the first item from myArray, assigning the "shifted off" value to removedFromMyArray.
/*myArray should now equal [["dog", 3]].
removedFromMyArray should contain ["John", 23].*/
// Example
var ourArray = ["Stimpson", "J", ["cat"]];
var removedFromOurArray = ourArray.shift();
// removedFromOurArray now equals "Stimpson" and ourArray now equals ["J", ["cat"]].

// Setup
var myArray = [["John", 23], ["dog", 3]];

// Only change code below this line.
var removedFromMyArray = myArray.shift();

```
## exercise44 
```js
/*Create a shopping list in the variable myList. The list should be a multi-dimensional array containing several sub-arrays.

The first element in each sub-array should contain a string with the name of the item. The second element should be a number representing the quantity i.e.

["Chocolate Bar", 15]
*/
//There should be at least 5 sub-arrays in the list.
/*myList should be an array
The first elements in each of your sub-arrays must all be strings
The second elements in each of your sub-arrays must all be numbers
You must have at least 5 items in your list*/
// Example
var ourArray = ["Stimpson", "J", "cat"];
ourArray.shift(); // ourArray now equals ["J", "cat"]
ourArray.unshift("Happy"); 
// ourArray now equals ["Happy", "J", "cat"]

// Setup
var myArray = [["John", 23], ["dog", 3]];
myArray.shift();

// Only change code below this line.
myArray.unshift( ["Paul",35]);

```
## exercise45 
```js
/*Not only can you shift elements off of the beginning of an array, you can also unshift elements to the beginning of an array i.e. add elements in front of the array.

.unshift() works exactly like .push(), but instead of adding the element at the end of the array, unshift() adds the element at the beginning of the array.
*/
//Add ["Paul",35] to the beginning of the myArray variable using unshift().
/*myArray should now have [["Paul", 35], ["dog", 3]].*/
// Example
var ourArray = ["Stimpson", "J", "cat"];
ourArray.shift(); // ourArray now equals ["J", "cat"]
ourArray.unshift("Happy"); 
// ourArray now equals ["Happy", "J", "cat"]

// Setup
var myArray = [["John", 23], ["dog", 3]];
myArray.shift();

// Only change code below this line.
myArray.unshift( ["Paul",35]);

```
## exercise46 
```js
/*Create a shopping list in the variable myList. The list should be a multi-dimensional array containing several sub-arrays.

The first element in each sub-array should contain a string with the name of the item. The second element should be a number representing the quantity i.e.

["Chocolate Bar", 15]
*/
//There should be at least 5 sub-arrays in the list.
/*myList should be an array
Passed
The first elements in each of your sub-arrays must all be strings
Passed
The second elements in each of your sub-arrays must all be numbers
Passed
You must have at least 5 items in your list.*/
var myList = [["dog",5], ["cat",1],  ["bird",2], ["monkey",3], ["sparrow",4]];

```

## exercise48 
```js
/*Parameters are variables that act as placeholders for the values that are to be input to a function when it is called. When a function is defined, it is typically defined along with one or more parameters. The actual values that are input (or "passed") into a function when it is called are known as arguments.

Here is a function with two parameters, param1 and param2:

function testFun(param1, param2) {
  console.log(param1, param2);
}
Then we can call testFun:

testFun("Hello", "World");

We have passed two arguments, "Hello" and "World". Inside the function, param1 will equal "Hello" and param2 will equal "World". Note that you could call testFun again with different arguments and the parameters would take on the value of the new arguments.
*/
//Create a function called functionWithArgs that accepts two arguments and outputs their sum to the dev console.Call the function with two numbers as arguments.
/*functionWithArgs should be a function
Passed
functionWithArgs(1,2) should output 3
Passed
functionWithArgs(7,9) should output 16
Passed
Call functionWithArgs with two numbers after you define it.*/
// Example
function ourFunctionWithArgs(a, b) {
  console.log(a - b);
}
ourFunctionWithArgs(10, 5); // Outputs 5

// Only change code below this line.
function functionWithArgs(a, b) {
  console.log(a+b);
}
functionWithArgs(1,2);
functionWithArgs(7,9);

}
```
## exercise47 
```js
/*In JavaScript, we can divide up our code into reusable parts called functions.

Here's an example of a function:

function functionName() {
  console.log("Hello World");
}
You can call or invoke this function by using its name followed by parentheses, like this:

functionName();

Each time the function is called it will print out the message "Hello World" on the dev console. All of the code between the curly braces will be executed every time the function is called.
*/
//Create a function called reusableFunction which prints "Hi World" to the dev console.Call the function.
/*reusableFunction should be a function
reusableFunction should output "Hi World" to the dev console
Call reusableFunction after you define it*/
// Example
function ourReusableFunction() {
  console.log("Heyya, World");
}

ourReusableFunction();

// Only change code below this line
function reusableFunction() {
    console.log("Hi World");
}
reusableFunction();

```
## exercise49
```js
/*In JavaScript, scope refers to the visibility of variables. Variables which are defined outside of a function block have Global scope. This means, they can be seen everywhere in your JavaScript code.

Variables which are used without the var keyword are automatically created in the global scope. This can create unintended consequences elsewhere in your code or when running a function again. You should always declare your variables with var.
*/
//Using var, declare a global variable myGlobal outside of any function. Initialize it with a value of 10.

//Inside function fun1, assign 5 to oopsGlobal without using the var keyword.
/*fmyGlobal should be defined
myGlobal should have a value of 10
myGlobal should be declared using the var keyword
oopsGlobal should be a global variable and have a value of 5*/
var myGlobal = 10;

function fun1() {
  // Assign 5 to oopsGlobal Here
  oopsGlobal=5;
}

// Only change code above this line
function fun2() {
  var output = "";
  if (typeof myGlobal != "undefined") {
    output += "myGlobal: " + myGlobal;
  }
  if (typeof oopsGlobal != "undefined") {
    output += " oopsGlobal: " + oopsGlobal;
  }
  console.log(output);
}
```
## exercise50
```js
/*Variables which are declared within a function, as well as the function parameters have local scope. That means, they are only visible within that function.

Here is a function myTest with a local variable called loc.

function myTest() {
  var loc = "foo";
  console.log(loc);
}
myTest(); // logs "foo"
console.log(loc); // loc is not defined
loc is not defined outside of the function.
*/
//No global myVar variable Passed
//Add a local myVar variable
function myLocalScope() {
  'use strict'; // you shouldn't need to edit this line
 var myVar = 5;
  console.log(myVar);
}
myLocalScope();
```
## exercise51
```js
/*t is possible to have both local and global variables with the same name. When you do this, the local variable takes precedence over the global variable.

In this example:

var someVar = "Hat";
function myFun() {
  var someVar = "Head";
  return someVar;
}
*/
//Add a local variable to myOutfit function to override the value of outerWear with "sweater".
/*Do not change the value of the global outerWear
myOutfit should return "sweater"
Do not change the return statement*/
// Setup
var outerWear = "T-Shirt";

function myOutfit() {
  // Only change code below this line
  
 var outerWear = "sweater";
  
  // Only change code above this line
  return outerWear;
}

myOutfit();
```
## exercise52
```js
/*We can pass values into a function with arguments. You can use a return statement to send a value back out of a function.

Example

function plusThree(num) {
  return num + 3;
}
var answer = plusThree(5); // 8
plusThree takes an argument for num and returns a value equal to num + 3.
*/
//Create a function timesFive that accepts one argument, multiplies it by 5, and returns the new value. See the last line in the editor for an example of how you can test your timesFive function.
/*timesFive should be a function
timesFive(5) should return 25
timesFive(2) should return 10
timesFive(0) should return 0*/
// Example
function minusSeven(num) {
  return num - 7;
}

// Only change code below this line
function timesFive(num) {
  return num * 5;
}
timesFive(5);
timesFive(2);
timesFive(0);
```
## exercise53
```js
/*A function can include the return statement but it does not have to. In the case that the function doesn't have a return statement, when you call it, the function processes the inner code but the returned value is undefined.

Example

var sum = 0;
function addSum(num) {
  sum = sum + num;
}
var returnedValue = addSum(3); // sum will be modified but returned value is undefined
addSum is a function without a return statement. The function will change the global sum variable but the returned value of the function is undefined
*/
//Create a function addFive without any arguments. This function adds 5 to the sum variable, but its returned value is undefined.
/*addFive should be a function
sum should be equal to 8
Returned value from addFive should be undefined
Inside of your functions, add 5 to the sum variable*/
// Example
var sum = 0;
function addThree() {
  sum = sum + 3;
}

// Only change code below this line
var sum=8;
function addFive(){
  sum = sum +5;
}


// Only change code above this line
var returnedValue = addFive();
```
## exercise54
```js
/*If you'll recall from our discussion of Storing Values with the Assignment Operator, everything to the right of the equal sign is resolved before the value is assigned. This means we can take the return value of a function and assign it to a variable.

Assume we have pre-defined a function sum which adds two numbers together, then:

ourSum = sum(5, 12);

will call sum function, which returns a value of 17 and assigns it to ourSum variable.


*/
//Call the processArg function with an argument of 7 and assign its return value to the variable processed
/*processed should have a value of 2
You should assign processArg to processed*/
// Example
var changed = 0;

function change(num) {
  return (num + 5) / 3;
}

changed = change(10);

// Setup
var processed = 0;

function processArg(num) {
  return (num + 3) / 5;
}

// Only change code below this line
 processArg(7);
var processed=processArg(7);

```
## exercise55
```js
/*In Computer Science a queue is an abstract Data Structure where items are kept in order. New items can be added at the back of the queue and old items are taken off from the front of the queue.

Write a function nextInLine which takes an array (arr) and a number (item) as arguments.
*/
//Add the number to the end of the array, then remove the first element of the array.
//The nextInLine function should then return the element that was removed.
/*nextInLine([], 5) should return a number.
nextInLine([], 1) should return 1
nextInLine([2], 1) should return 2
nextInLine([5,6,7,8,9], 1) should return 5
After nextInLine(testArr, 10), testArr[4] should be 10*/
function nextInLine(arr, item) {
  // Your code here

  var queue = arr.push(item);

  var removeItem = arr.shift();

  return removeItem;  // Change this line
}

// Test Setup
var testArr = [1,2,3,4,5];

// Display Code
console.log("Before: " + JSON.stringify(testArr));
console.log(nextInLine(testArr, 6)); // Modify this line to test
console.log("After: " + JSON.stringify(testArr));

  nextInLine([], 5);
  nextInLine([], 1);
  nextInLine([2], 1);//2
  nextInLine([5,6,7,8,9], 1);//5
   nextInLine(testArr, 10), testArr[4];//10
```
## exercise56
```js
/*Another data type is the Boolean. Booleans may only be one of two values: true or false. They are basically little on-off switches, where true is "on" and false is "off." These two states are mutually exclusive.Note
Boolean values are never written with quotes. The strings "true" and "false" are not Boolean and have no special meaning in JavaScript.
*/
//Add the number to the end of the array, then remove the first element of the array.
//Modify the welcomeToBooleans function so that it returns true instead of false when the run button is clicked.
/*The welcomeToBooleans() function should return a boolean (true/false) value.
welcomeToBooleans() should return true.*/
function welcomeToBooleans() {

// Only change code below this line.

return true; // Change this line

// Only change code above this line.
}
welcomeToBooleans();
```
## exercise57
```js
/*If statements are used to make decisions in code. The keyword if tells JavaScript to execute the code in the curly braces under certain conditions, defined in the parentheses. These conditions are known as Boolean conditions and they may only be true or false.

When the condition evaluates to true, the program executes the statement inside the curly braces. When the Boolean condition evaluates to false, the statement inside the curly braces will not execute.

Pseudocode

if (condition is true) {
  statement is executed
}
Example

function test (myCondition) {
  if (myCondition) {
     return "It was true";
  }
  return "It was false";
}
test(true); // returns "It was true"
test(false); // returns "It was false"
When test is called with a value of true, the if statement evaluates myCondition to see if it is true or not. Since it is true, the function returns "It was true". When we call test with a value of false, myCondition is not true and the statement in the curly braces is not executed and the function returns "It was false".
*/
//Create an if statement inside the function to return "Yes, that was true" if the parameter wasThatTrue is true and return "No, that was false" otherwise.
/*trueOrFalse should be a function
trueOrFalse(true) should return a string
trueOrFalse(false) should return a string
trueOrFalse(true) should return "Yes, that was true"
trueOrFalse(false) should return "No, that was false"*/
// Example
function ourTrueOrFalse(isItTrue) {
  if (isItTrue) { 
    return "Yes, it's true";
  }
  return "No, it's false";
}

// Setup
function trueOrFalse(wasThatTrue) {

  // Only change code below this line.
  if (wasThatTrue){
      return  "Yes, that was true";
  }

  return "No, that was false";
  
  // Only change code above this line.

}

// Change this value to test
trueOrFalse(true);
trueOrFalse(false);
```
## exercise58
```js
/*There are many Comparison Operators in JavaScript. All of these operators return a boolean true or false value.

The most basic operator is the equality operator ==. The equality operator compares two values and returns true if they're equivalent or false if they are not. Note that equality is different from assignment (=), which assigns the value at the right of the operator to a variable in the left.

function equalityTest(myVal) {
  if (myVal == 10) {
     return "Equal";
  }
  return "Not Equal";
}
If myVal is equal to 10, the equality operator returns true, so the code in the curly braces will execute, and the function will return "Equal". Otherwise, the function will return "Not Equal".

In order for JavaScript to compare two different data types (for example, numbers and strings), it must convert one type to another. This is known as "Type Coercion". Once it does, however, it can compare terms as follows:

1 == 1 // true
1 == 2 // false
1 == '1' // true
"3" == 3 // true
*/
//Add the equality operator to the indicated line so that the function will return "Equal" when val is equivalent to 12
/*testEqual(10) should return "Not Equal"
Passed
testEqual(12) should return "Equal"
Passed
testEqual("12") should return "Equal"
Passed
You should use the == operator*/
// Setup
function testEqual(val) {
  if (val==12) { // Change this line
    return "Equal";
  }
  return "Not Equal";
}

// Change this value to test
testEqual(12);
```
## exercise59
```js
/*Strict equality (===) is the counterpart to the equality operator (==). However, unlike the equality operator, which attempts to convert both values being compared to a common type, the strict equality operator does not perform a type conversion.

If the values being compared have different types, they are considered unequal, and the strict equality operator will return false.

Examples

3 === 3 // true
3 === '3' // false
In the second example, 3 is a Number type and '3' is a String type.


*/
//Use the strict equality operator in the if statement so the function will return "Equal" when val is strictly equal to 7
/*testStrict(10) should return "Not Equal"
testStrict(7) should return "Equal"
testStrict("7") should return "Not Equal"
You should use the === operator*/
// Setup
function testStrict(val) {
  if (val===7) { // Change this line
    return "Equal";
  }
  return "Not Equal";
}

// Change this value to test
testStrict(7);
```
## exercise60
```js
/*In the last two challenges, we learned about the equality operator (==) and the strict equality operator (===). Let's do a quick review and practice using these operators some more.

If the values being compared are not of the same type, the equality operator will perform a type conversion, and then evaluate the values. However, the strict equality operator will compare both the data type and value as-is, without converting one type to the other.

Examples

3 == '3' // returns true because JavaScript performs type conversion from string to number
3 === '3' // returns false because the types are different and type conversion is not performed
Note
In JavaScript, you can determine the type of a variable or a value with the typeof operator, as follows:

typeof 3 // returns 'number'
typeof '3' // returns 'string'
*/
//The compareEquality function in the editor compares two values using the equality operator. Modify the function so that it returns "Equal" only when the values are strictly equal.
/*compareEquality(10, "10") should return "Not Equal"
Passed
compareEquality("20", 20) should return "Not Equal"
Passed
You should use the === operator*/
// Setup
function compareEquality(a, b) {
  if ("20" === 20) { // Change this line
    return "Equal";
  }
  return "Not Equal";
}

// Change this value to test
compareEquality("20",20 );
```
## exercise61
```js
/*The inequality operator (!=) is the opposite of the equality operator. It means "Not Equal" and returns false where equality would return true and vice versa. Like the equality operator, the inequality operator will convert data types of values while comparing.

Examples

1 != 2 // true
1 != "1" // false
1 != '1' // false
1 != true // false
0 != false // false
*/
//Add the inequality operator != in the if statement so that the function will return "Not Equal" when val is not equivalent to 99
/*testNotEqual(99) should return "Equal"
testNotEqual("99") should return "Equal"
testNotEqual(12) should return "Not Equal"
testNotEqual("12") should return "Not Equal"
testNotEqual("bob") should return "Not Equal"
You should use the != operator*/
// Setup
function testNotEqual(val) {
  if (val!=99) { // Change this line
    return "Not Equal";
  }
  return "Equal";
}

// Change this value to test
testNotEqual(10);
```
## exercise62
```js
/*The strict inequality operator (!==) is the logical opposite of the strict equality operator. It means "Strictly Not Equal" and returns false where strict equality would return true and vice versa. Strict inequality will not convert data types.

Examples

3 !== 3 // false
3 !== '3' // true
4 !== 3 // true
*/
//Add the strict inequality operator to the if statement so the function will return "Not Equal" when val is not strictly equal to 17
/*testStrictNotEqual(17) should return "Equal"
testStrictNotEqual("17") should return "Not Equal"
testStrictNotEqual(12) should return "Not Equal"
testStrictNotEqual("bob") should return "Not Equal"
You should use the !== operator*/
// Setup
function testStrictNotEqual(val) {
  // Only Change Code Below this Line
  
  if (val !==17) {

  // Only Change Code Above this Line

    return "Not Equal";
  }
  return "Equal";
}

// Change this value to test
testStrictNotEqual(10);
```
## exercise63
```js
/*The greater than operator (>) compares the values of two numbers. If the number to the left is greater than the number to the right, it returns true. Otherwise, it returns false.

Like the equality operator, greater than operator will convert data types of values while comparing.

Examples

5 > 3 // true
7 > '3' // true
2 > 3 // false
'1' > 9 // false
*/
//Add the greater than operator to the indicated lines so that the return statements make sense.
/*testGreaterThan(0) should return "10 or Under"
testGreaterThan(10) should return "10 or Under"
testGreaterThan(11) should return "Over 10"
testGreaterThan(99) should return "Over 10"
testGreaterThan(100) should return "Over 10"
testGreaterThan(101) should return "Over 100"
testGreaterThan(150) should return "Over 100"
You should use the > operator at least twice*/
function testGreaterThan(val) {
  if (val > 100) {  // Change this line
    return "Over 100";
  }
  
  if (val >10) {  // Change this line
    return "Over 10";
  }

  return "10 or Under";
}

// Change this value to test
testGreaterThan(10);
```
## exercise64
```js
/*The greater than or equal to operator (>=) compares the values of two numbers. If the number to the left is greater than or equal to the number to the right, it returns true. Otherwise, it returns false.

Like the equality operator, greater than or equal to operator will convert data types while comparing.

Examples

6 >= 6 // true
7 >= '3' // true
2 >= 3 // false
'7' >= 9 // false
*/
//Add the greater than or equal to operator to the indicated lines so that the return statements make sense.
/*testGreaterOrEqual(0) should return "Less than 10"
testGreaterOrEqual(9) should return "Less than 10"
testGreaterOrEqual(10) should return "10 or Over"
testGreaterOrEqual(11) should return "10 or Over"
testGreaterOrEqual(19) should return "10 or Over"
testGreaterOrEqual(100) should return "20 or Over"
testGreaterOrEqual(21) should return "20 or Over"
You should use the >= operator at least twice*/

function testGreaterOrEqual(val) {
  if (val>=20) {  // Change this line
    return "20 or Over";
  }
  
  if (val>=10) {  // Change this line
    return "10 or Over";
  }

  return "Less than 10";
}

// Change this value to test
testGreaterOrEqual(10);
```
## exercise65
```js
/*The less than operator (<) compares the values of two numbers. If the number to the left is less than the number to the right, it returns true. Otherwise, it returns false. Like the equality operator, less than operator converts data types while comparing.

Examples

2 < 5 // true
'3' < 7 // true
5 < 5 // false
3 < 2 // false
'8' < 4 // false
*/
//Add the less than operator to the indicated lines so that the return statements make sense.
/*testLessThan(0) should return "Under 25"
testLessThan(24) should return "Under 25"
testLessThan(25) should return "Under 55"
testLessThan(54) should return "Under 55"
testLessThan(55) should return "55 or Over"
testLessThan(99) should return "55 or Over"
You should use the < operator at least twice*/

function testLessThan(val) {
  if (val<25) {  // Change this line
    return "Under 25";
  }
  
  if (val<55) {  // Change this line
    return "Under 55";
  }

  return "55 or Over";
}

// Change this value to test
testLessThan(10);
```
## exercise66
```js
/*The less than or equal to operator (<=) compares the values of two numbers. If the number to the left is less than or equal to the number to the right, it returns true. If the number on the left is greater than the number on the right, it returns false. Like the equality operator, less than or equal to converts data types.

Examples

4 <= 5 // true
'7' <= 7 // true
5 <= 5 // true
3 <= 2 // false
'8' <= 4 // false
*/
//Add the less than or equal to operator to the indicated lines so that the return statements make sense
/*testLessOrEqual(0) should return "Smaller Than or Equal to 12"
testLessOrEqual(11) should return "Smaller Than or Equal to 12"
testLessOrEqual(12) should return "Smaller Than or Equal to 12"
testLessOrEqual(23) should return "Smaller Than or Equal to 24"
testLessOrEqual(24) should return "Smaller Than or Equal to 24"
testLessOrEqual(25) should return "More Than 24"
testLessOrEqual(55) should return "More Than 24"
You should use the <= operator at least twice*/

function testLessOrEqual(val) {
  if (val<=12) {  // Change this line
    return "Smaller Than or Equal to 12";
  }
  
  if (val<=24) {  // Change this line
    return "Smaller Than or Equal to 24";
  }

  return "More Than 24";
}

// Change this value to test
testLessOrEqual(10);

```
## exercise67
```js
/*Sometimes you will need to test more than one thing at a time. The logical and operator (&&) returns true if and only if the operands to the left and right of it are true.

The same effect could be achieved by nesting an if statement inside another if:

if (num > 5) {
  if (num < 10) {
    return "Yes";
  }
}
return "No";
will only return "Yes" if num is greater than 5 and less than 10. The same logic can be written as:

if (num > 5 && num < 10) {
  return "Yes";
}
return "No";
*/
//Combine the two if statements into one statement which will return "Yes" if val is less than or equal to 50 and greater than or equal to 25. Otherwise, will return "No".
/*You should use the && operator once
Passed
You should only have one if statement
Passed
testLogicalAnd(0) should return "No"
Passed
testLogicalAnd(24) should return "No"
Passed
testLogicalAnd(25) should return "Yes"
Passed
testLogicalAnd(30) should return "Yes"
Passed
testLogicalAnd(50) should return "Yes"
Passed
testLogicalAnd(51) should return "No"
Passed
testLogicalAnd(75) should return "No"
Passed
testLogicalAnd(80) should return "No"*/

function testLogicalAnd(val) {
  // Only change code below this line

  if (val>=25 && val<=50) {
    
      return "Yes";
    
  }

  // Only change code above this line
  return "No";
}

// Change this value to test
testLogicalAnd(10);

```
## exercise68
```js
/*The logical or operator (||) returns true if either of the operands is true. Otherwise, it returns false.

The logical or operator is composed of two pipe symbols (|). This can typically be found between your Backspace and Enter keys.

The pattern below should look familiar from prior waypoints:

if (num > 10) {
  return "No";
}
if (num < 5) {
  return "No";
}
return "Yes";
will return "Yes" only if num is between 5 and 10 (5 and 10 included). The same logic can be written as:

if (num > 10 || num < 5) {
  return "No";
}
return "Yes";

*/
//Combine the two if statements into one statement which returns "Outside" if val is not between 10 and 20, inclusive. Otherwise, return "Inside".
/*You should use the || operator once
You should only have one if statement
testLogicalOr(0) should return "Outside"
testLogicalOr(9) should return "Outside"
testLogicalOr(10) should return "Inside"
testLogicalOr(15) should return "Inside"
testLogicalOr(19) should return "Inside"
testLogicalOr(20) should return "Inside"
testLogicalOr(21) should return "Outside"
testLogicalOr(25) should return "Outside"*/

function testLogicalOr(val) {
  // Only change code below this line

  if (val>20 || val<10) {
    return "Outside";
 
  }

  // Only change code above this line
  return "Inside";
}

// Change this value to test
testLogicalOr(15);

```
## exercise69
```js
/*When a condition for an if statement is true, the block of code following it is executed. What about when that condition is false? Normally nothing would happen. With an else statement, an alternate block of code can be executed.

if (num > 10) {
  return "Bigger than 10";
} else {
  return "10 or Less";
}


*/
//Combine the if statements into a single if/else statement.
/*You should only have one if statement in the editor
Passed
You should use an else statement
Passed
testElse(4) should return "5 or Smaller"
Passed
testElse(5) should return "5 or Smaller"
Passed
testElse(6) should return "Bigger than 5"
Passed
testElse(10) should return "Bigger than 5"
Passed
Do not change the code above or below the lines.*/

function testElse(val) {
  var result = "";
  // Only change code below this line
  
  if (val > 5) {
    result = "Bigger than 5";
  }
  
  else {
    result = "5 or Smaller";
  }
  
  // Only change code above this line
  return result;
}

// Change this value to test
testElse(4);

```
## exercise70
```js
/*If you have multiple conditions that need to be addressed, you can chain if statements together with else if statements.

if (num > 15) {
  return "Bigger than 15";
} else if (num < 5) {
  return "Smaller than 5";
} else {
  return "Between 5 and 15";
}
*/
//Convert the logic to use else if statements.
/*You should have at least two else statements
You should have at least two if statements
You should have closing and opening curly braces for each condition
testElseIf(0) should return "Smaller than 5"
testElseIf(5) should return "Between 5 and 10"
testElseIf(7) should return "Between 5 and 10"
testElseIf(10) should return "Between 5 and 10"
testElseIf(12) should return "Greater than 10"*/

function testElseIf(val) {
  if (val > 10) {
    return "Greater than 10";
  }
  
   else if (val < 5) {
    return "Smaller than 5";
  } else {
  
  return "Between 5 and 10";
}
}


testElseIf(5);
testElseIf(10);

```
## exercise71
```js
/*Order is important in if, else if statements.

The function is executed from top to bottom so you will want to be careful of what statement comes first.

Take these two functions as an example.

Here's the first:

function foo(x) {
  if (x < 1) {
    return "Less than one";
  } else if (x < 2) {
    return "Less than two";
  } else {
    return "Greater than or equal to two";
  }
}
And the second just switches the order of the statements:

function bar(x) {
  if (x < 2) {
    return "Less than two";
  } else if (x < 1) {
    return "Less than one";
  } else {
    return "Greater than or equal to two";
  }
}
While these two functions look nearly identical if we pass a number to both we get different outputs.

foo(0) // "Less than one"
bar(0) // "Less than two"

*/
//Change the order of logic in the function so that it will return the correct statements in all cases.
/*orderMyLogic(4) should return "Less than 5"
Passed
orderMyLogic(6) should return "Less than 10"
Passed
orderMyLogic(11) should return "Greater than or equal to 10"*/

function orderMyLogic(val) {
  if (val < 5) {
    return "Less than 5";
  } else if (val < 10) {
    return "Less than 10";
  } else {
    return "Greater than or equal to 10";
  }
}

// Change this value to test
orderMyLogic(10);
orderMyLogic(4);


```
## exercise72
```js
/*if/else statements can be chained together for complex logic. Here is pseudocode of multiple chained if / else if statements:

if (condition1) {
  statement1
} else if (condition2) {
  statement2
} else if (condition3) {
  statement3
. . .
} else {
  statementN
}
*/
//Write chained if/else if statements to fulfill the following conditions:

/*num < 5 - return "Tiny"
num < 10 - return "Small"
num < 15 - return "Medium"
num < 20 - return "Large"
num >= 20 - return "Huge"*/
/*You should have at least four else statements
You should have at least four if statements
You should have at least one return statement
testSize(0) should return "Tiny"
testSize(4) should return "Tiny"
testSize(5) should return "Small"
testSize(8) should return "Small"
testSize(10) should return "Medium"
testSize(14) should return "Medium"
testSize(15) should return "Large"
testSize(17) should return "Large"
testSize(20) should return "Huge"
testSize(25) should return "Huge"
*/

function testSize(num) {
  // Only change code below this line
  if (num<5){
     return "Tiny";
  } else if ( num<10) {
    return "Small";
  } else if (num<15){
return "Medium";
  }
  else if (num<20) {
     return "Large";
  }
  else {
    return "Huge";
  }
  
  return "Change Me";
  // Only change code above this line
}

// Change this value to test
testSize(7);
```

