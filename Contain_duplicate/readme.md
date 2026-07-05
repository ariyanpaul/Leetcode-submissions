# Contains Duplicate

## Approach

We use a **set** to keep track of numbers we have already seen.

* First, we create an empty set called `seen`.
* Then, we loop through every number in `nums`.
* If the number is already inside `seen`, that means the number has appeared before.
* In that case, we return `True`.
* Otherwise, we add the number to `seen`.
* If the loop finishes without finding any repeated number, we return `False`.

This approach is efficient because checking whether a value exists in a set is very fast.

---

## Complexity Analysis

### Time Complexity

```text
O(n)
```

We loop through the array once, where `n` is the number of elements in `nums`.

### Space Complexity

```text
O(n)
```

In the worst case, all numbers are unique, so the set may store all elements from the array.
