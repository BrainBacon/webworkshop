#JavaScript Introduction

- Node.js
  - Chrome’s V8 Javascript engine in a packaged form
  - npm (node package manager) - dependency management
  - from command line:
    - node myfile.js
    - node will open repl (read-eval-print loop)
- Loosely typed
- comments
  - double slash to comment out until end of line “//”
  - “/*” to open comment block and “*/” to end it.
- operators
  - == (compare) vs === (compare with type)
    - 1 === 1.0 => true
    - undefined === null => false
    - undefined === NaN => false
    - undefined == null => true
  - if
    - if can take any value and every value corresponds to a “truthiness” factor
    - falsy values: 0, undefined, NaN, null, false
    - truthy values: 1, strings, numbers, any defined variable, true
  - standard math expressions:
    - + - / * % (modulus)
  - variables
    - starts with a letter, $, or _
    - functions can be variables! (in the anonymous function form)
- arrays
  - can work like a stack, queue, or linked list
  - .push, .pop, .unshift, etc…
  - bracket notation to access array members
  - myArr[0];
  - can access an undefined value and skip empty positions
  - var myArr = [‘thing’]; myArr[100] = ‘thing2’; myArr[50] => undefined
- objects
  - created via bracket notation
  - var myObj = {foo: ‘bar’}
  - can be treated as maps or trees
  - can have any type as members
  - dot “.” operator to access members
  - access members programmatically with bracket “[ ]” operator
  - myObj[‘foo’]; // variables can be used inside brackets too!
- functions
  - return
    - any type
    - short circuit by returning early
    - returns undefined by default
  - Closures
    - variable context (local vs global)
  - function form
    - function myFn() { … }
  - Anonymous functions
    - var myFn = function() { … }
  - Arguments
    - no type declaration needed
    - can take any number of arguments
        var myFn = function(arg1, arg2) {
             console.log(arg1);
             console.log(arg2);
        };
        myFn(‘one’, ‘two’);
        => ‘one’
        => ‘two’
        myFn(‘one’);
        => ‘one’
        => undefined
    - “arguments” keyword to access arguments object
    - parens operator to run functions “( )”
- loops
  - for(var i = 1; i < 5; i++) { … }
  - while(expression) { … }
- Best practices & recommendations
  - use single quotation
  - use triple equals as much as possible
  - use semicolons
  - use anonymous form of function declaration
  - var myFn = function() { … };
  - ‘use strict’; as the first line of a function
  - https://msdn.microsoft.com/en-us/library/br230269(v=vs.94).aspx
- Browser console (developer tools)
  - Chrome, Firefox Windows: ctrl - shift - i 
  - Chrome, Firefox Mac: cmd - option - i

##Resources
- [Doug Crockford](http://javascript.crockford.com/code.html)
- [MDN (Mozilla Developer Network)](https://developer.mozilla.org/en-US/)
- [Learn JS from Mozilla](https://developer.mozilla.org/en-US/Learn/JavaScript)
- [Plnkr](plnkr.co)
- [JSFiddle](jsfiddle.net)
- [Repl.it](https://repl.it/languages/nodejs)

##Homework
- [Watch Wat](https://www.youtube.com/watch?v=20BySC_6HyY)
- Make a .js file that will run in node and shows all the weird js properties in the video
- Check into git
- Upload to github

##Learn More (extra credit)
- [prototypical inheritance](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Inheritance_and_the_prototype_chain)
- [Linting](http://jshint.com/)
- [Minification](https://github.com/mishoo/UglifyJS)
- [Lodash](https://lodash.com/ )



