# Read 02

## Review

1. Why would you want to run JavaScript code outside of a browser?
-  Javascript is a powerful language that you can use to interact with servers and with the system itself, not just the browser, it can run programs like python for example.

2. What is the difference between a module and a package?
-  A package is a group of modules.

3. What does the node package manager do?
-  Organizes modules in place as well as prevent dependencies conflicts.

3. Provide code snippets showing 3 different ways to export a function from a node module
-  ``` module.exports = Fucntion```


## Terms

**ecosystem** : In the context of software development, an ecosystem is a group of software that interacts with each other and have sub-levels that achieve a main goal. Starts from lines of codes all the way up to folders containing multiple files.

**Node.js** : Node.js is an open-source, cross-platform, JavaScript runtime environment that executes JavaScript code outside a web browser.

**V8 Engine** : V8 is Google’s open source high-performance JavaScript and WebAssembly engine, written in C++. It is used in Chrome (javascript) and in Node.js, among others.

**Module** : Reusable file that includes single or libraries of functions.


**Package** : A package is an individual module or a library grouped together.

**NPM** : Node Package Manager is a command line tool that installs, updates or uninstalls Node.js packages in your application. It is also an online repository for open-source Node.js packages.

**Environment** : The place or space that something works and runs, for example NODEjs is a runtime *environment* for javascript

**Interpreter** : Interpreter is a program that executes instructions written in a high-level language. 

**Compiler** : is a computer program that translates computer code written in one programming language into another language.

 ## Preparation Materials

 ### TDD
Test driven development is basically a style of development that uses tests as a way to validate everything is working fine. Using tests also helps recognize which parts of your script are not working normally.

### Inheritance

#### Inheriting properties
JavaScript objects are dynamic "bags" of properties (referred to as own properties). JavaScript objects have a link to a prototype object. When trying to access a property of an object, the property will not only be sought on the object but on the prototype of the object, the prototype of the prototype, and so on until either a property with a matching name is found or the end of the prototype chain is reached.