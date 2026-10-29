1. We have the root of a binary tree. We need to invert (flip/mirror) the tree and return its root.
2. We use recursion. If the current node is null, we return null. Otherwise, we swap the left and right children, recursively calling invertTree on both subtrees. Finally, we return the root.
3. Time complexity: O(n), where n is the number of nodes, because we visit and swap every node once.
4. Space complexity: O(h), where h is the tree height, due to the call stack. An alternative approach is iterative BFS using a Queue to swap children level by level.

