1. We have the root of a binary tree. We need to return all root-to-leaf paths in any order formatted as strings (e.g. "1->2->5").
2. We use DFS recursion. We maintain the current path string. At each node, we append its value. If the node is a leaf (both left and right are null), we add the completed path to our result list. If not, we add "->" and recursively continue down to the left and right children.
3. Time complexity: O(n), where n is the number of nodes, because we visit each node to construct the paths.
4. Space complexity: O(h), where h is the height of the tree, for the recursion stack (ignoring string storage for results). An alternative approach is BFS using two queues (one for nodes, one for path strings).

