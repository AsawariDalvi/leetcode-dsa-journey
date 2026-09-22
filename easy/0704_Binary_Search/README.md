# 704. Binary Search

## Problem

Given a sorted array and a target value, find the index
of the target. If the target doesn't exist, return -1.

## Approach

We use Binary Search.

Because the array is sorted, we can check the middle
element and eliminate half of the search space each time.

### Steps

1. Set `left` to the first index.
2. Set `right` to the last index.
3. Find the middle index.
4. If `nums[mid] == target`, return `mid`.
5. If `nums[mid] < target`, search the right half.
6. Otherwise, search the left half.
7. Continue until the target is found or the search space is empty.

## Complexity

- Time: `O(log n)`
- Space: `O(1)`

## Language

c++