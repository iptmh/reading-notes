### *Class 04*

#### What makes an interface useful?
An interface is a simplified way to enact more complex operations. Interfaces can be very helpful in standardizing how certain operations are called, and allowing for operations to be largely changed without the code having to be changed too much. 

#### Why is middleware called middleware?
Middleware typically means “software between two other softwares”, like a middleman between two operations that helps the process go more smoothly.

#### Fundamentally, what does it mean to have a mock of something? Why is this useful?
A mock of something is a copy of the exact thing with same data models and commands. We use it for testing and do not need to modify the actual data in our application.

#### What does it mean to have a mock database?
Mock database has the same structure as our application database. It has the same data models and commands. The only difference is that this mock database only exists during the lifetime of the test: it is created and initialized when we start our tests and deleted when tests are complete. We give this mock database some dummy data to initialize with as well, and thus we can be confident that any secure and application related data is not messed with when testing.
