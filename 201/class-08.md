[Home page](https://cfjalos.github.io/Reading-Notes/)

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

### Layout 

**Normal flow**

* Elements on webpages lay themselves out according to normal flow - until we do something to change that.

**Flexbox**

* Flexbox is a one-dimensional layout method for laying out items in rows or columns. Items flex to fill additional space and shrink to fit into smaller spaces. This article explains all the fundamentals. 
**Floats**

* Originally for floating images inside blocks of text, the float property became one of the most commonly used tools for creating multiple column layouts on webpages. 

**Grids**

* CSS Grid Layout is a two-dimensional layout system for the web. It lets you lay content out in rows and columns, and has many features that make building complex layouts straightforward. 

**Responsive design**

* As more diverse screen sizes have appeared on web-enabled devices, the concept of responsive web design (RWD) has appeared: a set of practices that allows web pages to alter their layout and appearance to suit different screen widths, resolutions, etc. It is an idea that changed the way we design for a multi-device web, and in this article we'll help you understand the main techniques you need to know to master it.

