### *Redux - Combined Reducers*

Combined Reducers: pulling in more than one reducer from source and creating a keyed object from them.

There are several important ideas to be aware of when using combineReducers:

First and foremost, combineReducers is simply a utility function to simplify the most common use case when writing Redux reducers. You are not required to use it in your own application, and it does not handle every possible scenario. It is entirely possible to write reducer logic without using it, and it is quite common to need to write custom reducer logic for cases that combineReducer does not handle. (See Beyond combineReducers for examples and suggestions.)

While Redux itself is not opinionated about how your state is organized, combineReducers enforces several rules to help users avoid common errors. (See combineReducers for details.)

One frequently asked question is whether Redux "calls all reducers" when dispatching an action. Since there really is only one root reducer function, the default answer is "no, it does not". However, combineReducers has specific behavior that does work that way. In order to assemble the new state tree, combineReducers will call each slice reducer with its current slice of state and the current action, giving the slice reducer a chance to respond and update its slice of state if needed. So, in that sense, using combineReducers does "call all reducers", or at least all of the slice reducers it is wrapping.

You can use it at all levels of your reducer structure, not just to create the root reducer. It's very common to have multiple combined reducers in various places, which are composed together to create the root reducer.

