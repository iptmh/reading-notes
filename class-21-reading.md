### *Component Based UI*

#### What is the benefit of breaking up HTML webpage content into components?
Because the components are modular, they can then be imported, duplicated and shared around multiple files, and thus your application composition can be neatly defined.

#### What is JSX? Why is it useful?
JSX stands for “JavaScript XML”, and refers to React JavaScript files which allow for JavaScript and HTML to be seamlessly mixed together. The only requirement is that the HTML code is enclosed in parentheses ()

#### What can cause a render (or re-render) of a component?
When React sees an element representing a user-defined component, it passes JSX attributes and children to this component as a single object.

#### When a render happens, how is the DOM affected?
Render means to build and display the HTML element(s) on your webpage. When a component is rendered, it appears on the page and within the DOM.

#### What is one thing a framework does that a library doesn’t do?
A library is a collection of tools that you can use to speed up complex development processes. You can call upon those tools wherever you see fit in your application. A framework, on the other hand, sets up rigid places for you to add your code, and the framework is what controls when certain pieces of code are called.
