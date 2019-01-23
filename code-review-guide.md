### Peer Code Review Guidelines

This document contains important points to check and common mistakes as well as links to further reading. Please read this document carefully. Reading additional materials is optional, but in our opinion will be of big advantage to you.

#### Attitude & Tone
- If you don’t understand any part of the code or have any doubt, don’t hesitate to ask your peer for explanation. This is advantageous both for you and your peer.

- Possible comment formulas
> Please consider refactoring this function  
> TBA

TBA

#### Formatting, Style, Manual Testing

1. Pull-request template
PRs should have proper name (as per task name), should contain link to working demo (if applicable) and to code. Advise your peer to fix or complete missing parts.

1. User interface testing
    - Make sure to test the demo properly (TBA)
    - Please check that all interactive elements are visually indicated (by changing cursor form, background etc.) 

1. Code formatting
    - `console.log` statements should not be left in final version of the code, unless it's part of the functionality

    - Please advise your peer to fix irregular indentations and remove redundant empty lines.

    - Please advise your peer to put newline at the end of every file.

    - Unnecessary comments should be avoided. Advise your peer to find a way to express their intent through expressive variable names or by abstracting part of the code into properly named function.

1. Code style

    - Variable name should be camelCase:  
    ```javascript
    //Before:  
    let my_var, myothervar;

    // After:
    let myVar, myOtherVar;
    ```
    - Variable names should not be too short or too  obscure:
    ```javascript
    //Before: 
    let fns, a, b, cont;

    // After:
    let functionsList, card, rootElement, content;
    ```

    - Variable names should not be too general.
    ```javascript
    //Before: 
    let arr, str;

    // After:
    let cardsList, cardTitle;
    ```

    - If-statement: multiple conditions can often be combined in one condition:
    ```javascript
    //Before: 
    If (a) return;
    If (b) return;

    // After:
    If (a || b) return;
    ```

    - Magic numbers in code should be avoided. For details see [this link](https://stackoverflow.com/questions/47882/what-is-a-magic-number-and-why-is-it-bad).

#### DRY, KISS, SOLID  
Please read carefully about DRY, KISS, SOLID principles and help your peers to find possibilities to apply them.

#### JavaScritp Features  
1. `for` loops, `forEach`, `map` & other iterative forms  
Please pay attention to the content of loop body or callback. Frequent mistake is to make some operation in every iteration, which can be done only once outside loop.

1. `forEach` or `map`? Rule of thumb: if you are using the result of iteration, namely newly created array, use map. if you only need the side-effect of iteration, use forEach. `forEach` says "we don't use the result".

1. Read about the following Array methods on MDN and try to find opportunities to use them:
    - `Array.prototype.find`
    - `Array.prototype.concat`
    - `Array.prototype.includes`
    - `Array.prototype.join`

1. Array function body with brackets & return statement where it is not necessary
    ```javascript
    // Before
    myArray.map(item => { return item.name });

    // After
    myArray.map(item => item.name);
    ```

1. Creating global variables by accident should be avoided. Variables should be always declared with let/const keywords:

    ```javascript
    // Before
    handleClick = (e) => { /* doSomething */ }

    // After
    const handleClick = (e) => { /* doSomething */ }
    ```
1. Missing `“use strict”` directive increases risk of unexpected behavior (except for ES6 modules).

1. Promises & asynchronicity
    - not returning promises
    - using `async`/`await` where Promise is enough

1. Encourage your peers to use more ES6 features  
    - `let`/`const` instead of `var`
    - Destructuring
        ```javascript
        // Before
        `element.addEventListener(‘click’, (e) => { const target = e.target ;  /* do something */})`

        // After
        `element.addEventListener(‘click’, ({ target }) => {  /* do something */})`
        ```
    - Arrow functions for callbacks and other small functions
    - Template literals (especially for string concatenation)

Read more: 
- [Airbnb JavaScript Style Guide](https://github.com/airbnb/javascript)
- ["Exploring ES6"](http://exploringjs.com/es6/)
- ["We have a Problem With Promises"](https://pouchdb.com/2015/05/18/we-have-a-problem-with-promises.html)


#### DOM API
- event delegation
- DOM manipulation in loops (istead of using wrapper elements, document fragment of cloning current container)
- use of `event` global variable instead event handler argument (fails in FireFox)
- Don't use constructions like `children[0]`, `firstElementChild `, `nextSibling`, etc. In such way, you rely on the order of DOM elements. So in case when you will have changed design - your code will be broken. Which is bad, obviously. Use `querySelector` or smth instead.
- Style manipulation through `element.style`
- `keyUp` handles not all input types (try pasting text via context menu instead of typing)