HOW TO LINK A CSS PAGE TO HTML 
<link rel="stylesheet" type="text/css" href="selectors.css">

CSS = The "adjectives" of a website 

The General Rule 
    selector { 
        property: value; 
        anotherProperty: value; 
    }

/* Make all h1's purple and 56px font */ 
h1 { 
    color: purple; 
    font-size: 56px; 
}

/* Give all img's a 3px red border */ 
img { 
    border-color; red; 
    border-width 3px; 
}



Write our CSS in a seperate CSS file 

<LINK> tag
<!DOCTYPE html> 
<html> 
<head> 
    <title> Demo Page </title>
    <link rel ="stylesheet" type= "text/css" href="app.css"> 
    </head> 
<body> 

</body> 
</html>

h1{ 
color: pruple; 
}

h3{ 
    color: pink; 
}

MDN Element Reference 

Closing Tags 
<h1> I need a Closing Tag ,h1> 

<p> Me too! </p> 

SELF-Closing TAGS 
<!-- NO closing tag or inner text needed --> 

<img src = "corgi.png"> 

<link href = "style.css"> 

<!-- Don't worry about what these tags do yet --> 


ATTRIBUTES = ADDING additional Information TO Tags 

<tag name> ="value"></tag> 

<img src ="corgi.png"> 
<p class ="selected"> woof wood</p> 
<a href ="wwww.google.com">CLick me to go to Google </a> 
<link rel="stylesheet" type ="text/css" href="style.css"> 

MDN attribute Reference

Images 
<img src = "corgi.png"> 

LINKS 
<a href ="url">Link Text </a> 

<a href ="wwww.google.com">Click me to go to Google</a> 

<a href = "www.reddit.com">Click me to go Reddit </a> 



INLINE STYLE CSS - BAD IDEA THIS WAY
<!DOCTYPE html>
<html> 
    <head> 
        <title> About Me</title>
    </head>
    <h1> About Me</h1>
    <h4> My hobbies:</h4>
    <ul> 
        <li style="color: purple";> Playing Guitar</li>
        <li style ="color: purple";> Cooking</li>
        <li style= "color: purple";>Origami</li>
    </ul>
</html>



USING STYLE TAGS 


<!DOCTYPE html>
<html> 
    <head> 
        <title> About Me</title>
    <style type ="text/css">
/* selector { 
    property: value;   //The element selector, lwet's us select based on the element type
}*/
h1 {
    color: purple;
}
li {
    color:cyan;
}
    </style>

</head>
    <h1> About Me</h1>
    <h1> About Me</h1>
    <h1> About Me</h1>
    <h1> About Me</h1>
    <h4> My hobbies:</h4>
    <ul> 
        <li> Playing Guitar</li>
        <li> Cooking</li>
        <li>Origami</li>
    </ul>
    <head> 
        
    </head>
</html>



COLORS IN CSS 
# + String of hexadecimal numbers(0-F)
```css
h1 { 
    color: #000000;
}
h2 { 
    color: #4B0082;
}
h3{ 
    color: #FF1493; 

}
```css
DECIMAL - BASE 10 
0,1,2,3,4,5,6,7,8,9

999

- - - 
BINARY, - Base 2 
0,1 

- - - 
HEXADECIMAL - Base 16 
0,1,2,3,4,5,6,7,8,9,A,B,C,D,E,F

- - -

# _ _ _ _ _ _ First 2 how much red there is in a color, second 2 how much green, last 2 how much blue 


RGB = 3 Channels Red, Green, and Blue. Each range from 0 - 255 
Full red,green and blue gives us all white, meanwhile 0,0,0 is all black

h1{ 
    color: rgb(0, 255, 0);
}


h2{ 
    color: rgb(100, 0, 100);
}


h3{ 
    color: rgb(11, 99, 150);
}


RGBA = fourth channel which is transparent. Ranges from 0.0 -0.1 
h1{ 
    color: rgba(11,99, 150, 1); 
}

h2{ 
    color: rgba(11, 99, 150, 0.6); 
}

h3{ 
    color: rgba(11, 99, 150, 0.2);  
}

COLOR AND BACKGROUND 

body { 
    background: #95a5a6;
}

div{ 
    background: #3498db;
}

div{ 
    color: #ecf0f1;  
}









/*width 
color 
style */

h1 { 
   color: rgba(0, 200, 100, 0.8); 
   border-color: purple; 
   border-width: 5px;
   border-style: solid; 
}
h1{
border: 9px dashed rgb(255, 100, 80); 
}



CSS Selectors: Element, Id and class 

selector { 
    property: value; 
}

<!DOCTYPE html> 
<html> 
<head> 
    <title> TO DO list </title> 

<head> 

<body> 
    <h1> TO DO List <h1> 
</body> 
<html> 


Element Selector: select all instances of a given element 
<div> 
    <p> You say Yes </p> 
    <p> I say no </p> 
</div> 

<div> 
    <p> You say Goodbye </p> 
    <p> I say Hello </p> 
</div> 


div{ 
    background: purple;
}

p { 
    color: yellow; 

}



    <li id="special"> 
            <input type = "checkbox" > 
            Finish learning CSS 
        </li>

     background: yellow; 
}




id's have a higher specificity that is higher than classes 
Id's will override. 


em is a relative font size.  
by-default if font-size is not set 
1 em = 16px 
2 em = 32 px 
if you set a font-size of 20px on the body element, then 
1 em = 20px 
2em = 40px 
em = desired element pixel value/ parent element font-size in pixels



Font-Weigth certain fonts will let you use a numeric value and that ranges from 100-800px 


Positioning Of Elements
The BOX MODEL: PADDING, MARGIN, BORDER 
    HOW DO WE LAYOUT A PAGE AND MOVE A DIV TO THE TOP RIGHT
    MAKE ANCOR TAG WIDER 
    ADD SPACING BETWEEN IMAGES 

'IN a document, each element is represented as a rectangular box. In CSs, each of these rectangular boxes is described using the standard box model. 
Each box has four exges: the margin edge, border edge,
padding edge, and content edge". 

Blue is the content 
Green is the padding 
Orange is the margin 

Margin auto centers an element for us 

margin 
margin: 100px; 
margin-auto: 500px; 
margin: 20px 40px 500px 100px; 
margin: 0 auto 0 auto; 
margin: 0 auto; 
} 


#one{ 
    background-color: red; 
}

#two{ 
    background-color: blue; 
}

div{ 
    width: 100px;
    float: left;  
}