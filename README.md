# JavaScript_Assignment_1

Ques : 1   create a jaascript file, using jaascript comments, List all the datatypes of Jaascript, and specify an example for each of them.

Ans    // JavaScript Data Types and Examples

// 1. Number
var numberExample = 42; // Example of a number

// 2. String
var stringExample = "Hello, World!"; // Example of a string

// 3. Boolean
var booleanExample = true; // Example of a boolean

// 4. Array
var arrayExample = [1, 2, 3, 4, 5]; // Example of an array

// 5. Object
var objectExample = { name: "John", age: 30 }; // Example of an object

// 6. Null
var nullExample = null; // Example of null

// 7. Undefined
var undefinedExample; // Example of undefined

// 8. Symbol
var symbolExample = Symbol("unique"); // Example of a symbol

// 9. BigInt
var bigIntExample = 1234567890123456789012345678901234567890n; // Example of a BigInt

// 10. Function
function functionExample() {
  return "This is a function";
}

// 11. Date
var dateExample = new Date(); // Example of a Date

// 12. RegExp (Regular Expression)
var regexExample = /pattern/; // Example of a regular expression

// 13. Map
var mapExample = new Map(); // Example of a Map

// 14. Set
var setExample = new Set(); // Example of a Set

// 15. ArrayBuffer
var arrayBufferExample = new ArrayBuffer(16); // Example of an ArrayBuffer

// 16. DataView
var dataViewExample = new DataView(arrayBufferExample); // Example of a DataView

// 17. Promise
var promiseExample = new Promise((resolve, reject) => {
  // Example of a Promise
});

// 18. Generator
function* generatorExample() {
  yield 1;
  yield 2;
  yield 3;
}

// 19. Typed Arrays
var typedArrayExample = new Int32Array([1, 2, 3]); // Example of a Typed Array

// 20. Function Constructor
var functionConstructorExample = new Function("x", "y", "return x + y"); // Example of a Function Constructor

// 21. Custom Objects
function CustomObject(name, age) {
  this.name = name;
  this.age = age;
}
var customObjectExample = new CustomObject("Alice", 25); // Example of a custom object

// 22. Any other user-defined objects

// End of JavaScript Data Types

// Feel free to add more data types or examples as needed.


Ques 2  Create an array of 10 products that you have recently purchased or viewed on an e-commerce site.

Ans --  var recentlyViewedProducts = [
  "Smartphone Case",
  "Wireless Earbuds",
  "Laptop Backpack",
  "Fitness Tracker",
  "Coffee Maker",
  "Bluetooth Speaker",
  "Digital Camera",
  "Smart TV",
  "Running Shoes",
  "Kitchen Blender"
];


Ques 3  Create an object of a student registry of 5 students whose key is the registration number and the value is the student name. Registration number starts from 1 and continues.

Ans   var studentRegistry = {
  1: "John Doe",
  2: "Alice Smith",
 3: "Bob Johnson",
 4: "Emily Wilson",
 5: "Michael Brown"
};

Variables and typeof

Ques  1   Specify an example for all the datatypes in Javascript, store the values in a variable, and verify the type of value stored.

Ans   // Number
var num = 42;
console.log("Type of num: " + typeof num);

// String
var str = "Hello, World!";
console.log("Type of str: " + typeof str);

// Boolean
var bool = true;
console.log("Type of bool: " + typeof bool);

// Array
var arr = [1, 2, 3, 4, 5];
console.log("Type of arr: " + typeof arr);

// Object
var obj = { name: "John", age: 30 };
console.log("Type of obj: " + typeof obj);

// Null
var n = null;
console.log("Type of n: " + typeof n);

// Undefined
var u;
console.log("Type of u: " + typeof u);

// Symbol
var sym = Symbol("unique");
console.log("Type of sym: " + typeof sym);

// BigInt
var bigInt = 1234567890123456789012345678901234567890n;
console.log("Type of bigInt: " + typeof bigInt);

// Function
function myFunction() {
  return "This is a function";
}
console.log("Type of myFunction: " + typeof myFunction);

// Date
var date = new Date();
console.log("Type of date: " + typeof date);

// Regular Expression
var regex = /pattern/;
console.log("Type of regex: " + typeof regex);

// Map
var map = new Map();
console.log("Type of map: " + typeof map);

// Set
var set = new Set();
console.log("Type of set: " + typeof set);

// ArrayBuffer
var buffer = new ArrayBuffer(16);
console.log("Type of buffer: " + typeof buffer);

// DataView
var dataView = new DataView(buffer);
console.log("Type of dataView: " + typeof dataView);

// Promise
var promise = new Promise((resolve, reject) => {
  // A promise example
});
console.log("Type of promise: " + typeof promise);

