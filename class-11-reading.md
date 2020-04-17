### *DSA: Stacks and Queues*

#### Come up with an application scenario where you would want to use a stack.
The back/forward button on a web browser: When a user visits a new web page, the current page gets pushed onto the stack. When the user clicks the back button, the last page pushed onto the stack is popped off of the stack and loaded in the browser window. When all of the pages are popped off of the stack, the back button grays out, indicating that the stack is empty.

Also the Undo/Redo stacks in Excel or Word.

#### Come up with an application scenario where you would want to use a queue.
Serving requests on a single shared resource, like a printer.
Call Center phone systems uses queues to hold people calling them in an order, until a service representative is free.
A bank processing transactions against an account. Usually you'll see a list of "pending" transactions at the end of the day. 

#### Why are pop, push, enqueue and dequeue always O(1)?
This is because it takes the same amount of time to perfrom the operation no matter how many Nodes (n) or items you have in the stack/queue.

#### Why do stacks and queues not have traversal or searching operations?
It is mostly meant for temporary storage instead of long-term storage or traversal.
