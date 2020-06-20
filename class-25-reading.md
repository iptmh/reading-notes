### *DSA: HashTables*

#### Is a HashTable useful for search or sorting operations? Why?
It is useful for searching because the idea of a hashtable is the ability to store a key-value pair into a data structure, and quickly retrieve the value as long as you know the key. 

#### What makes a good hash function?
A collision occurs when more than one key hashes to the same index in an array. A “perfect hash function” will never have any collisions.

#### Why should you try to reduce the number of collisions?
Typically a collission is handled by setting the value at the collided index to a list instead of an individual value. This can be either an array or LinkedList, though traditionally it has been a LinkedList. Now, if two keys resolve to the same index in the array then their key/value pairs can be added to the end of a list.

#### What is stored at each index of a HashTable? Why?
The entire key/value pair. Since different keys can lead to the same index, it’s important to store the entire key/value pair in the bucket, not just the value. If only values were stored in buckets then it would be impossible to determine which value to return when a key led you to an index.
