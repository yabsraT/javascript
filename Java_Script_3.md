# **Java Script Methods,Doms,Events**

## **JavaScript methods**
An object is a collection of key/value pairs or properties. When the value is a function, the property becomes a method. Typically, you use methods to describe the object behaviors.

For example, the following adds the **greet** method to the **person** object:
```

let person = {
    firstName: 'John',
    lastName: 'Doe'
};

person.greet = function () {
    console.log('Hello!');
}

person.greet();
```
Output:
```

Hello!
```
In this example:

First, use a function expression to define a function and assign it to the greet property of the **person** object.
Then, call the method **greet() ** method.
Besides using a function expression, you can define a function and assign it to an object like this:
```

let person = {
    firstName: 'John',
    lastName: 'Doe'
};

function greet() {
    console.log('Hello, World!');
}

person.greet = greet;

person.greet();
```

In this example:
- First, define the greet() function as a regular function.
- Second, assign the function name to the the greet property of the person object.
- Third, call the greet() method.

Object method shorthand

JavaScript allows you to define methods of an object using the object literal syntax as shown in the following example:
```

let person = {
    firstName: 'John',
    lastName: 'Doe',
    greet: function () {
        console.log('Hello, World!');
    }
};
```
ES6 provides you with the concise method syntax that allows you to define a method for an object:
```
let person = {
    firstName: 'John',
    lastName: 'Doe',
    greet() {
        console.log('Hello, World!');
    }
};
person.greet();
```
This syntax looks much cleaner and less verbose.

## **The this value**
Typically, methods need to access other properties of the object.

For example, you may want to define a method that returns the full name of the person object by concatenating the first name and last name.

Inside a method, the this value references the object that invokes the method. Therefore, you can access a property using the this value as follows:
```
this.propertyName
```

The following example uses the this value in the getFullName() method:
```
let person = {
    firstName: 'John',
    lastName: 'Doe',
    greet: function () {
        console.log('Hello, World!');
    },
    getFullName: function () {
        return this.firstName + ' ' + this.lastName;
    }
};
console.log(person.getFullName());
```

Output
```
'John Doe'
```
## **DOM of Java Script**

The document object represents the whole html document.
When html document is loaded in the browser, it becomes a document object. It is the root element that represents the html document. 
It has properties and methods. By the help of document object, we can add dynamic content to our web page.

As mentioned earlier, it is the object of window. So
```
window.document  
```
Is same as
```
document    
```
According to W3C - "The W3C Document Object Model (DOM) is a platform and language-neutral interface that allows programs and scripts to 
dynamically access and update the content, structure, and style of a document."

### **Methods of document object**
We can access and change the contents of document by its methods.

The important methods of document object are as follows:

```

**write("string")**	writes the given string on the doucment.
**writeln("string")**	writes the given string on the doucment with newline character at the end.
**getElementById()**	returns the element having the given id value.
**getElementsByName()	** returns all the elements having the given name value.
**getElementsByTagName()**	returns all the elements having the given tag name.
**getElementsByClassName()**	returns all the elements having the given class name.

```
### **Accessing field value by document object**
In this example, we are going to get the value of input text by user. Here, we are using document.form1.name.value to get the value of name field.

Here, document is the root element that represents the html document.

form1 is the name of the form.

name is the attribute name of the input text.

value is the property, that returns the value of the input text.

Let's see the simple example of document object that prints name with welcome message.

```
<script type="text/javascript">  
function printvalue(){  
var name=document.form1.name.value;  
alert("Welcome: "+name);  
}  
</script>  
  
<form name="form1">  
Enter Name:<input type="text" name="name"/>  
<input type="button" onclick="printvalue()" value="print name"/>  
</form>  

```
## ** javascript Events **

The change in the state of an object is known as an Event. In html, there are various events which represents that some activity is performed by the user or by the browser. When javascript code is included in HTML, js react over these events and allow the execution. This process of reacting over the events is called Event Handling. Thus, js handles the HTML events via Event Handlers.

For example, when a user clicks over the browser, add js code, which will execute the task to be performed on the event.

Some of the HTML events and their event handlers are:

Click Event

```
<html>  
<head> Javascript Events </head>  
<body>  
<script language="Javascript" type="text/Javascript">  
    <!--  
    function clickevent()  
    {  
        document.write("This is JavaTpoint");  
    }  
    //-->  
</script>  
<form>  
<input type="button" onclick="clickevent()" value="Who's this?"/>  
</form>  
</body>  
</html>  

```
MouseOver Event

```
<html>  
<head>   
<h1> Javascript Events </h1>  
</head>  
<body>  
<script language="Javascript" type="text/Javascript">  
    <!--  
    function mouseoverevent()  
    {  
        alert("This is JavaTpoint");  
    }  
    //-->  
</script>  
<p onmouseover="mouseoverevent()"> Keep cursor over me</p>  
</body>  
</html>  

```


Focus Event
```
<html>  
<head> Javascript Events</head>  
<body>  
<h2> Enter something here</h2>  
<input type="text" id="input1" onfocus="focusevent()"/>  
<script>  
<!--  
    function focusevent()  
    {  
        document.getElementById("input1").style.background=" aqua";  
    }  
//-->  
</script>  
</body>  
</html>  
```








