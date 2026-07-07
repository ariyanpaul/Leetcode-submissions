# Remove Duplicates from Sorted Array II

## Approach

We use the **two-pointer technique**.

* The array is already sorted, so duplicate values appear next to each other.
* This problem allows each number to appear **twice**.
* If the length of `nums` is less than or equal to `2`, we can directly return the value as it satisfies the condition.
* We start `k` from `2` because the first two elements are always allowed.
* Then we loop from index `2` to the end of the array.
* For each element, we compare it with the element at position `k - 2`.
* If `nums[i]` is different from `nums[k - 2]`, that means adding this element will not create more than two duplicates.
* So, we place it at index `k` and increase `k`.

At the end, `k` represents the length of the valid array where each number appears at most twice.

---

## Complexity Analysis

### Time Complexity

```text id="0bnah3"
O(n)
```

We loop through the array once, where `n` is the number of elements in `nums`.

### Space Complexity

```text id="nwrt1k"
O(1)

```

We modify the array directly and do not use any extra data structure.

