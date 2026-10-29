1. We have the root of a binary tree and an integer targetSum. We need to check if there is a root-to-leaf path where the sum of node values equals targetSum.
2. We use recursion. If the node is null, we return false. If the node is a leaf (no left or right child), we check if targetSum equals the node's value. Otherwise, we subtract the current value from targetSum and recursively check if the left or right subtree has a valid path.
3. Time complexity: O(n), where n is the number of nodes, because we visit each node at most once.
4. Space complexity: O(h), where h is the height of the tree, due to the recursion stack. An alternative approach is using an iterative DFS or BFS with two stacks or queues storing nodes and remaining sums.

