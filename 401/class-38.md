# Read 38

## Review

How granular should your reducers be?
Reducers should be granular to the extent that you write the least code since some things can be activated twice

Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched
Based on how you code it, it can be a pro if you name common actions when you want them to fire at the same time, con if it was by mistake.
Name a strategy for preventing the above
Be aware of what namings you use


## Preview

### Middleware
In redux, you can use thunk in order to pass states from one group to another, this way you can pass full states from one reducer to another, acting as a middleware.