### *Event Driven Applications*

#### Given the examples of front-end events such as button click, window resize, form submit, etc, what are some examples of back-end events?
Server sent events

#### Why are events sometimes better than asynchronous actions with callbacks?
Because sometimes we don't know how long asynchronous actions with callbacks will take. Also, the benefit of this approach is that now you can have multiple listeners on a single event - having multiple callbacks however is harder to do and can quickly get very confusing.

#### What does an EventEmitter instance do?
When we require the events module, what we get is an exported class called EventEmitter. When we think of the term “emit”, we should think of an event being “raised” or “triggered”. So, this class allows us to both raise new events and to listen to events that have been raised. In order to use this class, we need to create an object from it.

#### When is a program’s call stack, event queue, and event loop active?
When an event is triggered.
