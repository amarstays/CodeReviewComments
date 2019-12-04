# Javascript

As javascript being a highly evolving language of the day different teams are suck with different capabilities (ES versions) and tools. We will try to list checks considering most recent ES versions and tag then with appropriate ES version.

Any JS Developer / JS Reviewer mush go though Ref [6](#6) / [7](#7).

Checklist Item | Category
-------------- | --------
ES6 - Use of arrow function to avoid .bind() or short hand function definition|Functional Programming
Javascript programs could be build as OOP or FP. Decide one paradigm to use base on the application|General Programming
ES6 - Use of `Template String` instead of concatenation|General Programming
ES6 - Use `let` and `const` over `var`|General Programming
ES6 - Use of `Promises` over `Callbacks`|General Programming
ES7 - Use of `Array.prototype.includes()` for include checks in `Arrays`|General Programming
ES8 - Use of `async\await` over `Promise` for more clear code|General Programming
Avoid undeclared assignments `MyApp = { }`. See ref [1](#1)|General Programming
Avoid the usage of global variables whenever possible|General Programming
If there is a need to access global variable make sure to use most compatible solution ref [2](#2)|General Programming
Avoid use of `typeof "undefined"`, or `=== undefined` checks; plain ! operator works. `(!this.MyApp) this.MyApp = MyApp()` this may represent `global` or `window`|General Programming
Be extra careful about all `typeof` checks other than object type `function` Ref [4](#4)|General Programming
Avoid mixing this/window/global and global variable object|General Programming
Always validate the type of objects passed as callback functions.`if (callback && typeof(callback) === "function"){}`|General Programming
Double check the use of `==` instead of `===`|General Programming
Always cache `Array.length` while looping especially if you accessing DOM|General Programming
Be mindful of Javascript hoisting. Javascript hoisting does not hoist the variable inits|General Programming
Use the configuration object pattern (when using object literal pattern). It provide a cleaner way changing configurations later on compared declarations|General Programming
Application of proper namespaces strategy. Ref [5](#5)|General Programming
Avoid building JSON strings in-memory using string concatenation. Instead use JSON.stringify()|Library
Use lodash/ramda functions instead of implementing itself.|Library
Is Immutable.js was used correct|Library
Any nice/useful library was used which is new|Library

## References

1. http://perfectionkills.com/unnecessarily-comprehensive-look-into-a-rather-insignificant-issue-of-global-objects-creation/
2. https://2ality.com/2016/09/global.html
3. https://gist.github.com/addyosmani/1170518
4. https://javascriptweblog.wordpress.com/2011/08/08/fixing-the-javascript-typeof-operator/
5. https://addyosmani.com/blog/essential-js-namespacing/
6. https://exploringjs.com/
7. https://medium.com/ableneo/testable-javascript-functional-programming-pure-functions-756e049bfd4a