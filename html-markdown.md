HTML 
HyperText Markup language 
Defines the structure of the web page. 
 1. put an image here 
 1. put a form here 
 The nouns of a webpage. 


CSS
Cascading Style Sheets 
Defines the style of HTML 
1. “make all text purple” 
1.	“give the first image a yellow border” 
The “adjectives” of a webpage 

JAVASCRIPT 
Adds Logic and interactivity to a page 
1.	“Do some math” 
2.	Change color when the user clicks” 
3.	Load new data from twitter 
The actions or “verbs” of a webpage. 



UNIT 3 – HTML 
Write simple HTML documents 
Understand the difference between closing and self-closing tags 
Write tags with attributes
Use MDN as a reference 
Given an image, write the corresponding HTML. 

HISTORY OF HTML = HYPER TEXT MARKUP LANGUAGE
¬¬

Images - HTML 
```html
<img src = “corgi.png’> 

LINKS
<a href= “url”>Link Text</a> 
<a href = "www.google.com"> Click me to go to google</a> 
<a href ="www.reddit.com"> Click me to go to Reddit </a> 
```
Write Validated HTML Forms using <form>, <input>, <select> and <label>


HTML FORMS - GETTING USER INPUT 
1. Use the <form> </form>  tag 
1. Use the <input> tag 
1. Use the <label> </label> tag 
1. Write Simple Validations 

The <form> tag 
<form action= "/my-form-submitting-page" method="post" > 
<! --   All our inputs will go in here -->
</form>


1. Action - the URL to send form data to 
1. method - the type of HTTP request 

//Dumb forms , we need Javascript 


// Mozilla Developer Network Inputs 
 b
The <input> tag 
//The Input tag creates interactive controls. The "type attribute determines the type of input. 
<input type ="text">
<input type ="date">
<input type ="color">
<input type ="file">
<input type ="checkbox">




HTML SKELETON 
<!DOCTYPE html>
<html>

<head> 
<title></title>
</head>

<body>

</body>
</html>


THE FORM TAG 
container where we put our inputs 
Action - where the form send the data too 
Method - what HTTP method (get/post) 


<form> 
    <input name = "username" type ="text" placeholder ="username"> 
    <input name = "password" type ="password" placeholder = "password"> 
    <input type = "submit"> 
</form>


<form>
    <input type = "text" placeholder="username"> 
        <input type = "password" placeholder="password"> 
        <input type = "submit">
</form>



LABELS

<form action = "/sign-in-url" method = "post"> 
<label>username: <input type = "text"></label>
<label>password: <input type = "password"></label>
<button>Login</button>
</form>


Alternative Syntax, using "for" and "id" attributes 
<form action "/sign-in-url" method = "post"> 
<label for = "username"> Username:</label>
<input id ="username"> type = "text"> 
<label for = "password">password:</label>
<input id="password" type ="password">
<button>Login</button>
</form>




REQUIRED ATTRIBUTE 

<!DOCTYPE html> 
<html> 
    <head> 
        <title> Form Demo </title> 
    </head> 
    <body> 
        <h1> LOGIN</h1>

        <!-- action - where the form sends data too -->
        <!-- method - what HTTP method (get/post)-->
<form action="http://www.wikipedia.org">

<label for ="username">Email:</label>
<input id ="username" type="Email" placeholder="username" required>

<label for = "password">Password:</label>
<input id="password" type="password" placeholder="password" required> 

<input type ="submit"> 
</form>
</body> 
</html> 



Background Image = The background property can also set a background image 

body { 
    background: url(http)
}