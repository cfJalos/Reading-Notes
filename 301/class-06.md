# NODEJS

## DEFINITION ##

NodeJS is an open source platform and a runtime environment for executing JavaScript code outside of a browser.
Single-threaded language which in background uses multiple threads to execute asynchronous code
It is also event-driven, meaning all that happens in Node is in response to an event

## APPLICATION ##

Build back-end services (API)
Client apps such as web app and mobile app use these services to store data, send emails or push notifications and etc.
Highly scalable, data-intensive and real-time apps
Real-time chat app
CodeShare

## ADVANTAGES OF NODEJS ##

Great for prototyping and agile development
Superfast and highly scalable services (paypal, uber, Netflix)
More optimized programming codes
Faster response time
It uses JavaScript everywhere and has excellent support for the modern language

      function upcase(strings, ...values) {
        return values.map(name => name[0].toUpperCase() + name.slice(1))
          .join(' ') + strings[2];
      }
 
      const person = {
        first: 'brendan',
        last: 'eich',
        age: 56,
        position: 'CEO of Brave Software',
      };
 
      const { first, last } = person;
      const emoticon = [ ['┌', '('], ['˘', '⌣'], ['˘', ')', 'ʃ'] ];
      
      console.log(
        upcase`${first} ${last} is the creator of JavaScript! ` + emoticon.flat().join('')
      );

Save it to a file named index.js and run it in the terminal node index.js and output would be 
Brendan Eich is the creator of JavaScript! ┌(˘⌣˘)ʃ

Cleaner and more consistent codebase (same naming convention, same tools, same best practices)
Large ecosystem of open-source libraries
The execution model of the node creates very little overhead for the server and thus it is able to manage a large number of simultaneous connections.
DISADVANTAGE OF NODEJS

Have limitations such as user should avoid:
blocking I/O calls
CPU-intensive operations and should be handed off to a worker thread
Errors that are not handled correctly (might crash the entire process)


## INSTALLATION AND VERIFICATION ##

Globally
Open your terminal and type the following npm install -g jshint


Locally
We can also install packages locally to a project, as opposed to globally, on our system. Create a test folder and open a terminal in that directory. 
Next type this: npm init -y
This will create and auto-populate a package.json file in the same folder. Next, use npm to install the lodash package and save it as a project dependency: npm install lodash –save
Create a file named test.js and add the following: 
        const _ = require('lodash');
const arr = [0, 1, false, 2, '', 3];
console.log(_.compact(arr));
Finally, run the script using node test.js. You should see [ 1, 2, 3 ] output to the terminal.
Verification
Type in the terminal node -v and the output would display out v12.14.1
Cloning
If you open the packet.json file you will see lodash listed below the field of dependencies. By specifying the dependencies of your project in this way, you allow any developer to clone your project anywhere, and use npm to install any packages that you need to run.

EXAMPLE – Hello World Server Version

      const http = require('http'); 
      
      http.createServer((request, response) => { 
        response.writeHead(200);
        response.end('Hello, World!');
      }).listen(3000);
 
console.log('Server running on http://localhost:3000');NODEJS

DEFINITION

NodeJS is an open source platform and a runtime environment for executing JavaScript code outside of a browser.
Single-threaded language which in background uses multiple threads to execute asynchronous code
It is also event-driven, meaning all that happens in Node is in response to an event

APPLICATION

Build back-end services (API)
Client apps such as web app and mobile app use these services to store data, send emails or push notifications and etc.
Highly scalable, data-intensive and real-time apps
Real-time chat app
CodeShare

ADVANTAGES OF NODEJS

Great for prototyping and agile development
Superfast and highly scalable services (paypal, uber, Netflix)
More optimized programming codes
Faster response time
It uses JavaScript everywhere and has excellent support for the modern language

function upcase(strings, ...values) {
  return values.map(name => name[0].toUpperCase() + name.slice(1))
    .join(' ') + strings[2];
}
 
const person = {
  first: 'brendan',
  last: 'eich',
  age: 56,
  position: 'CEO of Brave Software',
};
 
const { first, last } = person;
const emoticon = [ ['┌', '('], ['˘', '⌣'], ['˘', ')', 'ʃ'] ];
 
console.log(
  upcase`${first} ${last} is the creator of JavaScript! ` + emoticon.flat().join('')
);

Save it to a file named index.js and run it in the terminal node index.js and output would be 
Brendan Eich is the creator of JavaScript! ┌(˘⌣˘)ʃ

Cleaner and more consistent codebase (same naming convention, same tools, same best practices)
Large ecosystem of open-source libraries
The execution model of the node creates very little overhead for the server and thus it is able to manage a large number of simultaneous connections.
DISADVANTAGE OF NODEJS

Have limitations such as user should avoid:
blocking I/O calls
CPU-intensive operations and should be handed off to a worker thread
Errors that are not handled correctly (might crash the entire process)


INSTALLATION AND VERIFICATION

Globally
Open your terminal and type the following npm install -g jshint


Locally
We can also install packages locally to a project, as opposed to globally, on our system. Create a test folder and open a terminal in that directory. 
Next type this: npm init -y
This will create and auto-populate a package.json file in the same folder. Next, use npm to install the lodash package and save it as a project dependency: npm install lodash –save
Create a file named test.js and add the following: 
const _ = require('lodash');
const arr = [0, 1, false, 2, '', 3];
console.log(_.compact(arr));
Finally, run the script using node test.js. You should see [ 1, 2, 3 ] output to the terminal.
Verification
Type in the terminal node -v and the output would display out v12.14.1
Cloning
If you open the packet.json file you will see lodash listed below the field of dependencies. By specifying the dependencies of your project in this way, you allow any developer to clone your project anywhere, and use npm to install any packages that you need to run.

EXAMPLE – Hello World Server Version

const http = require('http'); 
 
http.createServer((request, response) => { 
  response.writeHead(200);
  response.end('Hello, World!');
}).listen(3000);
 
console.log('Server running on http://localhost:3000');

createServer - method to create a new web server object
request, response - contain the request from the user and the response, which we use to send back a 200 HTTP status code, along with our “Hello World!” message.
listen - server to listen for incoming requests on port 3000, and output a message to the terminal to let us know it’s running.

To run this, copy the code into a file named hello-world-server.js and run it using node hello-world-server.js. Open up a browser and navigate to http://localhost:3000 to see “Hello, World!” displayed in the browser.

