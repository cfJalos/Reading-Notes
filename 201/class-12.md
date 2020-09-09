[Home page](https://cfjalos.github.io/Reading-Notes/)

# Readings : Chart.js, Canvas #

## Canvas ##

* The ****canvas** element

      At first sight a <canvas> looks like the <img> element, with the only clear difference being that it doesn't have the src and alt attributes. Indeed, the <canvas> element has only two attributes, width and height. 

* The **canvas** element can be styled just like any normal image (margin, border, background…). These rules, however, don't affect the actual drawing on the canvas.       

### The rendering context ###

* The canvas element creates a fixed-size drawing surface that exposes one or more rendering contexts, which are used to create and manipulate the content shown. In this tutorial, we focus on the 2D rendering context. 

### Drawing shapes with canvas ###

**Shapes we can draw with Canvas**

* grid
* rectangles
* Drawing paths
* Triangle
* Lines
* Arcs
* Bezier and quadratic curves

### Applying styles and colors ###

If we want to apply colors to a shape, there are two important properties we can use: fillStyle and strokeStyle.

* fillStyle = color
  * Sets the style used when filling shapes.
* strokeStyle = color
  * Sets the style for shapes' outlines.

**Transparency**

* globalAlpha = transparencyValue
  * Applies the specified transparency value to all future shapes drawn on the canvas. The value must be between 0.0 (fully transparent) to 1.0 (fully opaque). This value is 1.0 (fully opaque) by default.

**Patterns**

* createPattern(image, type)
  * Creates and returns a new canvas pattern object. image is a CanvasImageSource (that is, an HTMLImageElement,

**Shadows**

Using shadows involves just four properties:

* shadowOffsetX = float
  * Indicates the horizontal distance the shadow should extend from the object. This value isn't affected by the transformation matrix. The default is 0.
* shadowOffsetY = float
  * Indicates the vertical distance the shadow should extend from the object. This value isn't affected by the transformation matrix. The default is 0.
* shadowBlur = float
  * Indicates the size of the blurring effect; this value doesn't correspond to a number of pixels and is not affected by the current transformation matrix. The default value is 0.
* shadowColor = color
  * A standard CSS color value indicating the color of the shadow effect; by default, it is fully-transparent black.


 ## Drawing text ##

* fillText(text, x, y [, maxWidth])
  * Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.
* strokeText(text, x, y [, maxWidth])
  * Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.


## Styling text ##

* font = value
  * The current text style being used when drawing text. This string uses the same syntax as the CSS font property. The default font is 10px sans-serif.
* textAlign = value
  * Text alignment setting. Possible values: start, end, left, right or center. The default value is start.
* textBaseline = value
  * Baseline alignment setting. Possible values: top, hanging, middle, alphabetic, ideographic, bottom. The default value is alphabetic.
* direction = value
  * Directionality. Possible values: ltr, rtl, inherit. The default value is inherit.
