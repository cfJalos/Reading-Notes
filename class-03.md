
[Home page](https://cfjalos.github.io/code201-reading-notes/)
# HTML Lists, CSS Boxes, JS Control Flow #

## HTML Lists ##

* An **Ordered list** created using the ol element, and each list item starts with the li element. Ordered lists are used when the order of the list's items is important. The list items in an ordered list are marked with numbers.

```html
<ol>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>
```

*  An **Unordered list** is a collection of related items that have no special order or sequence. This list is created by using HTML ul tag. Each item in the list is marked with a bullet.

```html
<ul>
  <li>Beetroot</li>
  <li>Ginger</li>
  <li>Potato</li>
  <li>Radish</li>
</ul>
```      

* **definition list** is a list of terms and corresponding definitions. Definition lists are typically formatted with the term on the left with the definition following on the right or on the next line.

```html
<dl>
  <dt>Definition List</dt>
  <dd>A list of terms and their definitions/descriptions.</dd>
  <dt>HTML</dt>
  <dd>An HTML tutorial.</dd>
  <dt>PHP</dt>
  <dd>An PHP tutorial.</dd>
</dl>
```

## Boxes ##

* The CSS box model is essentially a box that wraps around every HTML element. It consists of: margins, borders, padding, and the actual content. The image below illustrates the box model

* Content - The content of the box, where text and images appear
* Padding - Clears an area around the content. The padding is transparent
* Border - A border that goes around the padding and content
* Margin - Clears an area outside the border. The margin is transparent

**Example**

```html
div {
  width: 300px;
  border: 15px solid green;
  padding: 50px;
  margin: 20px;
}
```
## Basic Javascript Instruction ##

* An **Array** is a special type of variable. It doesnt just store one values;it stores a list of values.

```html
var colors;
colors = ['white','red','blue'];

Index 0 = 'white'
Index 1 = 'red'
Index 2 = 'blue'

colors[0] = 'white'
colors[1] = 'red'
colors[2] = 'blue'
```

## Conditional Statements ##

Use **if** to specify a block of code to be executed, if a specified condition is true
Use **else** to specify a block of code to be executed, if the same condition is false
Use **else if** to specify a new condition to test, if the first condition is false
Use **switch** to specify many alternative blocks of code to be executed

## JavaScript Data Types ##

```html
var length = 16;                               // Number
var lastName = "Johnson";                      // String
var x = {firstName:"John", lastName:"Doe"};    // Object
true || false;                                 // Boolean
null                                           // Empty Value
undefined                                      // variable without assigned value
```

### Loops ###

* Loops check a condition. If it returns true, a code of block will run.

* **for loops**

```html
for (var i = 0; i < 10; i++) {
  document.write(i);
}
```
* **The While Loop**
The while loop loops through a block of code as long as a specified condition is true.
```html
while (condition) {
  // code block to be executed
}
```