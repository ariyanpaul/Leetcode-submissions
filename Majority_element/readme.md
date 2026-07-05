    # Majority Element

## Approach

We use the **sorting approach**.

* First, we sort the array.
* The majority element appears more than `n / 2` times.
* Because it appears more than half of the array, it must be present at the middle index after sorting.
* So, we return the element at index:

```python id="7xvrc6"
n // 2
```

This works because the majority element takes up enough space in the sorted array to always cover the middle position.

---

## Complexity Analysis

### Time Complexity

```text id="f3a61k"
O(n log n)
```

We sort the array, and sorting takes `O(n log n)` time.

### Space Complexity

```text id="wq9p72"
O(1)
```

We are not using any extra data structure. The array is sorted directly.
