# Reading 1: Node Ecosystem, TDD, CI/CD

## Reading, Research, and Discussion

**1. Why would you want to run JavaScript code outside of a browser?**

A situation in which you'd run JavaScript code **outside of a browser** would be in a **Node** environment - that is, **running JavaScript on the back-end**. This allows you to operate a server to serve your front end, access data in databases, write new data to them, and to interact with APIs.

**2. What is the difference between a module and a package?**

A **module** in Node.js is essentially equivalent to a single JavaScript file. A **package**, on the other hand, is a collection of modules/files wrapped together (much like a library) that developers can download and reuse.

**3. What does the node package manager do?**

The **node package manager**, or **npm**, is a huge registry/repository of open-source software for developers to use in their Node.js projects. It features a command-line utility that makes for simple installation of software packages.

**4. Provide code snippets showing 3 different ways to export a function from a node module.**

    const myFunction = () => {
      console.log('Check out this cool function!');
    };

    exports.myFunction = myFunction;

<!-- -->

    module.exports = function (note) {
      console.log(note);
    };

<!-- -->

    module.exports = function (firstName, lastName) {
      this.firstName = firstName;
      this.lastName = lastName;
    }

## Vocabulary Terms

- `ecosystem`: A network of software, applications, and projects that are centered around/utilize the same programming environment. [Source](https://en.wikipedia.org/wiki/Software_ecosystem).

- `Node.js`: An open-source JavaScript development environment that allows you to write JavaScript on the back-end of an application.

- `V8 Engine`: An open-source JavaScript runtime created by Google written in C++. Powers Google Chrome browser. [Source](https://v8.dev/).

- `module`: A JavaScript file featuring a function or set of functions you want to use in your application. [Source](https://www.w3schools.com/nodejs/nodejs_modules.asp).

- `package`: A collection of modules wrapped together for developers to download and use.

- `node package manager (npm)`: A huge, open-source repository for software to be used in Node.js projects. Free to use and also features a command-line installation tool. [Source](https://www.w3schools.com/whatis/whatis_npm.asp)

- `server`: A piece of hardware or software that "serves" functionality to other programs known as "clients". [Source](<https://en.wikipedia.org/wiki/Server_(computing)>).

- `environment`: A workspace for developers to write and change code without affecting a live application. A base on which programming can be implemented. [Source](https://www.tutorialspoint.com/computer_programming/computer_programming_environment.htm).

- `interpreter`: A program that translates code from a written, human-readable programming language into machine-readable code and instructions (in binary bits). Interpreters convert the code at the time the program is run. [Source](https://www.guru99.com/difference-compiler-vs-interpreter.html).

- `compiler`: A program that translates code from a written, human-readable programming language into machine-readable code and instructions (in binary bits). Compilers convert the code before the program is run. [Source](https://www.guru99.com/difference-compiler-vs-interpreter.html).

### Other Sources

- [Stack Overflow](https://stackoverflow.com/questions/20008442/difference-between-a-module-and-a-package-in-node-js#:~:text=A%20module%20is%20a%20single,has%20metadata%20about%20the%20package.&text=Now%20it's%20very%20common%20for,a%20package%20as%20a%20module.)

- [Sitepoint](https://www.sitepoint.com/understanding-module-exports-exports-node-js/)

- [TutorialsTeacher](https://www.tutorialsteacher.com/nodejs/nodejs-module-exports)