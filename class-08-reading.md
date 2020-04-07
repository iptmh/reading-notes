### *Class 08 Express Routing & Connected API*

#### What is a benefit to using express.Router()?
This allows us to modularize our routes very easily, into discrete files, typically located in a /routes folder.

#### When I say that top-down order matters in Express, what does that mean?
Express executes code from top to bottom. 

#### Why do we use a model class (with create(), read(), etc.) instead of directly calling MongoDB operations (such as save(), find(), etc.) within our Express route handlers?
Because we might not always use MongoDB, might switch to using other database. 
