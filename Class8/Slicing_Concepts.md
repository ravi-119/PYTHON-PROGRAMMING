# Python Slicing – Complete Concepts

## 1. What is slicing?
Slicing is a way to extract a part of a string, list, or tuple.

### Syntax
```python
sequence[start:end:step]
```

- `start` = beginning index
- `end` = stopping index (exclusive)
- `step` = how many positions to move each time

---

## 2. Basic slicing examples
Consider the string:

```python
s2 = "mysirg"
```

### Example 1: Slice from index 0 to 5
```python
print(s2[0:5:1])
```

This prints characters from index `0` to `4`.

### Example 2: Slice full string
```python
print(s2[0:6:1])
```

This prints the entire string because the end index is `6` and the length is `6`.

### Example 3: Slice with step 2
```python
print(s2[0:5:2])
```

This prints every second character.

---

## 3. Understanding the start, end, and step
### Start position
The first index from where slicing begins.

### End position
The index where slicing stops, but it is not included.

### Step value
The interval between elements.
- `1` means take every character
- `2` means take every second character
- `-1` means reverse the string

---

## 4. Slicing with positive step
When step is positive, slicing moves forward.

### Example
```python
print(s2[0:10:1])
```

This takes characters from the beginning up to index `9`, or until the string ends.

---

## 5. Slicing with negative step
When step is negative, slicing moves backward.

### Example
```python
print(s2[5:1:-1])
```

This prints characters in reverse order from index `5` down to index `2`.

### Important idea
A negative step reverses the sequence.

---

## 6. Omitting start or end values
### Omit start
```python
print(s2[:5:1])
```

This means start from the beginning.

### Omit end
```python
print(s2[1::1])
```

This means go to the end of the string.

### Reverse the whole string
```python
print(s2[::-1])
```

This prints the complete string in reverse order.

---

## 7. Extreme cases in slicing
### Positive step and empty start
```python
print(s2[:0:-1])
```

This prints the string in reverse order except the first character.

### Negative step and default end
```python
print(s2[5::-1])
```

This starts from index `5` and goes backward to the beginning.

---

## 8. Reversing a list using slicing
A list can also be sliced.

### Example
```python
l1 = ["mysirg", "education", "services", "private", "limited"]
print(l1[5::-1])
```

This reverses the list.

---

## 9. Reversing words in a sentence
You can reverse the words in a sentence by splitting it first.

### Example
```python
" ".join(input("Enter a string").split(" ")[::-1])
```

### How it works
1. `input()` reads the sentence
2. `.split(" ")` breaks it into words
3. `[:: -1]` reverses the order of words
4. `" ".join(...)` joins them back into one sentence

---

## 10. Important points to remember
- Slicing works on strings, lists, and tuples.
- The end index is exclusive.
- Default step is `1`.
- A negative step reverses the order.
- Slicing does not change the original sequence; it creates a new one.

---

## 11. Summary
Slicing is used to extract a part of a sequence.
It is very helpful for:
- taking a substring
- skipping characters
- reversing text or lists
- working with words and sentences

In simple words, slicing helps you select exactly the part of data you want.
