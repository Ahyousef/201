# Read 16

## Review

- Why is access control important?
    To not authorize everyone to everything, restrict it to ones who should have it.

- Describe an application that would need access control.
    A store needs to have access control for the owner, so not anyone can add items, change prices, etc.
- What is a role used for?
    Define what control goes to types of users.

- Why is role based access control more scalable than discretionary or mandatory access control?

    This way you can make sure certain users have certain access, while others have other access


## Preview

### Event-Driven Programming in Node.js

For the most recognizable example of Event-Driven Programming for people at any level of programming skill, we’ll turn to our old friend The Web Browser.

Every time you interact with a webpage through it’s user interface, an event is happening. When you click a button a click event is triggered. When you press a key a keydown event is triggered. These events have associated functions that, when triggered, are executed to make a change to the user interface in some way.

Event-Driven Programming makes use of the following concepts:

An Event Handler is a callback function that will be called when an event is triggered.
A Main Loop listens for event triggers and calls the associated event handler for that event.


### Node.js

Events
Stability: 2 - Stable
Source Code: lib/events.js

Much of the Node.js core API is built around an idiomatic asynchronous event-driven architecture in which certain kinds of objects (called "emitters") emit named events that cause Function objects ("listeners") to be called.

For instance: a net.Server object emits an event each time a peer connects to it; a fs.ReadStream emits an event when the file is opened; a stream emits an event whenever data is available to be read.

All objects that emit events are instances of the EventEmitter class. These objects expose an eventEmitter.on() function that allows one or more functions to be attached to named events emitted by the object. Typically, event names are camel-cased strings but any valid JavaScript property key can be used.

When the EventEmitter object emits an event, all of the functions attached to that specific event are called synchronously. Any values returned by the called listeners are ignored and discarded.

The following example shows a simple EventEmitter instance with a single listener. The eventEmitter.on() method is used to register listeners, while the eventEmitter.emit() method is used to trigger the event.

