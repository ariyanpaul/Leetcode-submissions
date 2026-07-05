# Two Sum

## Approach

We use a **brute force approach** with two loops.

* The first loop picks one number from the array.
* The second loop checks every number after it.
* For every pair, we check whether the second number is equal to:

```python
target - nums[i]
```

This means we are checking whether the two numbers together can make the target.

When we find the correct pair, we return their indices.

---

## Complexity Analysis

### Time Complexity

```text
O(n²)
```

We use two nested loops, so for every element, we may check many other elements.

### Space Complexity

```text
O(1)
```

We are not using any extra data structure. We only use loop variables.