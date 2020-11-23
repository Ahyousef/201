# Read 32

## Review

What does a component’s lifecycle refer to?
The time between a component's birth (mount) and death (unmount)
Why do you sometimes need to “wrap” functions in useCallback when called from within useEffect
For efficiency and speed, this way it calls the in-memory function, unless something changed
Why are functional components preferred over class components?
They are easier to read and interpret, since they don't have react details.
What is wrong with the following code?
the for loop
```
import React, {useState, useEffect} from 'react';

function MyComponent(props) {
  const [count, setCount] = useState(0);

  function changeCount(e) {
    setCount(e.target.value);
  }

  let renderedItems = []

  for (let i = 0; i < count; i++) {
    useEffect( () => {
      console.log('component mount/update');
    }, [count]);

    renderedItems.push(<div key={i}>Item</div>);
  }

  return (<div>
     <input type='number' value={count} onChange={changeCount}/>
      {renderedItems}
    </div>);
}
```

## Preview

### useEffect

useEffect can be used when we want to tell react to call the function after the first render or updates.

### async

when wanting to use async, we wrap the function with useEffect, this way we it would work.

