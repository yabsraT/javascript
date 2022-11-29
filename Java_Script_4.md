# java script function,arrays

## **JavaScript Function**

A function is a block of code that performs a specific task.

Suppose you need to create a program to create a circle and color it. You can create two functions to solve this problem:

- a function to draw the circle
- a function to color the circle
Dividing a complex problem into smaller chunks makes your program easy to understand and reusable.

JavaScript also has a huge number of inbuilt functions. For example, Math.sqrt() is a function to calculate the square root of a number.

In this tutorial, you will learn about user-defined functions.

### **Declaring a Function**
The syntax to declare a function is:
```
function nameOfFunction () {
    // function body   
}
```
- A function is declared using the function keyword.
- The basic rules of naming a function are similar to naming a variable. It is better to write a descriptive name for your function. For example, if a function is used to add two numbers, you could name the function add or addNumbers.
- The body of function is written within {}.
For example,
```
// declaring a function named greet()
function greet() {
    console.log("Hello there");
}
```
### **Calling a Function**

In the above program, we have declared a function named greet(). To use that function, we need to call it.

Here's how you can call the above greet() function.
```
// function call
greet();
```
**Example : Display a Text**
```
// program to print a text
// declaring a function
function greet() {
    console.log("Hello there!");
}

// calling the function
greet();
```
Output
```
Hello there!

```
Function Parameters
A function can also be declared with parameters. A parameter is a value that is passed when declaring a function.

Example 2: Function with Parameters

```
// program to print the text
// declaring a function
function greet(name) {
    console.log("Hello " + name + ":)");
}

// variable name can be different
let name = prompt("Enter a name: ");

// calling function
greet(name);

```
## **JavaScript Arrays**
An array is an object that can store multiple values at once. For example,

const words = ['hello', 'world', 'welcome'];
Here, **words** is an array. The array is storing 3 values.

**Create an Array**
You can create an array using two ways:

1. **Using an array literal**

The easiest way to create an array is by using an array literal []. For example,
```
const array1 = ["eat", "sleep"];
```
2.** Using the new keyword **
You can also create an array using JavaScript's new keyword.
```
const array2 = new Array("eat", "sleep");
```
In both of the above examples, we have created an array having two elements.



Here are more examples of arrays:
```
// empty array
const myList = [ ];

// array of numbers
const numberArray = [ 2, 4, 6, 8];

// array of strings
const stringArray = [ 'eat', 'work', 'sleep'];

// array with mixed data types
const newData = ['work', 'exercise', 1, true];
```
You can also store arrays, functions and other objects inside an array. For example,
```
const newData = [
    {'task1': 'exercise'},
    [1, 2 ,3],
    function hello() { console.log('hello')}
];
```

 ### Access Elements of an Array
You can access elements of an array using indices (0, 1, 2 …). For example,
```
const myArray = ['h', 'e', 'l', 'l', 'o'];

// first element
console.log(myArray[0]);  // "h"

// second element
console.log(myArray[1]); // "e"

```








