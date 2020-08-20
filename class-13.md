[Home page](https://cfjalos.github.io/code201-reading-notes/)

# Local Storage #

* What we want from Locale Storage 
  * a lot of storage space
  * on the client
  * that persists beyond a page refresh
  * and isn’t transmitted to the server

## HISTORY OF LOCAL STORAGE ##

* Microsoft invented a great many things and included them in their browser-to-end-all-browser-wars, Internet Explorer. One of these things was called DHTML Behaviors, and one of these behaviors was called userData.

* a pattern emerges: all of them are either specific to a single browser, or reliant on a third-party plugin. Despite heroic efforts to paper over the differences (in dojox.storage), they all expose radically different interfaces, have different storage limitations, and present different user experiences. So this is the problem that HTML5 set out to solve: to provide a standardized API, implemented natively and consistently in multiple browsers, without having to rely on third-party plugins.

## HTML5 STORAGE ## 

* a way for web pages to store named key/value pairs locally, within the client web browser. Like cookies, this data persists even after you navigate away from the web site, close your browser tab, exit your browser, or what have you. Unlike cookies, this data is never transmitted to the remote web server (unless you go out of your way to send it manually).

## USING HTML5 STORAGE ## 

* HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats.

  * setItem() method sets the value of the specified Storage Object item.
  * getItem() method returns value of the specified Storage Object item.
  * clear() method removes all the Storage Object item for this domain.
  * removeItem() method removes the specified Storage Object item.