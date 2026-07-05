# Two Sum II

## Approach

We use the **two-pointer technique**.

* The array `numbers` is already sorted.
* We create two pointers:

  * `left` starts from the beginning of the array.
  * `right` starts from the end of the array.
* Then we calculate the sum of `numbers[left]` and `numbers[right]`.
* If the sum is equal to `target`, we return the positions.
* Since the problem expects **1-based indexing**, we return:

```python id="9x2d7a"
[left + 1, right + 1]
```

* If the current sum is greater than `target`, we move the `right` pointer left.
* If the current sum is smaller than `target`, we move the `left` pointer right.

This works because the array is sorted.

---

## Complexity Analysis

### Time Complexity

```text id="6dh0ki"
O(n)
```

We only loop through the array once using two pointers.

### Space Complexity

```text id="n91cka"
O(1)
```

We do not use any extra data structure. Only two pointer variables are used.
