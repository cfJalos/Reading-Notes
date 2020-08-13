[Home page](https://cfjalos.github.io/code201-reading-notes/)

# Images,Color,Text #

## Images ##

* A picture can say aThousand words, and great image help make the difference between an average looking site in a really engaging one.

* Images should be relevant, convey information, convey the right mood, instantly recognizable, fit the color palette.

* If you are building a site from scratch, it is good practice to create a folder for all the images the site uses.

### Adding Images ###

```html
<img src="" alt="" title="">
```

* **height** This specifies the height of the image in pixels.

* **width** Specifies the width of the images in pixel.

**Where to place images in your code**

* Before the paragraph

* Inside the start of the paragraph

* In the middle of a paragraph

**align**

* The align attribute was commonly used to indicate how the other parts of a page should flow around an image.**left**,**right**

**Three rule for creating images**

* Save images in the right format

* save images at the right size

* measure image in pixel

**Figure and Figure camption**

```html
<figure> - contain images and their captin so that two are associated.

<figcaption> - to allow web pages authors to add a cation to an images.
```

## Color ##

* The color property allows you to specify the color of text inside an element.


**Hexadecimal notation: #RRGGBB**

* R (red), G (green), B (blue), and A (alpha) are hexadecimal characters (0–9, A–F). A is optional. For example, #ff0000 is equivalent to #ff0000ff.

**Hexadecimal notation: #RGB**

* R (red), G (green), B (blue), and A (alpha) are hexadecimal characters (0–9, A–F). A is optional. The three-digit notation (#RGB) is a shorter version of the six-digit form (#RRGGBB). For example, #f09 is the same color as #ff0099. Likewise, the four-digit RGB notation (#RGBA) is a shorter version of the eight-digit form (#RRGGBBAA).

**Functional notation: rgb(R, G, B[, A])**

* R (red), G (green), and B (blue) can be either numbers or percentages, where the number 255 corresponds to 100%. A (alpha) can be a number between 0 and 1, or a percentage, where the number 1 corresponds to 100% (full opacity).

* background-color - specify the background color of webpages.

## Text ## 

* **Font styles**: Properties that affect the font that is applied to the text, affecting what font is applied, how big it is, whether it is bold, italic, etc.

* **Text layout styles**: Properties that affect the spacing and other layout features of the text, allowing manipulation of, for example, the space between lines and letters, and how the text is aligned within the content box.

* **web safe font** 

* Arial, Corier New, Georgia, Timew New Roman, Verdana, Trebuchet MS

* **Default font**

* serif, sans-serif, monospace, cursive and fantasy

**Font size**

* px: The number of pixels high you want the text to be.

* em: 1 em is equal to the font size set on the parent element of the current element we are styling 

* rem: These work just like em, except that 1 rem is equal to the font size set on the root element of the document 

**Text Alignment**

The **text-align** property is used to control how text is aligned within its containing content box. The available values are as follows, and work in pretty much the same way as they do in a regular word processor application:

* left: Left-justifies the text.
* right: Right-justifies the text.
* center: Centers the text.
* justify: Makes the text spread out,

**Line height**

* The **line-height** property sets the height of each line of text — this can take most length and size units, but can also take a unitless value, which acts as a multiplier and is generally considered the best option — the font-size is multiplied to get the line-height