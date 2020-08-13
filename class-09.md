[Home page](https://cfjalos.github.io/code201-reading-notes/)

# Forms and JS Events # 

## Forms ##

**Forms** allow users to perform other functions online. You will see forms when registering as a member of a website, when shopping online, and when signing up for newsletters or mailing list.

* The best know fom on the web is probably the search box that sits right in the middle of Google's Homepage.

**Form controls**

* Adding Text
  * Text input 
  * Password input
  * Text Area

* Making CHoices
  * Radio Buttons 
  * Checkboxes
  * Drop down boxes

* Submitting Forms
  * Submit buttons
  * Image buttons
  * File upload

**How forms work**

1. User fills in a form and then presses a button to submit the information to the server.
2. The name of each form control is sent to the server along with the value the user enters or selects.
3. The server process the information using a programming language such as PHP C# VB.net, or JAVA. It may also store the information in a database.
4. The server creates a new page ti send back to the browser based on the information received.

**NAME = VALUE**

### Form Structure ###

      The <form> element formally defines a form and attributes that determine the form's behavior. Each time you want to create an HTML form, you must start it by using this element, nesting all the contents inside. Many assistive technologies and browser plugins can discover <form> elements and implement special hooks to make them easier to use.

      The <fieldset> element is a convenient way to create groups of widgets that share the same purpose, for styling and semantic purposes. 

      <legend> element represents a caption for the content of its parent <fieldset>.

      <label> element represents a caption for an item in a user interface.

      <input> element is used to create interactive controls for web-based forms in order to accept data from the user; a wide variety of types of input data and control widgets are available, depending on the device and user agent.

      <textarea> element represents a multi-line plain-text editing control, useful when you want to allow users to enter a sizeable amount of free-form text, for example a comment on a review or feedback form.

      <select> element represents a control that provides a menu of options:

**Type	Description**

```html
<input type="text">	Displays a single-line text input field
<input type="radio">	Displays a radio button (for selecting one of many choices)
<input type="check">	Displays a checkbox (for selecting zero or more of many choices)
<input type="submit">	Displays a submit button (for submitting the form)
<input type="button">	Displays a clickable button
```

## Lists ##

* The **list-style-type** CSS property sets the marker (such as a disc, character, or custom counter style) of a list item element.

* The **list-style-image** CSS property sets an image to be used as the list item marker.

* The **list-style-position** CSS property sets the position of the ::marker relative to a list item.

* The **list-style** CSS shorthand property allows you set all the list style properties at once.

## Table Properties ## 

**align** 
* This enumerated attribute indicates how the table must be aligned inside the containing document. It may have the following values:

  * left: the table is displayed on the left side of the document;
  * center: the table is displayed in the center of the document;
  * right: the table is displayed on the right side of the document.
  * Set margin-left and margin-right to auto or margin to 0 auto to achieve an effect that is similar to the align attribute.

**bgcolor** 
* The background color of the table. It is a 6-digit hexadecimal RGB code, prefixed by a '#'. One of the predefined color kewords can also be used.

  * To achieve a similar effect, use the CSS background-color property.

**border**
* This integer attribute defines, in pixels, the size of the frame surrounding the table. If set to 0, the frame attribute is set to void.

  * To achieve a similar effect, use the CSS border shorthand property.

**cellpadding** 
* This attribute defines the space between the content of a cell and its border, displayed or not. If the cellpadding's length is defined in pixels, this pixel-sized space will be applied to all four sides of the cell's content. If the length is defined using a percentage value, the content will be centered and the total vertical space (top and bottom) will represent this value. The same is true for the total horizontal space (left and right).

      To achieve a similar effect, apply the border-collapse property to the <table> element, with its value set to collapse, and the padding property to the <td> elements.

**cellspacing**

* This attribute defines the size of the space between two cells in a percentage value or pixels. The attribute is applied both horizontally and vertically, to the space between the top of the table and the cells of the first row, the left of the table and the first column, the right of the table and the last column and the bottom of the table and the last row.

      To achieve a similar effect, apply the border-spacing property to the <table> element. border-spacing does not have any effect if border-collapse is set to collapse.

**frame** 
* This enumerated attribute defines which side of the frame surrounding the table must be displayed.

  * To achieve a similar effect, use the border-style and border-width properties.

**rules** 
* This enumerated attribute defines where rules, i.e. lines, should appear in a table. It can have the following values:

      none, which indicates that no rules will be displayed; it is the default value;
      groups, which will cause the rules to be displayed between row groups (defined by the <thead>, <tbody> and <tfoot> elements) and between column groups (defined by the <col> and <colgroup> elements) only;
      rows, which will cause the rules to be displayed between rows;
      columns, which will cause the rules to be displayed between columns;
      all, which will cause the rules to be displayed between rows and columns.
      To achieve a similar effect, apply the border property to the appropriate <thead>, <tbody>, <tfoot>, <col>, or <colgroup> elements.

**summary** 
      This attribute defines an alternative text that summarizes the content of the table. Use the <caption> element instead.
**width** 
This attribute defines the width of the table. Use the CSS width property instead.

## EVENTS ##

**events** are actions or occurrences that happen in the system you are programming — the system produces (or "fires") a signal of some kind when an event occurs, and also provides a mechanism by which some kind of action can be automatically taken (that is, some code running) when the event occurs.

There are a lot of different types of events that can occur, for example:

* The user clicking the mouse over a certain element or hovering the cursor over a certain element.
* The user pressing a key on the keyboard.
* The user resizing or closing the browser window.
* A web page finishing loading.
* A form being submitted.
* A video being played, or paused, or finishing play.
* An error occurring.

      addEventListener() and removeEventListener()
The newest type of event mechanism is defined in the Document Object Model (DOM) Level 2 Events Specification, which provides browsers with a new function — **addEventListener()**. This functions in a similar way to the event handler properties, but the syntax is obviously different. 

      Event objects

*  inside an event handler function, you might see a parameter specified with a name such as event, evt, or simply e. This is called the **event object**, and it is automatically passed to event handlers to provide extra features and information.      

      Preventing default behavior

* preventDefault() function on the event object — which stops the form submission — and then display an error message in the paragraph below our form to tell the user what's wrong.

