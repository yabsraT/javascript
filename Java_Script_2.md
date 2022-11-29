# Javascript Conditional_statment,loops

## **Conditional_statment**
Conditional statements control behavior in JavaScript and determine whether or not pieces of code can run.

There are multiple different types of conditionals in JavaScript including:
- “If” statements: where if a condition is true it is used to specify execution for a block of code.
* “Else” statements: where if the same condition is false it specifies the execution for a block of code.
+ “Else if” statements: this specifies a new test if the first condition is false.

### **If Statement Example**
As the most common type of conditional, the if statement only runs if the condition enclosed in parentheses () is truthy.
```
**EXAMPLE**
if (10 > 5) {
      var outcome = "if block";
}
outcome;

**OUTPUT**
"if block"
```
Here’s what’s happening in the example above:
- The keyword if tells JavaScript to start the conditional statement.
- (10 > 5) is the condition to test, which in this case is true — 10 is greater than 5.
- The part contained inside curly braces {} is the block of code to run.
- Because the condition passes, the variable outcome is assigned the value "if block".

### **Else Statement Example**
You can extend an if statement with an else statement, which adds another block to run when the if conditional doesn’t pass.
```
**EXAMPLE**
if ("cat" === "dog") {
      var outcome = "if block";
} else {
      var outcome = "else block";
}
outcome;
**OUTPUT**
"else block"

```
In the example above, "cat" and "dog" are not equal, so the else block runs and the variable outcome gets the value "else block".

### **Else If Statement Example**
You can also extend an if statement with an else if statement, which adds another conditional with its own block.
```

EXAMPLE
if (false) {
      var outcome = "if block";
} else if (true) {
      var outcome = "else if block";
} else {
      var outcome = "else block";
}

outcome;
OUTPUT
"else if block"
```

You can use multiple if else conditionals, but note that only the first else if block runs. JavaScript skips any remaining conditionals after it runs the first one that passes.
EXAMPLE
```
if (false) {
      var outcome = "if block";
} else if (true) {
      var outcome = "first else if block";
} else if (true) {
      var outcome = "second else if block";
} else {
      var outcome = "else block";
}

outcome;
OUTPUT
"first else if block"
```
An else if statement doesn’t need a following else statement to work. If none of the if or else if conditions pass, then JavaScript moves forward and doesn’t run any of the conditional blocks of code.
```
EXAMPLE
if (false) {
      var outcome = "if block";
} else if (false) {
      var outcome = "else if block";
}

outcome;
OUTPUT
"first else if block"
```
## **JavaScript Loops**

The JavaScript loops are used to iterate the piece of code using for, while, do while or for-in loops. It makes the code compact. It is mostly used in array.

There are four types of loops in JavaScript.

1. for loop
2. while loop
3. do-while loop


1) **JavaScript For loop**
The JavaScript for loop iterates the elements for the fixed number of times. It should be used if number of iteration is known. The syntax of for loop is given below.
```
for (initialization; condition; increment)  
{  
    code to be executed  
} 
```
Let’s see the simple example of for loop in javascript.
```
<script>  
for (i=1; i<=5; i++)  
{  
document.write(i + "<br/>")  
}  
</script> 
```
Test it Now
```
Output:

1
2
3
4
5
```
2) **JavaScript while loop**
The JavaScript while loop iterates the elements for the infinite number of times. It should be used if number of iteration is not known. The syntax of while loop is given below.
```
while (condition)  
{  
    code to be executed  
}  
```
Let’s see the simple example of while loop in javascript.
```
<script>  
var i=11;  
while (i<=15)  
{  
document.write(i + "<br/>");  
i++;  
}  
</script> 
  ```
Test it Now
```
Output:

11
12
13
14
15
```
3) **JavaScript do while loop**
The JavaScript do while loop iterates the elements for the infinite number of times like while loop. But, code is executed at least once whether condition is true or false. The syntax of do while loop is given below.
```
do{  
    code to be executed  
}while (condition);  
```
Let’s see the simple example of do while loop in javascript.
```
<script>  
var i=21;  
do{  
document.write(i + "<br/>");  
i++;  
}while (i<=25);  
</script>  
```
Test it Now
```
Output:

21
22
23
24
25
```


