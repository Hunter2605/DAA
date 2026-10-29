1. We have the root of a binary tree. We need to find its minimum depth (the number of nodes along the shortest path from the root down to the nearest leaf node).
2. We use recursion. If root is null, depth is 0. If one child is missing (null), we must go through the other child to reach a leaf. If both children exist, we take the minimum of left and right depths, and add 1.
3. Time complexity: O(n), where n is the number of nodes in the tree, because in the worst case we visit all nodes.
4. Space complexity: O(h), where h is the tree height, due to the recursion stack. An alternative approach is BFS using a Queue, which is often faster in practice because it stops as soon as the first leaf is found.

