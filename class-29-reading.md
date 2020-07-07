### *Application State with Redux*

#### Why would you wrap your entire application within a context?
With the use of contexts, if your “ancestor” is your <App> component, then every subsequent component is by nature a descendant, and the ancestor -> descendant relationship no longer becomes a major concern.

#### What is the purpose of a reducer?
Reducer functions determine how to update the state. A reducer’s purpose is to take in the current state and an action, and then determine how to modify the state based on the action.

#### What does an action contain?
The action object that was dispatched (containing the action type and payload)

#### Why do we need to copy the state in a reducer?
It is common to begin each reducer function with copying the current state (you can’t mutate / change the state parameter directly) and then running a switch statement based on the type of action.
