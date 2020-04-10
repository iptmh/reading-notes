### *Class 09 — API Server*

#### Describe a use-case where param middleware would come in handy.
This ability to add specific middleware depending on if req.params has a key-value set, is immensely powerful. It can be particularly useful for validating or formatting the req.params key-value before that value is consumed by a GET, POST, PUT, or DELETE route.

#### What are the two ways to add middleware in-between Mongoose and MongoDB interactions?
The populate() method and can also use virtual joins.

#### What is the difference between a join by reference and a virtual join?
They should be the same.

#### What do localField and foreignField mean?
The local field within a product record will map to some foreign field within a category record.
