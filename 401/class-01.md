# Read 01

## Review

1. Array.map() creates a new array with the same length as the mother-array, and does a certain function on each item.
2. Array.reduce() saves time and effort by accumulating data from each item and return one item at the end.
3. ``` const superagent = require('superagent')  superagent.get(url).then((results) => console.log(results))```
4. ``` async function test(){ let results = await superagent.get(url)}```
5. Promises are tasks that take more than the usual instant tasks, which is why other things are run and it is executed later, basically they need results that take time.
6. All callbacks by default are asynchronous unless programmed otherwise.


## Preview

1. I have previously heard about:
    - NodeJS, now I know that we consider it single-threaded
    - NPM, now I know its basically like an app store for modules
    - Difference between javascript (programming language) and NodeJS (server environment)

2. I want to learn more:
    - Make desktop applications
    - Use frameworks
    - Industry tools

3. React


## Preparation summary

### Node.js intro

#### What is Node.js?
Node.js is an open source server environment
Node.js is free
Node.js runs on various platforms (Windows, Linux, Unix, Mac OS X, etc.)
Node.js uses JavaScript on the server

#### Why Node.js?
Node.js uses asynchronous programming!
A common task for a web server can be to open a file on the server and return the content to the client.

Here is how Node.js handles a file request:

Sends the task to the computer's file system.
Ready to handle the next request.
When the file system has opened and read the file, the server returns the content to the client.
Node.js eliminates the waiting, and simply continues with the next request.

Node.js runs single-threaded, non-blocking, asynchronously programming, which is very memory efficient.

#### What Can Node.js Do?
Node.js can generate dynamic page content
Node.js can create, open, read, write, delete, and close files on the server
Node.js can collect form data
Node.js can add, delete, modify data in your database


### About npm

npm is the world’s largest software registry. Open source developers from every continent use npm to share and borrow packages, and many organizations use npm to manage private development as well

#### Use npm to . . .
Adapt packages of code for your apps, or incorporate packages as they are.
Download standalone tools you can use right away.
Run packages without downloading using npx.
Share code with any npm user, anywhere.
Restrict code to specific developers.
Create Orgs (organizations) to coordinate package maintenance, coding, and developers.
Form virtual teams by using Orgs.
Manage multiple versions of code and code dependencies.
Update applications easily when underlying code is updated.
Discover multiple ways to solve the same puzzle.
Find other developers who are working on similar problems and projects.

 
### Node.Js

Node.js is a JavaScript runtime environment. 

The Node.js run-time environment includes everything you need to execute a program written in JavaScript.

![Node.js](https://www.freecodecamp.org/news/content/images/2019/06/1_sYPllpcAZLHmpuQSRPuO0Q.png)