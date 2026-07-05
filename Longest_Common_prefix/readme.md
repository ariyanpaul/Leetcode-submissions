# Longest Common Prefix

## Approach

We use a **character-by-character comparison** approach.

* First, we create an empty string called `res`.
* We use the first string in the list as the reference.
* Then, we check each character of the first string one by one.
* For every character position, we compare that character with the same position in all other strings.
* If any string ends at that position, or the character does not match, we return `res`.
* If all strings have the same character at that position, we add that character to `res`.

This way, `res` keeps storing only the characters that are common at the beginning of every string.

---

## Complexity Analysis

### Time Complexity

```text id="p7txqm"
O(n * m)
```

Here, `n` is the number of strings, and `m` is the length of the first string.

In the worst case, we compare every character of the first string with every other string.

### Space Complexity

```text id="f4zq31"
O(1)
```

We are only using a result string and loop variables. No extra data structure is used.
