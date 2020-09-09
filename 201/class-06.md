[Home page](https://cfjalos.github.io/Reading-Notes/)

# Object literals #

* A JavaScript object literal is a comma-separated list of name-value pairs wrapped in curly braces. Object literals encapsulate data, enclosing it in a tidy package. This minimizes the use of global variables which can cause problems when combining code.

```html
var myObject = {
    sProp: 'some string value',
    numProp: 2,
    bProp: false
};
```

### Object literals are defined using the following syntax rules: ###

* A colon separates property name from value.
* A comma separates each name-value pair from the next.
* There should be no comma after the last name-value pair.

**Why and How We Use Object Literals**

* Several JavaScripts from dyn-web use object literals for setup purposes. Object literals enable us to write code that supports lots of features yet still provide a relatively straightforward process for implementers of our code. No need to invoke constructors directly or maintain the correct order of arguments passed to functions. Object literals are also useful for unobtrusive event handling; they can hold the data that would otherwise be passed in function calls from HTML event handler attributes.

## Document Object Model ##

**The DOM**  Document Object Model

* The Document Object Model is the interface between your Javascript and HTML+CSS

* *The browser turns every HTML tag into a Javascript object that we can manipulate*

* *Everything is stored inside of the document object*

### The Process ###

* SELECT an element and then MANIPULATE

  * For our example, we'll change the <h1> color using JS

  ```html
  var h1 = document.querySelector("h1");

  h1.style.color = "pink";

  var body = document.querySelector("body"); //SELECT

  var isBlue = false;

  setInterval(function(){   //MANIPULATE
  if (isBlue) {
    body.style.background = "white";
  } else {
    body.style.background = "#3498db";
  }
  isBlue = !isBlue;
  }, 1000);
  ```

### DOM Selectors ###

* Document
It all starts with the document, the root node

* Methods
  * document.getElementById()
  * document.getElementsByClassName()
  * document.getElementsByTagName()
  * document.querySelector()
  * document.querySelectorAll()

getElementById -  Takes a string argument and returns the one element with a matching ID.

getElementsByClassName - Takes a string argument and returns a list of elements that have a matching class.

getElementsByTagName - Returns a list of all elements of a given tag name, like li or h1.

getElementsByTagName - Returns a list of all elements of a given tag name, like li or h1.

querySelector - Returns the first element that matches a given CSS-style selector.

querySelectorAll - Returns a list of elements that matches a given CSS-style selector

### Style ###

* The style property is one way to manipulate an element's style

```html
/SELECT
var tag = document.getElementById("highlight");

//MANIPULATE
tag.style.color = "blue";
tag.style.border = "10px solid red";
tag.style.fontSize = "70px";
tag.style.background = "yellow";
tag.style.marginTop = "200px";
```

* classList

```html
var tag = document.querySelector("h1");

//ADD A CLASS TO THE SELECTED ELEMENT
tag.classList.add("another-class");

//REMOVE A CLASS
tag.classList.remove("another-class");

//TOGGLE A CLASS
tag.classList.toggle("another-class");
```

* textContent

```html
/Select the <p> tag:
var tag = document.querySelector("p");

//Retrieve the textContent:
tag.textContent //"This is an awesome paragraph"

//alter the textContent:
tag.textContent = "blah blah blah";
```

* innerHTML - Similar to textContent, except it returns a string of all the HTML contained in a given element

```html
//Select the <p> tag:
var tag = document.querySelector("p");

tag.innerHTML
//"This is an <strong>awesome</strong> paragraph"
```

* Attributes - Use getAttribute() and setAttribute() to read and write attributes like src or href

```html
var link = document.querySelector("a");
link.getAttribute("href");  //"www.google.com"
//CHANGE HREF ATTRIBUTE
link.setAttribute("href","www.dogs.com"); 
///<a href="www.dogs.com">I am a link</a>

//TO CHANGE THE IMAGE SRC
var img = document.querySelector("img");
img.setAttribute("src", "corgi.png");
//<img src="corgi.png">
```

