# Remove Element

## Approach

We use the **two-pointer technique**.

* `i` is used to check every element in the array.
* `k` is used to track the position where the next valid element should be placed.
* If `nums[i]` is not equal to `val`, we copy it to `nums[k]`.
* Then we increase `k` by `1`.

At the end, `k` represents the number of elements that are not equal to `val`.

---

## Complexity Analysis

### Time Complexity

```text
O(n)
```

We loop through the array only once.

### Space Complexity

```text
O(1)
```

