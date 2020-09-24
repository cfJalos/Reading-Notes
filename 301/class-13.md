# Online Readings

## [Sending Form Data](https://developer.mozilla.org/en-US/docs/Learn/HTML/Forms/Sending_and_retrieving_form_data)

**Sending Form Data**
* Client/server architecture
  - A client (usually a web browser) sends a request to a server (most of the time a web server, using the HTTP protocol. The server answers the request using the same protocol.
  - HTML form on a web page is a convenient user-friendly way to configure an HTTP request to send data to a server. This enables the user to provide information to be delivered in the HTTP request.
* Client side: defining how to send the data
  - form element defines how the data will be sent.
  - Its attributes are designed to let you configure the request to be sent when a user hits a submit button. Attributes: action and method.
  - Action attribute defines where the data gets sent. Its value must be a valid relative or absolute URL. The names and values of the non-file form controls are sent to the server as name=value pairs joined with ampersands.
      * Action value should be a file on the server that can handle the incoming data. The server then responds, generally handling the data and loading the URL defined by the action attribute, causing a new page load.
  - Method attribute defines how data is sent. HTML form data can be transmitted via a number of different methods, the most common being the GET method and the POST method.
  -  GET method - the method used by the browser to ask the server to send back a given resource.
  - POST method - the method the browser uses to talk to the server when asking for a response that takes into account the data provided in the body of the HTTP request.
* HTTP requests are never displayed to the user.
* Server side: retrieving the data
  - The server receives a string that will be parsed in order to get the data as a list of key/value pairs. The way you access this list depends on the development platform you use and on any specific frameworks you may be using with it.
  - PHP offers some global objects to access the data.
* Languages and frameworks
  - Django for Python
  - Express for Node.js
  - Laravel for PHP
  - Ruby On Rails for Ruby.
* Sending files with HTML forms: Files are binary data because HTTP is a text protocol.
  - Enctype attribute - lets you specify the value of the Content-Type HTTP header included in the request generated when the form is submitted. HTTP header tells the server what kind of data is being sent.
* Security issues
  - HTML forms are the most common server attack vectors, but its due to how the server handles data.
  - Never trust your users. All data that comes to your server must be checked. Escape potentially dangerous characters. Limit the incoming amount of data to allow only what's necessary. Sandbox uploaded files.

## [HTML5 Forms Reference](https://htmlreference.io/forms/)

**HTML5 Forms Reference**
* 

## [Video Series on Styling HTML5 Forms](https://www.youtube.com/playlist?list=PL4cUxeGkcC9g5_p_BVUGWykHfqx6bb7qK)

**Forms in HTML5**
* Button - defines a clickable button. Attributes: 
  - name = "submit_button"
  - value = "primary"
  - type = "submit" or "reset"
  - disabled - disables button
  - autofocus - sets focus on element when page loads
* Fieldset - defines a group of controls within a form. Attribute:
  - Disabled - disables the controls the fieldset contains
* Form - defines an interactive form with controls. Attributes:
  - action - defines which URL the form's information is sent to when submitted. With "/contact" you can use a relative URL. Or you can use this "https://htmlreference.io/contact", which is an absolute URL.
  - method - defines the HTTP method used when submitting the form. "post" is the form information is sent to the server as part of the request body. "get" is the form information is sent to the server as part URL parameters: /contact?first_name=Alex&last_name=Smith.
  - name = "sign_up_form"
  - autocomplete = "off" or "on"
  - target = "_blank", "_self", "_parent", or "_top"
  - enctype = "application/x-www-form-urlencoded", "text/plain", or "multipart/form-data"
  - novalidate - tells the browser to not validate the form on submission
* input - defines an interactive control within a web form. Attributes:
  - type - defines the type of form input
  - name - defines the unique identifier for that input within the form
  - placeholder - defines a non-selectable placeholder text that only appears when the input is empty
  - required - tells the browser that this input is required 
  - disabled - disables the input
* legend - defines a caption for a parent's content. 
* textarea - defines a multi-line text control within a web form. Attributes:
  - name - defines the unique identifier for that textarea within the form 
  - autocomplete - determines if the browser can autocomplete the textarea
  - minlength - defines the minimum amount of characters the textarea required to be valid
  - maxlength - defines the maxlength amount of characters allowed
  - placeholder - defines a non-selectable placeholder text that only appears when the textarea is empty
  - cols - defines the number of columns
  - rows - defines the number of rows
  - wrap - defines how the text should be wrapped
  - disabled - disables the textarea
  - required - tells the browser that this textarea is required
  - autofocus - sets focus on the textarea when the web page loads
  - readonly - turns the textarea into a read-only element
  - spellcheck - enables the browser spell checker

**Styling HTML5 Forms**
* Video Notes
  - Will be going over radio buttons, checkboxes, fieldset, text input, select boxes, and input validation styles in HTML and CSS.
  - For the CSS of base form styles give the body background-color, magin of 0, font-family. Next style the header with background-color, padding, and text-align: center. After that do the form, put margin and color. Then stylize the form p with font-size and letter-spacing.
  - For the radio buttons styling work on the input with the type radio, and give it opacity, width, and margin. Next work on the labels for each button, and give it a margin-bottom, display-inline: block, padding-left, background: url(url) no-repeat, background-position, line-height, and cursor :pointer. Next style the input:checked + label[for =""] with background-position and color.
  - For the checkboxes styling work first style the input type with opacity, width, and margin. Next work on the labels for each checkbox, and give it display: inline-block, margin-bottom, padding-left, background: url(url) no-repeat, background-position, line-height, and cursor :pointer. Next style the input:checked + label[for =""] with background-position and color.
  - For the text inputs and flield set. Tag the flieldset and style it with padding, margin, and border. Then do the legend, and style it with padding, font-size, and letter-spacing.
  In the input styling put all of the type of the input you are working on, and then style it with display, margin-bottom, padding, border-radius, border, background: url(image) no-repeat for the icon images, background-color, font-size, and color. Next choose the specific output type you want to style, and give it a different background color.
  - Styling select boxes by first choosing the select element and style it with -webkit-appearance: none, -moz-appearance: none, -o-appearance:none, -ms-appearance:none, appearance: none, display: block, margin, padding, background: url(img) no-repeat % center, background-color, color, border-radius, border, and width. Then style the button with the input style of the button, and give it a background, padding, color, fon-size, letter-spacing, border-radius, border: 0, box-shadow, and width.
  - Validation styles for inputs using a valid psudo-class. First give the input a type and psudo-class of valid for all the inputs you are working on. Give these a border. Then give one of the spefic input types a backgound position, and do the same for the other one. Then finish give the input types that are valid a styling of background:url, background-color, fon-size, color, float: left, and clear:both.