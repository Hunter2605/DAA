1. We have the root of a binary tree. We need to return the inorder traversal of its nodes' values (Left -> Root -> Right).
2. We use recursion with a helper function. If the current node is null, we return. Otherwise, we recursively traverse the left subtree, add the current node's value to the result list, and then recursively traverse the right subtree.
3. Time complexity: O(n), where n is the number of nodes in the tree, because we visit each node exactly once.
4. This approach has O(n) space complexity due to the recursion stack in the worst case (for a skewed tree) and O(log n) for a balanced tree. An alternative approach is iterative using an explicit Stack.

