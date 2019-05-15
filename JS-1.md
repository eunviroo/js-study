# Preparation

- [Node.js](https://nodejs.org/en/download/)
- [Git](https://git-scm.com)

## 1. Hello
```
// hello.js
console.log("Hello Le Wagon");
```

## 2. Basic Types
```
"Hello Le Wagon"            // string

42                          // number
3.14                        // number

true                        // boolean
```

## 3. Checking types
```
typeof("Boris");
// => 'string'

typeof(42);
// => 'number'
```

## 4. Casting types
```
Number.parseInt('42', 10);
// => 42

(42).toString();
// => '42'
```

## 5. Data structures
```
[ 'Hello', 'Le', 'Wagon', 42 ]    // Array

{ name: 'bob', age: 42 }          // Object
{ 'name': 'bob', 'age': 42 }      // Object (the exact same)
```

### 5-1. Null & Undefined
```
let age; // undefined
let name = null;
```

## 5. Variables
Old JS uses var.<br>
ES6 uses two new keywords in replacement.

### <b>let</b>
For a variable you will re-assign
```
let counter = 1;
console.log(counter);

counter = counter + 1;
console.log(counter);
```

### <b>const</b>
For a variable you won't re-assign
```
const firstName = "John";
console.log(firstName);

firstName = "Paul"; // TypeError: Assignment to constant variable.
```

## Naming convention
```
const firstName = "Ringo";
// lowerCamelCase
```

## Strings

### Length
```
const firstName = "Paul";
firstName.length;
// => 4
```

### Character access
```
const firstName = "John";
firstName[0];
// => "J"

// Print all characters starting at index 1
firstName.substring(1);
```

### Case manipulation
```
const firstName = "Paul";
firstName.toUpperCase();
// => "PAUL"

firstName.toLowerCase();
// => "paul"
```

### Split
```
const monthString = "Jan,Feb,Mar,Apr,May,Jun,Jul,Aug,Sep,Oct,Nov,Dec";

const months = monthString.split(",");
// => [ 'Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun', 'Jul', 'Aug', 'Sep', 'Oct', 'Nov', 'Dec' ]
months.length;
// => 12
```

### Interpolation
```
const firstName = "Ringo";
const lastName = "Starr";

const message = `${firstName} ${lastName} is a drummer`;
// => "Ringo Starr is a drummer";
```

## Arrays
### CRUD
```
const fruits = [];
fruits.push("Apple"); // Create
fruits[0];            // Read
fruits[0] = "Banana"; // Update
fruits.splice(0, 1);  // Delete (1 item at index 0)
```

### forEach
```
const beatles = ["paul", "john", "ringo", "george"];
beatles.forEach((beatle) => {
  console.log(beatle.toUpperCase());
});
```

## Control Flow
### if / else
```
const age = 14;

if (age >= 18) {
  console.log("You can vote");
} else {
  console.log("You can't vote");
}
```

### Falsy values
```
false
undefined
null
0
NaN
""
```

### Ternary Operator
```
const raining = true;
const accessory = (raining ? "umbrella" : "sunglasses");
// => "umbrella"
```

```
if (digit === 0) {
  console.log('Zero');
} else if (digit === 1) {
  console.log('One');
} else {
  console.log("I don't know this digit, sorry!");
}
```

Read more about sameness in JS and the difference between == and ===.

## Objects

### Simple Object
```
const student = {
  firstName: "Boris",
  lastName: "Paillard"
};

console.log(typeof student);
// => "object"

console.log(student);
```

### Reading/Setting a property
You can use the dot-notation.
```
console.log(student.firstName);
// => "Boris"
console.log(student['firstName']); // Another way
// => "Boris"
```

```
student.firstName = "Romain";
console.log(student.firstName);
// => "Romain"
```

## Functions
### Defining
```
function square(x) {
  return x * x;
}
```

### Calling
```
square(10);
// => 100
```

### Arrow Function
```
const square = (x) => {
  return x * x;
};

// Or even shorter, with **implicit** return.
const square = x => x * x;
```
<b>What should I use?</b><br>
Arrow functions are a new way to write functions since ES6 and they are our preferred way of writing functions. During your batch, always use arrow functions instead of ES5 function statements.

### Capitalize example
```
var firstLetterCap = function(string) {
  return
}
```