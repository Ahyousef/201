# Read 28

## Review

Can a parent component access the state of a child component?
No
What can be passed along in a prop variable?
Everything
How can a child component “know” the state of another component?
Indirectly

## Preview

### The Component Lifecycle
By far the most important concept on this list is understanding the component lifecycle. The component lifecycle is exactly what it sounds like: it details the life of a component. Like us, components are born, do some things during their time here on earth, and then they die .

### Children

What even is ‘children’?
The React docs say that you can use props.children on components that represent ‘generic boxes’ and that ‘don’t know their children ahead of time’. For me, that didn’t really clear things up. I’m sure for some, that definition makes perfect sense but it didn’t for me.
My simple explanation of what this.props.children does is that it is used to display whatever you include between the opening and closing tags when invoking a component.

### Composition vs Inheritance

Containment
Some components don’t know their children ahead of time. This is especially common for components like Sidebar or Dialog that represent generic “boxes”.

We recommend that such components use the special children prop to pass children elements directly into their output:

```
function FancyBorder(props) {
  return (
    <div className={'FancyBorder FancyBorder-' + props.color}>
      {props.children}
    </div>
  );
}
```