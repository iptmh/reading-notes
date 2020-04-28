### *Access Control (ACL)*

#### Why is access control important? Describe an application that would need access control.
Access control means to restrict certain resources from being seen, changed or deleted by certain individuals. Some websites can limit access to pages based on the type of a signed in user. Ex: A shared googlesheet access.

#### What is a role used for?
Each user role (admin, editor, user, guest, etc) defines what CRUD operations (or capabilities) are accessible to that user. 

#### Why is role based access control more scalable than discretionary or mandatory access control?
Role Based Access Control is a very common method for implementing access control in API servers. By having two data models (one for users and one for roles), developers can quickly edit, change or increase the number of possible roles without largely affecting user data. 
