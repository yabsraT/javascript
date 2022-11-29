# CONCEPT,VARIABLE AND DATATYPE 

## **Concept of javascript**
 JavaScript is a powerful programming language that can add interactivity to a website. It was invented by Brendan Eich.
 JavaScript is versatile and beginner-friendly. With more experience, you'll be able to create games, animated 2D and 3D graphics, 
 comprehensive database-driven apps, and much more!. JavaScript itself is relatively compact, yet very flexible. Developers have written a 
 variety of tools on top of the core JavaScript language, unlocking a vast amount of functionality with minimum effort.
 ## **JavaScript Variable**
 A JavaScript variable is simply a name of storage location. There are two types of variables in JavaScript : local variable and global variable.
 There are some rules while declaring a JavaScript variable (also known as identifiers).
 Name must start with a letter (a to z or A to Z), underscore( _ ), or dollar( $ ) sign.
 After first letter we can use digits (0 to 9), for example value1.
 JavaScript variables are case sensitive, for example x and X are different variables.

 Correct JavaScript variables
```
var x = 10;  
var _value="sonoo"; 
```
Incorrect JavaScript variables
```
var  123=30;  
var *aa=320;  

```
Example of JavaScript variable
Let’s see a simple example of JavaScript variable.
```
<script>  
var x = 10;  
var y = 20;  
var z=x+y;  
document.write(z);  
</script>  

```
## **Javascript Data Types**
JavaScript provides different data types to hold different types of values. There are two types of data types in JavaScript.
1. Primitive data type
2. Non-primitive (reference) data type

JavaScript is a dynamic type language, means you don't need to specify type of the variable because it is dynamically used by JavaScript engine. You need to use var here to specify the data type. It can hold any type of values such as numbers, strings etc. For example:
```
var a=40;//holding number  
var b="Rahul";//holding string  

```
JavaScript primitive data types
There are five types of primitive data types in JavaScript. 
They are as follows:
```
**String	** represents sequence of characters e.g. "hello"
**Number**	represents numeric values e.g. 100
**Boolean	** represents boolean value either false or true
**Undefined**	represents undefined value
**Null**	represents null i.e. no value at all
```
JavaScript non-primitive data types
The non-primitive data types are as follows:
```
**Object**	represents instance through which we can access members
**Array**	represents group of similar values
**RegExp	** represents regular expression

```





