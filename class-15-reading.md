### *Tree*

#### What is a leaf node? Why is it important to be able to find leaf nodes?
A leaf Node is a Node without any subsequent edges / connections. It is important because for recursion function, the process continues until we hit a leaf node.

#### Describe the differences between pre-order, in-order, and post-order traversal. Why are they called pre, in, and post order?
- Pre-order: root >> left >> right
- In-order: left >> root >> right
- Post-order: left >> right >> root

Pre goes from top (root) to bottom. In goes from left to right. Post goes from bottom (leaf node to top).

#### What is the height of a fully balanced (each non-leaf node has two children) tree? What is this used for?
A “perfect” binary tree is one where every non-leaf node has exactly two children. The maximum width for a perfect binary tree, is 2^(h-1), where h is the height of the tree. Height can be calculated as log n, where n is the number of nodes.

#### How are stacks and queues used in relation to trees?
We utilize stack to implement depth first traversal and queue to implement a breadth first traversal.
