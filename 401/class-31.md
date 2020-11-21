# Read 31

## Review

Why do we not need more .html pages in a multi-page React app?
Single use app allows us to render multiple pages in just one html file

If we wanted a component to show up on every page, where would we put it and why?
Outside the <BrowserRouter/>
Inside the <BrowserRouter />, outside a <Route />
Inside a <Route />

Inside the browserrouter since we need it to render, but outside the router so it renders in all pages nost just one

What does props.children contain?
everything in the component 

## Preview

### Making sense of hooks

Hooks allow the users to solve the 'seperation of concerns' problem that react has, since you can't breakdown the componenets to their smallest parts, now you can use a hook to make your code more reusable and flow better

### Hooks at a glance

Hooks allow you to keep your functions, instead of turning them into a class everytime you need to set a state, this way you code less and make your code more efficient.
Hooks also allow you to hold multiple variables or just one.
