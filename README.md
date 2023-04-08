# LightSort
LightSort is a sorting algorithm that uses a divide-and-conquer approach to sort a list of elements. The algorithm works by recursively dividing the input list into smaller sublists until each sublist contains only one element. These single-element sublists are then merged in pairs to create larger sorted sublists. This merging process is repeated until the entire list is sorted.

The merge process is optimized for performance by using a "lighter" implementation of the merge algorithm that uses fewer comparisons and assignments. Instead of using a separate list to store the merged elements, LightSort merges the elements in-place in the original list. This approach reduces the overhead of creating new lists and copying elements, resulting in a more efficient sorting algorithm.

LightSort has a time complexity of O(n log n), which makes it a good choice for sorting large lists of elements. The algorithm is also stable, meaning that it preserves the relative order of equal elements in the input list.

Overall, LightSort is a simple, efficient, and stable sorting algorithm that can be used in a wide range of applications.
