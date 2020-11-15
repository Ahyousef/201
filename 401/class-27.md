# Read 27

## Review

Does a deployed React application require a server?
No, it can use the virtual DOM.
Why do we prefer to test a React application at the behavior rather than the unit level?
Because its a library that has alot of stuff going together, so you just want to test the outcome rather than the process in the background.
What does npm run build do?
Creates an npm build with react library.

## Preview

### setState

We have a search component that displays a search term
That search term is currently empty
The user submits a search term
That term is captured and stored by setState as a value
Reconciliation takes place and React notices the change in value
React instructs the search component to update the value and the search term is merged in

### Handling Events

Handling events with React elements is very similar to handling events on DOM elements. There are some syntax differences:

React events are named using camelCase, rather than lowercase.
With JSX you pass a function as the event handler, rather than a string.
For example, the HTML:
```
<button onclick="activateLasers()">
  Activate Lasers
</button>
is slightly different in React:

<button onClick={activateLasers}>
  Activate Lasers
</button>
```

