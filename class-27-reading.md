### *Hooks API*

#### Why do custom hooks need the use prefix?
All custom hooks must start with the word “use”. This tells the React linter that it is acceptable for that function to utilize other hook functions inside of it. 
When we have the use work prefixed on our custom hook, React will treat this function differently, allowing the function to return a stateful variable. We don’t need to ever set the value of the stateful variable in our App component, so we only receive the getter and not the setter. This drasitically simplifies our component code.

#### What do custom hooks usually do?
Custom hooks offer the flexibility of sharing logic that wasn’t possible in React components before. We can write custom hooks that cover a wide range of use cases like form handling, animation, declarative subscriptions, timers, etc.

#### Using the links above, list one custom hook that you would be interested in trying/using.
react-fetch-hook
