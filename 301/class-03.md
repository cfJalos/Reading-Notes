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

  


