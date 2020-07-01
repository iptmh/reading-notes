### *Context API*

#### What is the difference between the variables MyContext and MyProvider in the examples above?
The class component MyProvider which creates the state variables, and the context object, MyContext. This context object is what does the work of sharing the state variables out. Even though our class component is named “provider”, the context object is what creates the provider behavior.

#### Why is context useful?
By using the Context API, a provider can send the state directly to any descendant. Without using context, the provider could only send the state to components directly in the render function of the provider. This means that components defined or used elsewhere would need to have the state passed down in a chain of parent-child props.

#### Can a component outside of a provider get its context?
Using the React “Context API”, we can create and manage state in a more “global” fashion. This allows you to expost the state variables you care about to your entire application.
