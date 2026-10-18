1. We have the head of a linked list. We need to sort the list in ascending order and return its head in O(n log n) time complexity.
2. We use Merge Sort for linked lists. First, we find the middle of the list using "slow" and "fast" pointers and split the list into two halves. Then, we recursively sort each half. Finally, we merge the two sorted halves by comparing elements and rewiring existing pointers using a dummy node.
3. Time complexity: O(n log n), where n is the number of nodes. The list is divided in half log n times, and merging nodes at each level takes O(n) time.
4. This approach achieves the required O(n log n) time complexity with O(log n) space due to the recursive call stack. An alternative approach is an iterative bottom-up merge sort, which achieves O(1) space, but is much more complex to implement.

