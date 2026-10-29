1. We have the root of a binary tree. We need to return the preorder traversal of its nodes' values (Root -> Left -> Right).
2. We use recursion with a helper function. If the node is null, we return. Otherwise, we add the current node's value to the result list first, then recursively visit the left child, and finally the right child.
3. Time complexity: O(n), where n is the number of nodes in the tree, as every node is visited once.
4. Space complexity: O(h), where h is the tree height, for the call stack. An alternative approach is an iterative solution using a Stack.