// Generator
function* generator() {
  yield 1;
  yield 2;
  yield 3;
}
console.log("Type of generator: " + typeof generator);

// Typed Array
var typedArray = new Int32Array([1, 2, 3]);
console.log("Type of typedArray: " + typeof typedArray);

// Custom Object
function CustomObject(name, age) {
  this.name = name;
  this.age = age;
}
var customObj = new CustomObject("Alice", 25);
console.log("Type of customObj: " + typeof customObj);


Ques  2  Create 2 valid variables and 2 invalid variables and print them onto the console. Comment the results and error messages.

Ans  // Valid Variables

// Valid variable name containing letters, numbers, and underscores.
var validVariableName = "Hello_World";

// Valid variable assignment using the 'const' keyword.
const validConstVariable = 42;

// Invalid Variables

// Invalid variable name starting with a number (results in a syntax error).
var 1stVariable = 10; // SyntaxError: Identifier starts immediately after numeric literal

// Invalid variable assignment to a constant (results in a TypeError).
const invalidConstAssignment = "This will cause an error";
invalidConstAssignment = "Trying to reassign"; // TypeError: Assignment to a constant variable

// Print the valid and invalid variables (will only execute the valid variables).

console.log("Valid Variable 1: " + validVariableName);
console.log("Valid Variable 2: " + validConstVariable);

// Attempting to print the invalid variables would result in errors, so they are commented out.

// console.log("Invalid Variable 1: " + 1stVariable); // Uncommenting this line will result in a syntax error.
// console.log("Invalid Variable 2: " + invalidConstAssignment); // Uncommenting this line will result in a TypeError.



Operators

Ques 1 Write a program that prints the multiplication table in the textbook format of any number specified.

Ans   function printMultiplicationTable(number, range) {
  // Iterate through the specified range (default is 10 if not provided)
  range = range || 10;
  
  for (let i = 1; i <= range; i++) {
    // Calculate the product of the number and the current iterator value
    const product = number * i;
    
    // Print the result in a formatted manner
    console.log(`${number} x ${i} = ${product}`);
  }
}

// Call the function with the desired number and range
const numberToPrint = 5; // Change this to any number you want
printMultiplicationTable(numberToPrint);



Ques 2  Write a program to perform all the arithmetic operations [except increment and decrement operators] of javascript of any two numbers stored in the variables num1 and num2. Also, print the results to the console.


Ans   // Define the two numbers
var num1 = 10;
var num2 = 5;

// Addition
var addition = num1 + num2;
console.log(`Addition: ${num1} + ${num2} = ${addition}`);

// Subtraction
var subtraction = num1 - num2;
console.log(`Subtraction: ${num1} - ${num2} = ${subtraction}`);

// Multiplication
var multiplication = num1 * num2;
console.log(`Multiplication: ${num1} * ${num2} = ${multiplication}`);

// Division
var division = num1 / num2;
console.log(`Division: ${num1} / ${num2} = ${division}`);

// Modulus (Remainder)
var modulus = num1 % num2;
console.log(`Modulus: ${num1} % ${num2} = ${modulus}`);

// Exponentiation
var exponentiation = Math.pow(num1, num2);
console.log(`Exponentiation: ${num1} ^ ${num2} = ${exponentiation}`);


Ques 3 Write a program to find out the perimeter of a rectangle. Print the results to the console.

Ans 

// Define the dimensions of the rectangle
var length = 10; // Replace with the actual length of the rectangle
var width = 5;   // Replace with the actual width of the rectangle

// Calculate the perimeter
var perimeter = 2 * (length + width);

// Print the result to the console
console.log("The perimeter of the rectangle is: " + perimeter);


Ques 4   Write a program to demonstrate the results of comparison operators. Note that both the truth and false condition for each operator must be specified.


Ans  

// Comparison operators
var num1 = 10;
var num2 = 5;

// Equal to (==)
console.log(`${num1} == ${num2} is ${num1 == num2}`); // False

// Not equal to (!=)
console.log(`${num1} != ${num2} is ${num1 != num2}`); // True

// Greater than (>)
console.log(`${num1} > ${num2} is ${num1 > num2}`); // True

// Less than (<)
console.log(`${num1} < ${num2} is ${num1 < num2}`); // False

// Greater than or equal to (>=)
console.log(`${num1} >= ${num2} is ${num1 >= num2}`); // True

// Less than or equal to (<=)
console.log(`${num1} <= ${num2} is ${num1 <= num2}`); // False

What are Conditions, If, If-else, if-else-if


Ques 1   
Write a program of traffic control that accepts the traffic light displayed and prints the message. If the traffic light is red print the vehicles must stop.

Ans  

