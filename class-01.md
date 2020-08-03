
[Home page](https://cfjalos.github.io/code201-reading-notes/)

# Intro to HTML and Javascript#

### History of HTML ###

* Created in 1989/1990
* Allowed publishing and exchanging of scientific  and technical documents
* Allowed electronic linking of documents via hyperlinks

### The General Rule ###

//<tagName> Some Content </tagName>

### Every HTML document we create will start with this boilerplate ###

```html
<!DOCTYPE html>
<html>
<head>
<!-- Our metadata goes here -->
  <title></title>
</head>
<body>

<!-- Our content goes here -->

</body>
</html>
```

### Comments ###


//<!-- This is a comment.  It doesn't do anything! -->

### Common Tags ###



> //<h1>I'm a header </h1>
> //<h2>I'm a slightly smaller header </h2>
> //<h6>I'm the smallest header </h6>

> //<p>I'm a paragraph</p>

> //<button>I'm a button!</button>

> //<ul>
> //	<li>List Item 1</li>
> //	<li>List Item 2</li>
> //</ul>

> //<ol>
> //	<li>List Item 1</li>
> //	<li>List Item 2</li>
> //</ol>

* [HTML elements reference](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)

### Attributes ### 
Adding Additional Information To Tags

> //<tag name="value"></tag>
> //<img src="corgi.png">

> //<p class="selected">woof woof</p>

> //<a href="www.google.com">Click me to go to Google</a>

> //<link rel="stylesheet" type="text/css" href="style.css">

### Grouping text and Elements in a block ###

```html
The <div> element allows you to group a set of elements together in one block level box.

The <span> element acts like an inline equivalent of the <div> element.
```

### NAVIGATION ###

```html
The <nav> element is used to contain the major navigational blocks on the site such as the primary site navigation.
```

### Article ###

```html
The <article> element act as a container for any selection of a page that could stand alone and potentially be syndicated.
```

### Aside ##

```html
The <aside> element has two purposes, depending on whether it is inside an <article> element or not.
```

### Sections ###

```html
The <section> element groups related content together and typically each section would have its own heading.
```

### Heading group ###

```html
The purpose of the <hgroup> element is to groyp together a set of one or more heading through <h6> elements so that they are treated as one single heading.
```

### MDN Attribute Reference ###

[Attribute MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Attributes)

### Images ###


```html
> //<img src="corgi.png">
```

### Links ###

```html
//<a href="url">Link Text</a
```

### Iframes ###

```html
 <iframe>
```

An **iframe** is like a little window that has been cut into your page and in that window you can see another page. The term iframe is an abbreviation of inline frame.

# Process & Design # 

### Who is the site for? ###

Understand the audience your site may attract and what information they will expect to find on it. Every website should be designed for the target audience- not just for yourself or the site owner. It is therefore very important to understand who your target audience is.

After knowing who are visitor our site. Ask ourselves why are they coming. Most people will visit for a very specific reason.
* Are they looking for general entertainment or do they need to achieve a specific goal?
* If there is a specific goal, is it a personal or professional one? 
* Do they see spending time on this activity as essential or a luxyry?

Now that we know who is coming to our site and why they are coming, work out on what information they need in order to achieve their goals quickly and effectively.

### Get your message across using design ###

Organize information so that visitors can find what they are looking for. The primary aim of any kind of visual design is to communicate. Organizing and prioritizing information on a page helps users understand its importance and what order to read it in.

**CONTENT**

Web pages often have a lot of information to communicate. For example, the pages of online newspapers will have information that does not appear on every page. With so much on the page, the designer needs to **organize** and **prioritize** the information to communicate their message and help users find what they’re looking for.

* **PRIORITIZING**
If everything on a page appeared in the same style, it would be much harder to understand. By making parts of the page look **distinct** from surrounding content, designers draw attention to those items. 

* **ORGANIZING**
**Grouping** together related content into **blocks** or **chunks** makes the page look simpler and easier to understand. User should be able to identify the purpose of each block without processing each individual item. By presenting certain types of information in a s**similar** visual style. Users will learn to associate that style with a particular type of content. 

### Designing Navigation ##

Site navigation not only helps people find where they want to go, but also helps them understand what your site is about and how it is organized. Good navigation tends to follow these principles.

* CONCISE       
* CLEAR
* SELECTIVE
* CONTEXT
* INTERACTIVE
* CONSISTENT

## Javascript basic ##

### How Javascript makes web pages more interactive ###

* Access content

You can use Javascript to select any element, attribute, or text from an HTML page.

* Modify content

Javascript add elements, attributes and text to the page or remove them.

* Program rules

You can specify a set if steos fir tge briwser to follow(like recipe), which allows it to access or change the content of a page.

* React to events

You can specify that a script should run when a specific event has occured.

### Example of Javascript in the browser ###

* Slideshow

* Forms

* Reload part of the page 

* Filtering data

## ABC of programming

* **A**: What is a script and how do i create one?

* **B**: How do computers fit in with the world around them?

* **C**: How do i write a scruot for a web page?

### What is a script and how do i create one? ###

* A script is a series of instructions that a computer can follow to acheve a goal. Series are made up of instructions a computer can follow step by step.

### Writing a script ###

* To write a script you need to first state your goal and then list the task that need to be  completed in order to achieve it.

1. DEFINE THE GOAL

* once you know the goal of your script, you can work out the individual tasks needed to achieve it, This high-level view of the tasks can be represented using a flowchart.

2. DESIGN THE SCRIPT

* Each individual task may be broken down into a sequence of steps. Whten you are ready to code the script, theses steps can tgen be translated into infividual lines of code.

3. CODE EACH STEP

* Every step for every task shown in a flowchart needs to be written in a language the computer can understand and follow.

### EXPRESSIONS ###

* An **expresion evaluates into a single value. Broadly speaking there are two types of expressions.

1. Expressions that just assign a value to a variable

2. Expressions that use two or more values to return a single value.

### Operators ###

* Expressions rely on things called **operators**; they allow programmers to create a single value from one or more values.

```html
* Assignment operators
color = 'biege';

* Arithmetic operators
area = 3 * 2;

* String operators
greeting = 'Hi' + 'Molly'

* Comparison operators
buy = 3 > 5;

* Logical Operators
buy = (5 > 3) && (2 < 4);
```

### Functions ###

* Functions let us wrap bits of code up into REUSABLE packages.  They are one of the building blocks of JS.

```html
function doSomething() {
  console.log("HELLO WORLD");
}
```
then call it
```html
doSomething();
doSomething();
doSomething();
doSomething();
```

* Suppose I want to write code to sing "Twinkle Twinkle Little Star"

```html
console.log("Twinkle, twinkle, little star,");
console.log("How I wonder what you are!");   
console.log("Up above the world so high,");
console.log("Like a diamond in the sky.");
```
* To sing it again, I have to rewrite all the code.  This is not DRY!

```html
console.log("Twinkle, twinkle, little star,");
console.log("How I wonder what you are!");   
console.log("Up above the world so high,");
console.log("Like a diamond in the sky.");
```

* We can write a **function** to help us out

```html
function singSong() {
    console.log("Twinkle, twinkle, little star,");
    console.log("How I wonder what you are!");   
    console.log("Up above the world so high,");
    console.log("Like a diamond in the sky.");
}
```
* To sing the song, we just need to call singSong();

```html
//to sing the entire song 4 times
singSong();
singSong();
singSong();
singSong();
```

### Arguments ###

* Often we want to write functions that take inputs.

```html
function square(num) {
  console.log(num * num);
}
```
* Now when we call square we need to pass in a value

```html
square(10);  //prints 100
square(3);   //prints 9
square(4);   //prints 16
```

* Functions can have as many arguments as needed

```html
function area(length, width) {
  console.log(length * width);
}
area(9,2); //18


function greet(person1, person2, person3){
  console.log("hi " + person1);
  console.log("hi " + person2);
  console.log("hi " + person3);
}
greet("Harry", "Ron", "Hermione");
```

### The Return key word ###

Often we want a function to send back an output value;

* **Input** to **Function** to **Output**

* We use the **return** keyword to output a value from a function

```html
//this function capitalizes the first char in a string:

function capitalize(str) {
  return str.charAt(0).toUpperCase() + str.slice(1);
}

var city = "paris";              //"paris"
var capital = capitalize(city);  //"Paris"

//we can capture the returned value in a variable
```
*  The return keyword stops execution of a function

```html
function capitalize(str) {
  if(typeof str === "number") {
    return "that's not a string!"
  }
  return str.charAt(0).toUpperCase() + str.slice(1);
}

var city = "paris";              //"paris"
var capital = capitalize(city);  //"Paris"

var num = 37;           
var capital = capitalize(num);  //"that's not a string!"

```

### Function Declaration vs. Function Expression ###

```html
//function declaration
function capitalize(str) {
  return str.charAt(0).toUpperCase() + str.slice(1);
}

//function expression
var capitalize = function(str) {
  return str.charAt(0).toUpperCase() + str.slice(1);
}
```