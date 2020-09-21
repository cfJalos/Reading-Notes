[Home page](https://cfjalos.github.io/Reading-Notes/)
# Online Readings

## [Watch EJS tutorial from WalkThroughCode on YouTube, Videos 1-5](https://www.youtube.com/playlist?list=PL7sCSgsRZ-slYARh3YJIqPGZqtGVqZRGt)

**Video Notes**
* Video Notes
  - First video is an overview of what will be covered in the other videos, which includes:
    * getting started,
    * iterate/loop over an array of values,
    * if/else statements, etc..
  * Getting Started:
   - Do npm init -y to get started, then npm install --save express body-parser cors ejs
   - Then put your code in js file, and putting the vars you need for app, app.use directory, and app.set().
   - Create new ejs folder
   - Then put app.get () function, and app.listen() in js file
   - Doing this we are creating an instance of a server, configuring are express server to run everything through parser, and create a git route for root directory
   - use node server.js to see if its working
  * Injecting value into the view and then how to evaluate that particular value 
    - render takes the view and object of local variables.
    - make foo variable available inside of the view by going to index.js file and put foo in header or whatever element you want to put it in
    - to check out to see if its working and to refresh the page put nodemon
    - you then can pass whatever you want in the js file
  * Loops & Arrays
    - make an unorder list in index.ejs file for an array and put the loop inside of the ul tags with the li part of the list inside of the loop.
  * If/ Else statement
    - go into index.ejs and put the if/ else statement inside of the loop, which is inside of the ul curly brackets with the li's inside of that, just like you would if you were working in a regular JS file.
    
## [Google Books API Docs](https://developers.google.com/books/docs/v1/using#WorkingVolumes)

**Working with volumes**
* Perform a volumes search by sending an HTTP GET request to the following URI: https://www.googleapis.com/books/v1/volumes?q=search+terms
* This request has a single required parameter:
  - q : search for volumes that contain this text string. Special keywords you can specify in the search terms to search in particular fields, such as: intitle, inauthor, inpublisher, subject,  isbn, lccn, and oclc.
* Can use standard query parameters or optional query parameters, such as download, filter, pagination, printType, projection, and sorting.
* Can retrieve information for a specific volume by sending an HTTP GET request to the Volume resource URI: https://www.googleapis.com/books/v1/volumes/volumeId
* accessInfo section - determines what features are available for an eBook. 
* For this you can use standard query parameters or optional query parameter, such as projection.

## [EJS Docs](http://ejs.co/)
**EJS (Embedded JavaScript Templating)**
* EJS - templating language that lets you generate HTML markup with plain JavaScript. 
  - Can use plain JavaScript
  - Fast development time
  - Simple syntax
  - Speedy execution
  - Easy debugging
  - Active development
* EJS features:
  - Fast compilation & rendering
  - Simple template tags
  - Custom delimiters
  - Sub-template included
  - Ships with CLI
  - Both serve JS & browser support
  - Static caching of intermediate JS and templates
  - Complies with the Express view system  

## [EJS Tutorial](https://scotch.io/tutorials/use-ejs-to-template-your-node-application)

**Use EJS to Template Your Node Application**
* Test Application
  - File Structure:
    - views
    ----- partials
    ---------- footer.ejs
    ---------- head.ejs
    ---------- header.ejs
    ----- pages
    ---------- index.ejs
    ---------- about.ejs
    - package.json
    - server.js
  - Node Setup in package.json
    {
    "name": "node-ejs",
    "main": "server.js",
    "dependencies": {
        "ejs": "^1.0.0",
        "express": "^4.6.1"
    }
}
  - Then install npm, and make a index page
  - Define application in server.js file, and set EJS as the view engine for our Express application.
  - Start up server using: $ node server.js
  - EJS Partials - code that is reused in an application. Example files: footer.ejs, head.ejs, header.ejs
  - Pass data to views
  - Echo a single variable
  - Loop over the data
* EJS doesn't support the ability to have layouts. 

## [Source Code for the EJS Tutorial](https://github.com/scotch-io/node-ejs)
* Use this to review code that goes along with the EJS tutorial above to get a better understanding of the code.