// Accept the current traffic light color (you can change this value)
var trafficLightColor = "red"; // Change this to "green" or "yellow" to test other cases

// Check the traffic light color and print a message
if (trafficLightColor === "red") {
  console.log("Vehicles must stop.");
} else if (trafficLightColor === "green") {
  console.log("Vehicles can proceed.");
} else if (trafficLightColor === "yellow") {
  console.log("Prepare to stop if safe.");
} else {
  console.log("Invalid traffic light color.");
}



  Ques 2 Write a program to print the largest of 2 numbers.


Ans  // Accept two numbers as input (you can change these values)
var num1 = 10;
var num2 = 5;

// Compare the two numbers and determine the largest
if (num1 > num2) {
  console.log("The largest number is: " + num1);
} else if (num2 > num1) {
  console.log("The largest number is: " + num2);
} else {
  console.log("Both numbers are equal.");
}

Ques 3 Write a program that takes a number as input and outputs "Fizz" if it is divisible by 3, "Buzz" if it is divisible by 5, and "FizzBuzz" if it is divisible by both 3 and 5. Note that any number can be passed and not restricted to the numbers divisible by 3 or 5.

Ans  // Accept a number as input (you can change this value)
var number = 15; // Change this to test with different numbers

// Check if the number is divisible by 3, 5, or both
if (number % 3 === 0 && number % 5 === 0) {
  console.log("FizzBuzz");
} else if (number % 3 === 0) {
  console.log("Fizz");
} else if (number % 5 === 0) {
  console.log("Buzz");
} else {
  console.log(number);
}


Switch Case

Quss 1  Write a program that takes in a day of the week (e.g., Monday, Tuesday, etc.) and outputs the number of days until the weekend.

Ans  // Accept the day of the week as input (case-insensitive)
var dayOfWeek = "Monday"; // Change this to the desired day of the week

// Convert the input to lowercase for case-insensitive comparison
dayOfWeek = dayOfWeek.toLowerCase();

// Define an array representing days of the week
var daysOfWeek = ["sunday", "monday", "tuesday", "wednesday", "thursday", "friday", "saturday"];

// Find the index of the input day in the array
var dayIndex = daysOfWeek.indexOf(dayOfWeek);

// Calculate the number of days until the weekend (Saturday)
var daysUntilWeekend = (6 - dayIndex + 7) % 7;

console.log(`There are ${daysUntilWeekend} days until the weekend.`);

Ques 2  Write a program that takes in a number between 1 and 12 and outputs the corresponding month of the year.

Ans   // Accept a number between 1 and 12 as input
var monthNumber = 7; // Change this to the desired number

// Define an array representing the months of the year
var monthsOfYear = [
  "January", "February", "March", "April",
  "May", "June", "July", "August",
  "September", "October", "November", "December"
];

// Check if the input number is within the valid range
if (monthNumber >= 1 && monthNumber <= 12) {
  var monthName = monthsOfYear[monthNumber - 1]; // Adjust for zero-based array index
  console.log(`The corresponding month is: ${monthName}`);
} else {
  console.log("Invalid input. Please enter a number between 1 and 12.");
}

Ternary Conditions

Ques 1  Write a program that takes in a number and outputs whether it is positive, negative, or zero.

Ans  // Accept a number as input
var number = 0; // Change this to the desired number

// Check if the number is positive, negative, or zero
if (number > 0) {
  console.log("The number is positive.");
} else if (number < 0) {
  console.log("The number is negative.");
} else {
  console.log("The number is zero.");
}

Ques 2  Create a program that takes in two numbers and prints the larger one.

Ans  // Accept two numbers as input
var number1 = 15; // Change this to the first number
var number2 = 25; // Change this to the second number

// Compare the two numbers and print the larger one
if (number1 > number2) {
  console.log("The larger number is: " + number1);
} else if (number2 > number1) {
  console.log("The larger number is: " + number2);
} else {
  console.log("Both numbers are equal.");
}

Loops

Ques 1  Write a program that generates the multiplication table in the textbook format for a given number.

// Accept a number for which you want to generate the multiplication table
var number = 7; // Change this to the desired number

// Define the range for the multiplication table
var range = 10; // You can change this to control how many times you want to multiply

// Generate and print the multiplication table
console.log(`Multiplication Table for ${number}:`);
for (var i = 1; i <= range; i++) {
  var product = number * i;
  console.log(`${number} x ${i} = ${product}`);
}


Que 2 Write a program that prints all the positive even numbers till the number specified.

Ans  // Specify the maximum number
var maxNumber = 20; // Change this to the desired maximum number

// Print all positive even numbers up to the specified number
console.log("Positive even numbers up to " + maxNumber + ":");
for (var i = 2; i <= maxNumber; i += 2) {
  console.log(i);
}
