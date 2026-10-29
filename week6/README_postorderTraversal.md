1. We have the root of a binary tree. We need to return the postorder traversal of its nodes' values (Left -> Right -> Root).
2. We use recursion with a helper function. If the node is null, we return. Otherwise, we recursively traverse the left subtree, then the right subtree, and finally add the current node's value to the result list.
3. Time complexity: O(n), where n is the number of nodes in the tree, because each node is visited once.
4. Space complexity: O(h), where h is the tree height, due to recursion stack. An alternative approach is iterative using one or two Stacks.

