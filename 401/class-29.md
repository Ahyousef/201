# Read 29

## Review

Do child components have direct access to props/state from the parent?
Yes

When a component “wraps” another component, how does the child component’s output get rendered?

```
<Main>
  <Content />
</Main>
```
it is rendered within the parent

Can a component, such as <Content />, which is a child also be used as a standalone component elsewhere in the application?
Yes

What trick can a parent use to share all props with it’s children
You can use React.children by iritating over the children and cloning them with the props

## Preview

### React Router V4
React Router provides the routing solution to the applications, there are react-router-dom and native, dom is for the web while native is for applications. Now the App should be wrapped with a render, while in the app there should be a router that expects a /router.

### Children

What even is ‘children’?
The React docs say that you can use props.children on components that represent ‘generic boxes’ and that ‘don’t know their children ahead of time’. For me, that didn’t really clear things up. I’m sure for some, that definition makes perfect sense but it didn’t for me.
My simple explanation of what this.props.children does is that it is used to display whatever you include between the openi