# Remove Duplicates from Sorted Array

## Approach

We use the **two-pointer technique**.

* The array is already sorted, so duplicate values will be next to each other.
* We keep a pointer `k` to track where the next unique value should be placed.
* Since the first element is always unique, we start `k` from `1`.
* Then we loop from the second element of the array.
* If `nums[i]` is different from `nums[k - 1]`, that means we found a new unique value.
* We place that value at index `k`.
* Then we increase `k` by `1`.

At the end, `k` represents the number of unique elements in the array.

---

## Complexity Analysis

### Time Complexity

```text id="6mnv3p"
O(n)
```

We loop through the array once, where `n` is the number of elements in `nums`.

### Space Complexity

```text id="4qryot"
O(1)
```

We modify the array directly and do not use any extra data structure.
