
[Home page](https://cfjalos.github.io/code201-reading-notes/)

# HTML Links, CSS Layout, JS Function #

### HTML ###

```html
The tags used to produce links are the <a> and </a>.

The <a> tells where the link should start and the </a> indicates where the link ends.

Everything between these two will work as a link.

The target of the link is added to the <a> tag using
the href="http://www.whateverpage.com" setting.


Click <a href="http://www.yahoo.com">here</a> to go to yahoo.
```

### Relative URL ###

* **Same Folder** To link a file in the same folder, just use the file name.

* **Child folder** For a child, use the name of the child folder, followed by a forward slash, then file name.

* **Grandchild Folder** Use the name of the child folder, followed by a forward slash, then the name of the grandchild, followed by another forward slash then the file name.

* **Parent Folder** Use../ to indicate the folder above the current one, then follow it with the file name.

### Email Links ##

```html
<a href="mailto:jon@example.org">Email Jon</a
```

# CSS Layout #

### The Four Schemes

**There are four positioning schemes in CSS positioning:**

* Static

* Absolute

* Relative

* Fixed

All these themes have a specific relationship to normal flow.

**Static Positioning**

* Static positioning is simply placing a box in the normal flow. Because static is the default behavior of an unpositioned box, using the declaration position: static; is comparable to the rule p {text-align: left;}. There's no need to apply a rule that mimics default behavior unless you are overriding another rule.

**Absolute Positioning**

* Absolute positioning absolutely positions a box within its containing block. You can then use any one or combination of left, top, right, and bottom properties to position the box.

**Relative Positioning**

* Relative positioning works differently. Instead of blocks being positioned to their containing block, blocks in relative positioning are positioned to the normal flow. The following CSS sets up the content division to be positioned relatively.

**Fixed Positioning**

* Fixed positioning is calculated in the same way as absolute positioning with respect to containing blocks in that it pulls the positioned box out of the normal flow. In the case of fixed positioning, the fixed reference is the browser viewport.

# JS Functions, Methods, and Objects." 

### Functions ###

* Functions let us wrap bits of code up into REUSABLE packages.  They are one of the building blocks of JS.

```html
function doSomething() {
  console.log("HELLO WORLD");
}
```V
then call it
```htmlV
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

### JavaScript Methods ###
JavaScript methods are actions that can be performed on objects.

A JavaScript method is a property containing a function definition.

**Property**	**Value**
firstName	John