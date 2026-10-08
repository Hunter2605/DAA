1. We have a linked list. We need to determine if the list is cycled.
2. We use "slow" and "fast", both starting at the head. In while loop, until "fast" or "fast.next" reaches null, "slow" moves 1 step and "fast" moves 2 steps. If there is a cycle, the fast will meet the slow (slow == fast), and we return true. If "fast" reaches null, there is no cycle and we return false.
3. Time complexity: O(n). If there is no cycle, fast reaches the end in n/2 steps. If there is a cycle, fast catches up to slow within the length of the cycle.
4. This approach is already optimal in both time O(n) and space O(1). An alternative approach is using a HashSet to store visited nodes, but we will get worse space complexity.
