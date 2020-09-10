[Home page](https://cfjalos.github.io/Reading-Notes/)
# Mustache and Flexbox

## [Javascript Templating Language and Engine— Mustache.js with Node and Express](https://medium.com/@1sherlynn/javascript-templating-language-and-engine-mustache-js-with-node-and-express-f4c2530e73b2)

### By Sherlynn Tan

## Javascript Templating

* fast and efficient technique to render client-side view templates with Javascript by using a JSON data source. The template is HTML markup, with added templating tags that will either insert variables or run programming logic.

### Mustache

* logic-less template syntax. It can be used for HTML, config files, source code — anything. It works by expanding tags in a template using values provided in a hash or object.

* there are no if statements, else clauses, or for loops. Instead, there are only **tags**.

      Mustache.render(“Hello, {{name}}”, { name: “Sherlynn” });
      // returns: Hello, Sherlynn

* In the above, we see two braces around {{ name }}. This is Mustache syntax to show that it is a placeholder. When Mustache compiles this, it will look for the ‘name’ property in the object we pass in, and replace {{ name }} with the actual value, e,g, “Sherlynn”.



# Flexbox

## [A Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

### From CSS-TRICKS

  - Properties for the Parent

    - display

    - flex-direction

    - flex-wrap

    - flex-flow

    - justify content

    - align-items

    - align-content

 - Properties for the Children

    - order

    - flex-grow

    - flex-shrink

    - flex-basis

    - flex

    - align-self
    
 ##FlexBox Froggy##
 
 **justify-content**

flex-start: Items align to the left side of the container.
flex-end: Items align to the right side of the container.
center: Items align at the center of the container.
space-between: Items display with equal spacing between them.
space-around: Items display with equal spacing around them.

**align-items**

flex-start: Items align to the top of the container.
flex-end: Items align to the bottom of the container.
center: Items align at the vertical center of the container.
baseline: Items display at the baseline of the container.
stretch: Items are stretched to fit the container.

**flex-direction**

row: Items are placed the same as the text direction.
row-reverse: Items are placed opposite to the text direction.
column: Items are placed top to bottom.
column-reverse: Items are placed bottom to top.

**order**

Sometimes reversing the row or column order of a container is not enough. In these cases, we can apply the order property to individual items. By default, items have a value of 0, but we can use this property to also set it to a positive or negative integer value (-2, -1, 0, 1, 2).

**flex-wrap**

nowrap: Every item is fit to a single line.
wrap: Items wrap around to additional lines.
wrap-reverse: Items wrap around to additional lines in reverse.

      The two properties flex-direction and flex-wrap are used so often together that the shorthand property flex-flow was created to combine them. This shorthand property accepts the value of one of the two properties separated by a space.

      For example, you can use flex-flow: row wrap to set rows and wrap them.
  
**align-content**

flex-start: Lines are packed at the top of the container.
flex-end: Lines are packed at the bottom of the container.
center: Lines are packed at the vertical center of the container.
space-between: Lines display with equal spacing between them.
space-around: Lines display with equal spacing around them.
stretch: Lines are stretched to fit the container.




