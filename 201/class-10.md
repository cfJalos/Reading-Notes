[Home page](https://cfjalos.github.io/Reading-Notes/)

#  JS Debugging #

* A program is crystallized thought. Sometimes those thoughts are confused. Other times, mistakes are introduced when converting thought into code. Either way, the result is a flawed program.

* JavaScript can be made a little more strict by enabling **strict mode**. This is done by putting the string "use strict" at the top of a file or a function body.

## Testing ## 

* Using console.log()

     If the language is not going to do much to help us find mistakes, we’ll have to find them the hard way: by running the program and seeing whether it does the right thing.

     Doing this by hand, again and again, is a sure way to drive yourself insane. Fortunately, it is often possible to write a second program that automates testing your actual program.


## Debugging ## 

Once you notice that there is something wrong with your program because it misbehaves or produces errors, the next step is to figure out **what** the problem is.

* Analyze what is happening and come up with a theory of why it might be happening. Then, make additional observations to test this theory—or, if you don’t yet have a theory, make additional observations that might help you come up with one.

* Putting a few strategic console.log calls into the program is a good way to get additional information about what the program is doing. In this case, we want n to take the values 13, 1, and then 0. Let’s write out its value at the start of the loop.

* An alternative to using console.log is to use the **debugger capabilities of your browser**. Modern browsers come with the ability to set a breakpoint on a specific line of your code. This will cause the execution of the program to pause every time the line with the breakpoint is reached and allow you to inspect the values of variables at that point.


## Exceptions ## 

* When a function cannot proceed normally, what we would like to do is just stop what we are doing and immediately jump back to a place that knows how to handle the problem. This is what exception handling does.

## Assertions ##

Assertions are a tool to do basic sanity checking for programmer errors. Consider this helper function, assert:

```html
function AssertionFailed(message) {
  this.message = message;
}
AssertionFailed.prototype = Object.create(Error.prototype);

function assert(test, message) {
  if (!test)
    throw new AssertionFailed(message);
}

function lastElement(array) {
  assert(array.length > 0, "empty array in lastElement");
  return array[array.length - 1];
}
```

      Mistakes and bad input are facts of life. Bugs in programs need to be found and fixed. They can become easier to notice by having automated test suites and adding assertions to your programs.

      Problems caused by factors outside the program’s control should usually be handled gracefully. Sometimes, when the problem can be handled locally, special return values are a sane way to track them. Otherwise, exceptions are preferable.