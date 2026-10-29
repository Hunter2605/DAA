1. We have the root of a binary tree. We need to find its maximum depth (the number of nodes along the longest path from the root down to the farthest leaf).
2. We use recursion (DFS). If the root is null, the depth is 0. Otherwise, we find the maximum depth of the left subtree and the right subtree, take the larger one, and add 1 for the current node.
3. Time complexity: O(n), where n is the number of nodes in the tree, because we visit every node once.
4. Space complexity: O(h), where h is the tree height (O(n) in worst case, O(log n) in balanced tree) due to the call stack. An alternative approach is iterative BFS (level-order traversal) using a Queue.

