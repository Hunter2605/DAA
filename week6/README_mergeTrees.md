1. We have the roots of two binary trees root1 and root2. We need to merge them into a single binary tree: if two nodes overlap, sum their values; otherwise, use the existing non-null node.
2. We use recursion. If root1 is null, we return root2; if root2 is null, we return root1. When both nodes exist, we create a new node with the sum of their values (root1.val + root2.val), and recursively merge their left and right children. Finally, we return the merged node.
3. Time complexity: O(n), where n is the minimum number of overlapping nodes between the two trees, as we only visit nodes that exist in at least one tree.
4. Space complexity: O(h), where h is the height of the trees, due to recursion stack. An alternative approach is modifying root1 in-place to avoid allocating new TreeNode objects.

