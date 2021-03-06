# OOP - Classes
You'll rarely use free-standing inheritance manipulation.  What's more common is to wrap prototype manipulations in a function or other syntax for re-use - to dynamically create similar objects, to manage inheritance chains in real-time, for extended functionality.  


boost this

[TOP](#table-of-contents)
___
### Mixins
* add to an object's inheritance chain.  sometimes right, but not usually
* a good idea when you want to have the ability to modify the functionality of a whole lot of objects from one place.  try to avoid needing to do this
* arrow functions don't work well with inheritance, stick to es5.  This has to do with closures, figure out what that is.  
* common vs individual props
* [Mr. Funfunfunction on Inheritance vs Composition](https://medium.com/humans-create-software/composition-over-inheritance-cb6f88070205)
* http://raganwald.com/2015/06/17/functional-mixins.html
* https://medium.com/javascript-scene/functional-mixins-composing-software-ffb66d5e731c

[TOP](#table-of-contents)
___
### Constructor Functions
important for reading mozilla documentation, but not the best practice for your own apps
why avoid them?  because it uses 'this' in confusing ways and needing 'new' makes your code more futurproof. 

constructing constructors
    factory that sets prototype to outside object
    facotry that attaches that object to the function
    constructor - note the subtle differences
    ```js
    outerproto
    function
    addtoouterproto
    
    function.outerproto
    function
    addtoouterproto
    
    constructor
    addtoprototype
    ```

ahttps://sangupta007.wordpress.com/2017/02/12/inheritance-tree-in-javascript/
the diagram, explain it
[TOP](#table-of-contents)
[strange pseud-factory using constructors](https://carldanley.com/js-factory-pattern/)
http://2ality.com/2013/07/defending-constructors.html

[TOP](#table-of-contents)
___
### ES6 Classes 

ES6 introduced a lovely thing called 'classes'.  
If you've never programmed before, they will make your life easy as you begin to learn interitance and OOP modeling in JS. (Easy, not better.) 
If you've already learned how prototypes work in JS you may or may not want to use them, but you'll appreciate the abstraction they provide.  
If you come from a language with true classical inheritance, don't start here.  First learn pure prototypical inheritance then learn how classes work in JS. The name is very misleading, they work nothing like true classes.

 Because this syntax hides what is truely happening, we recommend only using classes once you understand what they do behind the scenes when you can say why they're the best solution.

RESOURCES:
* [Our progressive examples](https://github.com/jankeLearning/content-code/tree/master/Week%2003/classes)
* [How to use them well](https://medium.com/@dan_abramov/how-to-use-classes-and-sleep-at-night-9af8de78ccb4) (skip the react bit at the end of the article.)
* Two from Mozilla herself: [1](https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Classes) [2](https://hacks.mozilla.org/2015/07/es6-in-depth-classes/)
* [very good examples from google](https://github.com/googlechrome/samples/tree/gh-pages/classes-es6)
* [advanced introduction](https://scotch.io/tutorials/better-javascript-with-es6-pt-ii-a-deep-dive-into-classes)
* [friendly introduction](https://ilikekillnerds.com/2015/02/a-guide-to-es6-classes/)
* [fancy things to do with classes](https://www.sitepoint.com/object-oriented-javascript-deep-dive-es6-classes/)
* [Building factories with classes](https://medium.com/@SntsDev/the-factory-pattern-in-js-es6-78f0afad17e9)
* [outstanding video](https://www.youtube.com/watch?v=SS-9y0H3Si8)


[TOP](#table-of-contents)