# Best Time to Buy and Sell Stock

## Approach

We use a **single-pass approach**.

* First, we store the first price as `min_price`.
* This represents the lowest buying price we have seen so far.
* We also create `max_profit` and set it to `0`.
* Then we loop through every price in the array.
* For each price, we calculate the profit by subtracting the lowest price from the current price:

```python id="gvxz91"
profit = price - min_price
```

* If this profit is greater than `max_profit`, we update `max_profit`.
* If the current price is smaller than `min_price`, we update `min_price`.
* At the end, we return `max_profit`.

This works because we always try to buy at the lowest price before selling at the current price.

---

## Complexity Analysis

### Time Complexity

```text id="86kx0b"
O(n)
```

We loop through the price array only once.

### Space Complexity

```text id="c8x0x9"
O(1)
```

We only use two extra variables: `min_price` and `max_profit`.
