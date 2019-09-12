# August 8, 2019 - LEARNING NODE.JS AND NPM  
1. Npm init - Generates a package.json file 
1. Npm install express - Install a package locally 
1. Npm install -g nodemon Install a package globally 
__

* Install 3rd Party Packages(frameworks, libraries, tools, etc.) 
* Packages get stored in the “node_modules” folder 
* All dependencies are listed in a “package.json” file 
* Npm scripts can be created to run certain tasks such as run a server. 

* Node Core Modules (path, fs, http. Etc) 
* 3rd Party Modules/packages install via NPM 
* Custom modules (files) 

```bash
Const path = require(‘path’); 
Const myFile = require(‘./myFile’); 
```

## NODE.JS
`Non Blocking I/O. Works on a single thread using non-blocking I/O c
  Supports tens of thousands concurrent connections ` 
* Optimizes scalability in web applications with many I/o operations.  
* This makes Node.Js extremely fast and efficient 

## Node Package Manager 

1. Install 3rd Party Packages (frameworks, libraries, tools, etc)
2. Package gets installed in the "node - modules" folder 

3. All dependencies are listed in a "Package.Json" file 
NPM scripts can be created to run certain tasks such as run on a server

## COMMANDS ON TERMINAL 
```bash
Last login: Wed Aug  7 13:09:37 on ttys000
Jiamaos-MacBook-Pro:~ Jatin$ node --version #command to check node version  
v10.16.1
Jiamaos-MacBook-Pro:~ Jatin$ npm --version #command to check npm 
6.9.0
Jiamaos-MacBook-Pro:~ Jatin$ node
> 1+1 #you can run javascript on the terminal due to node
2
> const name = 'Brad'
undefined
> console.log('name')
name
undefined
> console.log(name);
Brad
undefined
> name
'Brad'
> function hello() {return 'Hello' + name }
undefined
> hello()
'HelloBrad'
>
(To exit, press ^C again or type .exit)
>
Jiamaos-MacBook-Pro:~ Jatin$
```

```javascript 
function doll(name1) { 
console.log(name1); 
}

//doll('jatin'); 

//GLOBAL objects 
console.log(window); 

setTimeout() //
clearTimeout(); //call a function after a delay

setInterval()  // repeatedly call a function after a given delay 
clearInterval(); // stop a function from being called repeatedly 

window.console.log
window.setTimeout(() => {
    
}, timeout);
```


#PRO TIP - when working in VIsual studio code 

`Make sure vim as an extension is not enabeled, when you try to copy code you will leve insert mode and enter into overtype mode.  ` 

1. Short Cut: Shift + I keaves overtype mode
1. Short Cut Command + Shift + P in VS studio code will bring up the path search bar as well as the run command search bar. 

---
# TO BE CONTINUED... Finishing up Node.Js. Will be adding the project created to test node on GITHUB 
---

Avoid defining modules in the global scope. 
We needs modularity instead. 

Modularity = create small building blocks where we define variables and functions, encapsulated inside that module. 

```javascript 
//modules 

var sayHello = function() { 

}
window.sayHello(); 
 // Reference Error: Window is not defined 
 

//IN TERMINAL 
jshint app.js 
//output = 

//Node.js Path Module - Path Mefthod 
const path =require('path'); 
var pathObj = path.parse(__filename); 
console.log(pathObj);

//OutPut 
$ node app.js
{ root: '/',
  dir: '/Users/Jatin/Desktop/first-app',
  base: 'app.js',
  ext: '.js',
  name: 'app' }

os.freemem()  //gets the free memory of the machine 

os.totalmem() //gets the total memory of the machine 

os.userInfo([options]) //information about the current user 

//Loading Os 
const os = require('os'); 

var totalMemory = os.totalmem(); 
var freeMemory = os.freemem(); 
console.log('Total memory: ' +  totalMemory); 

//Template string 
//ES 6 // Es2015 : ECMAScript 6 

console.log(`Total Memory: ${totalMemory}`); 
console.log(`Free Memory: ${freeMemory}`); 

//OUTPUT ON TERMINAL 
$ node app.js
Total memory: 17179869184
Total Memory: 17179869184
Free Memory: 3191939072

Synchronous and blocking 
Asynchronous and non-blocking 

//FILE SYSTEM MODULE -Set of methods for working with files and directories. 
const fs = require('fs'); 

const files = fs.readdirSync('./'); 
console.log(files); 

//on terminal 
node app.js
[ '.DS_Store', '20190808-node-intro.md', 'app.js', 'logger.js' ]

//FILE SYSTEM MODULE -Set of methods for working with files and directories. 
const fs = require('fs'); 

const files = fs.readdirSync('./'); 
console.log(files); 

//OUTPUT on terminal 
node app.js
[ '.DS_Store', '20190808-node-intro.md', 'app.js', 'logger.js' ]


fs.readdir('./', function(err, files) { 
    if (err) console.log('Error', err);
     else console.log('Result', files);
});
Result [ '.DS_Store', '20190808-node-intro.md', 'app.js', 'logger.js' ]

//Simulating an error 
fs.readdir('S', function(err, files) { 
    if (err) console.log('Error', err);
     else console.log('Result', files);
});
//OUTPUT OF THE ERROR (CHANGE THE path to S)
node app.js
[ '.DS_Store', '20190808-node-intro.md', 'app.js', 'logger.js' ]
Error { [Error: ENOENT: no such file or directory, scandir 'S'] errno: -2, code: 'ENOENT', syscall: 'scandir', path: 'S' }

```

## EVENTS MODULE 
A signal that something has happened Class EventEmitter 
```js

const EventEmittter = require('events'); 
const emitter = new EventEmittter(); 

emitter.emit('messageLogged'); 

//A class is a container for related methods and properties. 
//Making a noise, produce - signalling 

//Register a listener 
emitter.on('messageLogged', function() { 
    console.log('Listener called'); 
}); 

//Raise an Event 
emitter.emit('messageLogged'); 

//OUTPUT ON THE TERMINAL 
node app.js
Listener called