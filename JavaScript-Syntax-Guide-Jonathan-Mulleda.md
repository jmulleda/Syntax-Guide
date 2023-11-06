# JavaScript Syntax Guide
#### Jonathan Mulleda
---
## JavaScript Variables
- Variables are 'containers' for storing data
- To declare a variable, use **let**, **const** and **var**
```
let a = 1; 
const PI = 3.14;
var greeting = 'Hello!'
```
- Use camel case for variable names.
- For constant variables, use uppercase.
- Variable names cannot start with a number, use letters or underscore instead.
- Specials characters and spaces are not allowed, use only alpha-numeric characters and underscores.
- Variables are case sensitive.
---
## JavaScript Comparison Statements
- Comparison statements are used to test for **true** or **false**.
- **==**	equal to
- **===**	equal value and equal type
- **!=**	not equal
- **!==**	not equal value or not equal type
- **>**	    greater than
- **<**	    less than
- **>=**	greater than or equal to
- **<=**	less than or equal to

```
let a = 10;     not to be confused with **=** which is variable assignment
a == 20;        false
a === 10;       true
a != 5;         true
a !== 5;        true
a > 5;          true
a < 5;          false
a >= 5;         true
a <= 5;         false
```
---
## JavaScript Boolean Statements
- Can only be either **true** or **false**
```
let subscriptionChecked = true; // Yes, subscribe checkbox is checked
let ageFieldChecked = false; // No, age field is not checked
```
---
## Javascript Arrays
- Arrays are used to store ordered collections
```
let countries = ["Canada", "USA", "Mexico", "Philippines"];
```
- Array elements are numbered, starting with zero
- Individual element can be accessed by its number in square brackets
```
let countries = ["Canada", "USA", "Mexico", "Philippines"];
alert(countries[0]); // Canada
alert(countries[1]); // USA
alert(countries[3]); // Philippines
```
- Total count of the elements in the array is its **length**
```
let countries = ["Canada", "USA", "Mexico", "Philippines"];
console.log(countries.length); // 4 
```
- **pop** - extracts the last element of the array and returns it
```
let countries = ["Canada", "USA", "Mexico", "Philippines"];
alert(countries.pop() ); // removes "Philippines" and alert it
```
- **push** - appends the element to the end of the array
```
let countries = ["Canada", "USA", "Mexico", "Philippines"];
countries.push("Japan");
```
---
## JavaScript Objects
- Used to store various keyed collections and more complex entities
- Store properties (key-value pairs)
- Property keys must be strings or symbols (usually strings) and values can be of any type.
```
let user = {
  name: "Jonathan",
  age: 32,
  isAdmin: true
};
```
- Access the value of the property using its key by using dot notation
```
let user = {
  name: "Jonathan",
  age: 32,
  isAdmin: true
};

// accessing property
console.log(user.name); // Jonathan
```
- Using bracket Notation
```
console.log(user["name"]); // Jonathan
```
- Method - a property containing a function declaration
```
let user = {
  name: "Jonathan",
  age: 32,
    // using function as a value
  greet: function() { 
    console.log("hello");
  }
}

user.greet(); // hello
```
---
## JavaScript Functions
- The main “building blocks” of the program
- Allow the code to be called many times without repetition
- Functions are actions, so function names are usually verbal
```
function showMessage() {
  alert("Hello Web103!");
}
```
- Functions can return a value 
```
function addNumbers(a, b) {
  let sum = a + b;
  return sum;
}
addNumbers(1, 2); // 3
```
---
## JavaScript Functions & Parameters
- Parameters (also called arguments) are used to pass arbitrary data to functions
```
function multiply(a, b) {
  return a * b;
}
let x = multiply(3, 2); 
console.log(x); // 6
```
---
## JavaScript Loops
- **for** - loops through a block of code a number of times
```
for (let i = 0; i < 5; i++) {
  console.log(i);
}
```
- **while** - loops through a block of code while a specified condition is true
```
while (i < 5) {
  console.log(i);
  i++;
}
```
- **do while** - execute the code block once, before checking if the condition is true, then it will repeat the loop as long as the condition is true
```
let i = 0;
do {
  console.log(i);
  i++;
}
while (i < 5);
```
---
## JavaScript Data Types

### Integers 
- Numbers with no decimal or fractional part and it includes negative and positive numbers, including zero. 

```
1, -5, 0, -1, 5, 485, 9307
```
### Strings 
- A sequence of characters treated as a single piece of data.
- May include alphabetic letters, symbols, numbers and space.
- Numbers can also be a string when enclosing with quotation marks.
```
"hello", "Web103", "12345"
```
### Booleans 
- Store yes/no values: **true** means “yes, correct”, and **false** means “no, incorrect”

```
let x = 5;  // declare x as variable and assign the value of 5
x == 5;     // true
x >= 10;    // false
```
### Arrays 
- Special data type that can hold many values under a single name
- Can access the values by referring to an index number
```
let students = ["Lisa", "Benton", "Devon"];
let scores = [95, 90, 93];

```
### Objects
- Store keyed collections of various data and more complex entities
- Each property has a key (also known as “identifier”) before the colon ":" and a value to the right of it
- Property values are accessible using the dot notation

```
let user = {          // declare "user" as an object
  name: "Jonathan",   // key "name" stores value "Jonathan"
  age: 32             // key "age" stores value 32
};

console.log(user.age ); // 32
```
### NULL
- Only contains the ***null*** value
```
let age = null;
```
---
## JavaScript Comments
```
// Use double forward slashes for single line comment

/* Use slash and asterisk 
for multiple-line comments */
```

