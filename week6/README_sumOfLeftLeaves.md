1. We have the root of a binary tree. We need to find and return the sum of all left leaves. A left leaf is a node that is the left child of its parent and has no children of its own.
2. We use recursion. If the current node is null, we return 0. If the left child exists and is a leaf (both its left and right are null), we add its value to the sum. If the left child is not a leaf, we recursively search it. Then we also recursively search the right subtree and add the results.
3. Time complexity: O(n), where n is the number of nodes in the tree, because we visit each node once.
4. Space complexity: O(h), where h is the height of the tree, for the call stack. An alternative approach is an iterative traversal (BFS or DFS) with a queue or stack.

