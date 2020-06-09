### *React Testing and Deployment*

#### Describe a case where snapshot testing would be useful, and describe another case where it would be ineffective.
A snapshot test is useful for a fully developed UI page that you want to ensure does not change throughout development. Thus, the usecase of snapshot test can be limited - they are most useful when a completed application is undergoing some refactoring. If you are consistently changing your UI, any saved snapshots will quickly become out of date, and will incorrectly cause your tests to fail.

#### What is the difference between full mount and shallow mount?
Full mounting allows you render the entire component as well as any children components. This allows you to fully test the current component and any components it imports. 

Shallow mounting minimized the render of any imported components, and instead focuses on fully rendering the current component only. 

Both full mounting and shallow mounting allow you to test the values of state and props variables, which is very powerful! This allows you to ensure that the state changes as expected, or that the props passed in are used as expected.

#### What does npm run build do?
To start running test
