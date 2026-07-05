# Merge Sorted Array

## Approach

We first place all elements from `nums2` into the empty positions at the end of `nums1`.

* `nums1` already has extra space for the elements of `nums2`.
* The loop copies each element from `nums2` into `nums1`, starting from index `m`.
* After all elements are copied, we sort `nums1`.
* This gives us one final sorted array inside `nums1`.

The main idea is to **merge first, then sort**.

---

## Complexity Analysis

### Time Complexity

```text
O((m + n) log(m + n))
```

After copying the elements, we sort the full array. Sorting takes `O((m + n) log(m + n))` time.

### Space Complexity

```text
O(1)
```

We are modifying `nums1` directly and not creating another array.