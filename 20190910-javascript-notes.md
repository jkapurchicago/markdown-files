Objective 1: Evaluate JS using the developer console
Objective 2: List the 5 Js primitives
Objective 3: Define variables with the var keyword 
Objective 4: Write code using console.log alert and prompt 


GOOGLE CHROME CONSOLE FOR JAVASCRIPT Shortcut to open console: command + option + j 
View -> Developer -> Javacript Console 

```javascript
var logo = document.querySelector("hplogo"); 
setInterval(function(){
    logo.width+=5;
 }, 100)
alert("Hello everyone!"); 
```


Objectives: 
    Introduce the 5 primitive data types 
    Work with numbers and numeric operators
    Work with strings and common string methods

```javascript
//Numbers 
4 
9.3 
-10

//Strings 
"hello world" 
"43" 

//Boolean 
true 
false 

//null and undefined 
null 
undefined 

# SIMPLE OPERATORS 
```script
//We can do some math 
4 + 10 //14 
1/5 //0.2 

JAVASCRIPT FOLLOWS THE ORDER OF OPERATIONS 
(3-8) * 24  // -120 
(-5) * 24 //-120 

//Modulo - remainder operator 
10 % 3 //1 
24 % 2 //0 
15 % 11 //4 


Strings 
//single or double quotes OK 
"hello world" 
'hello world' 
```
BE AWARE THIS WILL SPIT OOUT AN ERROR, 

```javascript 

   'I can't stop' 

//concatenation 
"charlie" + "brown" // "charliebrown" 

//Escape Characters start with "\"
"Singin \"Do wah diddy, diddy, dum diddy do\" "
"This is a backslash: \\"

//Strings have a length property
"hello world".length  //11

//Access individual characters using [] and an index
"hello"[0]  //"h"
"hello"[4]  // "o" 

"hi" + "goodbye" 

Javascript escape characters 
"she said \"goodbye!" " 

"To see a backsplash: \\" ouputs "to see a backsplash: \" 

"HELLO".length 
5
"The Beatles"[0]
"T"
"The Beatles"[4]
"B"

"The Beatles"[10]
"s"
"The Beatles".length
11


"blah" + "blah" 

//Variables are simply containers that store values
//They follow this pattern:
var yourVariableName = yourValue;

//They can store all of the values we've seen
var name = "Rusty";
var secretNumber = 73;
var isAdorable = true;

//Recall the stored value by calling the variable name
var name = "Rusty";
"hello there " + name    //"hello there Rusty"

var num = 37;
num + 3 + 10    //50

//We can also update existing variables
var name = "Robert";
name = "Bob";

javascript has this called dynamic typic which defines that there is a convention 
that defines how we name them. 
javascript variables hpuld be cammel cased. 

//The two other primitives are null and undefined

//Variables that are declared but not 
//initialized are undefined
//The following variables are undefined:
var name;
var age;

//null is "explicitly nothing"
var currentPlayer = "charlie";
currentPlayer = null;   //game over

"hello".length

"hi".length


console.log("hello"); 

"hi".length; 

var boat = "hisdw"; 
console.log(boat.length); 

var yourVariableName = "yourValue"; 
console.log(yourVariableName); 

var name ="Rusty"; 
var secretNumber = 73; 
var isAdorable = true; 

var name = " Rusty"; 
"hello there " + name 
console.log("hello there" + name); 

var num = 43; 
num + 100; 
console.log(num + 100); 




var name; 
console.log(name); 



var currentPlayer = "charlie"; 
currentPlayer = null; 

```
---- 
# METHODS 
encapulation

Alert gives us a pop up that displays a message 
alert("Hello everyone!"); 
alert("fheiefhewifhefdhewfwefewf"); 
alert(13345235);
alert(12+5); 
alert(198 * 345); 

console.log("hello from the console!"); 
VM477:1 hello from the console!



//prompt 
prompt("what is your name?"); 
"Jatin Kapur "

// second part of prompt is storing the value in a variable 

var userName = prompt("what is your name?"); 


<script src="blahBlah.js"></script>


```html
<!--TESTING ALERTS--> 
<!DOCTYPE html> 
<html> 
<head>
    <title>Script Demo</title>
    <script src="practice.js"></script>
</head>
<body>
    <h1>Including JS Files</h1>
</body>
</html> 
```

```javascript

alert("Hello From the Js file"); 
var userName = prompt("What is your name?"); 
alert("hello " + userName); 
```

--- 
Control Flow:

Objective 1: Evaluate complex logical expressions

Objective 2: Write 3-part JS conditional statements 

Objectve 3: Write Js while loops and for loops 


BOOLEAN LOGIC: True, Fale and Beyond 
1. Everything starts with the idea that a statement is either True or False.
 
2. Then we can combine those initial statements to create more complex statements that also evaluate to True or False.

Comparsion Operators Assuming x = 5 
 

 if 

else if 


else 

