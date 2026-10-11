1. We have a sorted linked list. We need to delete all duplicates so that each element appears only once, and return the head.
2. We use "curr" starting at the head. In while loop, until "curr" or "curr.next" reaches null, we compare the current value with the next value. If curr.val == curr.next.val, we skip the duplicate by pointing curr.next to curr.next.next. Otherwise, we move "curr" forward to curr.next. Finally, we return the head.
3. Time complexity: O(n), where n is the number of nodes in the list, because we iterate through the list once.
4. This approach is already optimal in both time O(n) and space O(1), because we modify pointers in-place without creating new nodes. An alternative approach is using a HashSet, but it would have worse space complexity.

