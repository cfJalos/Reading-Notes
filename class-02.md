[Home page](https://cfjalos.github.io/code201-reading-notes/)

# TEXT #

## Common Tags ##

### Heading ###

```html
<h1>I'm a header </h1>
<h2>I'm a slightly smaller header </h2>
<h6>I'm the smallest header </h6>
```

### Paragraph ###

```html
> //<p>I'm a paragraph</p>
```

### Bold and Italic

```html
<b> this is how we make word appear bold</b>

<i> this is how we make word appear italic</i>
```

### Break and horizontal

```html
<br /> - This is how we add break.

<hr /> - This is how we add Horizontal line.
``` 

### Strong & Emphasis ###

```html
<strong> This is strong </strong>

<em> This is emphasis </em>
```

### Quotations ###

<blockquote> This is block quote </blockquote>

<q> this is double tick quations </q>

### address ###

```html
<address> 742 tacoma way, wa 98367 </address> this is address
```

* HTML are used to describe the structure of the page.

* THey also provide semantice information.

## INTRO TO CSS ##


### What is CSS? ###

* Cascading Style Sheets

### The General Rule ###

```css
selector {
  property: value;
  anotherProperty: value;
}
```
### Where do we write our styles? ###

* Inline

```css
<h3 style="color: pink;">blah blah blah </h3>
<h3 style="color: pink;">knock knock </h3>
<p style="color: yellow;">blah blah blah </p>
```

* Style

```css
<html>
<head>
    <title>About Rusty</title>
    <style type="text/css">
        li {
      color: red;
  }
    </style>
</head>
```

*CSS in a separate CSS file
Using the <link> tag

```css
<!DOCTYPE html>
<html>
<head>
    <title>Demo Page</title>
    <link rel="stylesheet" type="text/css" href="app.css">
</head>
<body>
  
</body>
</html>
```

In our app.css file:

```html
h1 {
  color: purple;
}

h3 {
 color: pink;
}
```

### Closing Tags ###
```html
<h1>I need a closing tag </h1>

<p>Me too!</p>
```

### Self-Closing Tags ###

```html
<!-- No closing tag or inner text needed -->

<img src="corgi.png">

<link href="style.css">

<!-- Don't worry about what these tags do yet -->
```

### Attributes ###

```html
<tag name="value"></tag>

<img src="corgi.png">

<p class="selected">woof woof</p>

<a href="www.google.com">Click me to go to Google</a>

<link rel="stylesheet" type="text/css" href="style.css">
```


# Intro to Javascript #

### Javascript Basics ###

## Primitives ##

5 Primitives Datatypes

```html
//Numbers
4
9.3
-10

//Strings
"Hello World"
"43"

//Booleans
true
false

//null and undefined
null
undefined
```

## Numbers

```html
//Numbers
4
9.3
-10

//We can do some math

4 + 10     //14
1/5        //0.2

//Modulo - remainder operator

10 % 3   //1
24 % 2   //0
15 % 11  //4
```

### Strings ###

```html
//Single or Double quotes OK
"hello world"
'hello world'

//Concatenation
"charlie" + "brown"  //"charliebrown"

//Escape Characters start with "\"
"Singin \"Do wah diddy, diddy, dum diddy do\" "
"This is a backslash: \\"

//Strings have a length property
"hello world".length  //11

//Access individual characters using [] and an index
"hello"[0]  //"h"
"hello"[4]  //"o"
```

### Variables ###

* A script will have to temporarily store the bits of information it needs to do its job. It can store this data in variables.

```html
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
```

### Rules for naming Variables ###

* Name your variables based on the terms of the subject area, so that the variable name clearly describes its purpose.

* Create variable names by deleting spaces that separate the words. Capitalize each word in the name, including prepositions and pronouns that consist of a single letter.

* Do not begin variable names with an underscore.

* Do not use variable names that consist of a single character. Short variable names are only allowed for loop counters.

* Name variables that describe binary states ("true" or "false") after the state that matches the "true" value.


### Null and undefined ###

```html
//The two other primitives are null and undefined

//Variables that are declared but not 
//initialized are undefined
//The following variables are undefined:
var name;
var age;

//null is "explicitly nothing"
var currentPlayer = "charlie";
currentPlayer = null;   //game over
```

### Javascript Built in Methods ###

[Built in Methods](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference)

```html
//alert
alert("Hello there!!!")

//console.log
console.log("Hello from the console!")

//prompt
prompt("what is your name?")
var userName = prompt("What is your name?");
```

### Javascript in a separate file ###

```html
document.write("Good afternoon!")
```

JavaScript is written in plain text, just like HTML and ACSS so you dont need any new tools to write a script.

### Linking to a JavaScript file from an HTML page ###

* When you want to use Javascript with a web page you use the HTML <script> element to tell the browser it is coming across a script.

```html
<!DOCTYPE html>
<html>
    <head>
        <title> Constructive & amp; Co. <title>
        <link rel ="stylesheet" href="css/c01.css" />
    </head>
<body>
    <h1>Constructive &amp; Co.</h1>
    <script src="js/add-content.js"</script>
    <p>For all orders and iquiries please calling <em>555-3344</em></p>
    </body>
</html>
```

### Statements ###

* A script is a series of instructions that a computer can follow one by one. Each individual instruction or step is known as a *statement*. Statements should end with a semicolon.

```html
var today = new Date();
var hourNow = today.getHours();
var greeting;

if (hourNow > 18) {
greeting = 'Good evening';
} else if(hourNow > 12) {
    greeting = 'Good afternoon';
} else if(hourNow > 0) {
    greeting = 'Good afternoon';
} else {
    greeting = 'welcome';
}
document.write(greeting);
```

### Comments ###

* Your comment should explain what your code does. They make your code easier to read and understand. This can help you and others who read your code.

```html
/* qweqweqweqweqweqweqweqweqwe */ this is comment

// qweqweqweqweqwe this is also comment.

