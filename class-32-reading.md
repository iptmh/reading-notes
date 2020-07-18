### *Redux - Asynchronous Actions*

## Actions
When you call an asynchronous API, there are two crucial moments in time: the moment you start the call, and the moment when you receive an answer (or a timeout).

Each of these two moments usually require a change in the application state; to do that, you need to dispatch normal actions that will be processed by reducers synchronously. Usually, for any API request you'll want to dispatch at least three different kinds of actions:

An action informing the reducers that the request began.

The reducers may handle this action by toggling an isFetching flag in the state. This way the UI knows it's time to show a spinner.

An action informing the reducers that the request finished successfully.

The reducers may handle this action by merging the new data into the state they manage and resetting isFetching. The UI would hide the spinner, and display the fetched data.

An action informing the reducers that the request failed.

The reducers may handle this action by resetting isFetching. Additionally, some reducers may want to store the error message so the UI can display it.

You may use a dedicated status field in your actions.

## Async Action Creators

The standard way to do it with Redux is to use the Redux Thunk middleware. It comes in a separate package called redux-thunk. By using this specific middleware, an action creator can return a function instead of an action object. This way, the action creator becomes a thunk.

When an action creator returns a function, that function will get executed by the Redux Thunk middleware. This function doesn't need to be pure; it is thus allowed to have side effects, including executing asynchronous API calls. The function can also dispatch actions.
