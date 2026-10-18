1. We have an integer array. We need to sort the array in ascending order and return it without using built-in sorting functions.
2. We use Merge Sort (divide and conquer approach). We recursively divide the array into two halves until we reach single elements. Then, we merge the two sorted halves by comparing elements one by one and placing the smaller one into a temporary array. Finally, we copy the sorted elements back into the original array.
3. Time complexity: O(n log n), where n is the length of the array. The array is split in half log n times, and merging elements at each level takes O(n) time.
4. This approach guarantees O(n log n) time in all cases (worst, average, best). An alternative approach is Quick Sort, which uses less extra space O(log n), but its worst-case time complexity can degrade to O(n^2).

