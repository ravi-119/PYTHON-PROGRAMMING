# Python Sets – Complete Concepts

## 1. What is a set?
A set is a collection of unique elements.
It stores values without duplicates and does not keep order.

### Example
```python
s1 = {1, 5, 8}
print(type(s1))
print(s1)
```

---

## 2. Creating a set
### Direct creation
```python
s1 = {1, 5, 8}
```

### Empty set
```python
s4 = set()
print(type(s4))
```

### Create set from a string
```python
s4 = set("rv119")
print(s4)
```

### Important note
```python
s3 = {}
print(type(s3))
```

This creates a dictionary, not a set.

---

## 3. Removing duplicates from a list
A set can be used to remove duplicates from a list.

### Example
```python
l1 = [20, 10, 50, 20, 30, 50, 20, 10]
print(list(set(l1)))
```

This returns only unique values.

---

## 4. Accessing set elements
Sets are unordered, so we cannot access them using index numbers.
We can iterate through them using a loop.

### Example
```python
s4 = {40, 10, 30, 20}
for e in s4:
    print(e)
```

---

## 5. Built-in functions on sets
### `len()`
```python
print(len(s4))
```

### `max()` and `min()`
```python
print(max(s4))
print(min(s4))
```

### `sum()`
```python
print(sum(s4))
```

### `sorted()`
```python
print(sorted(s4))
```

---

## 6. Operators on sets
### Concatenation and repetition
These are not supported for sets.

```python
# set + set -> not supported
# set * int -> not supported
```

### Comparison operators
Sets can be compared using `==`, `!=`, `<`, `>`, `<=`, `>=`.

```python
s1 = {10, 20, 30, 40}
s2 = {10, 20, 40, 50, 60}

print(s1 > s2)
print(s1 < s2)
print(s1 >= s2)
print(s1 <= s2)
print(s1 == s2)
print(s1 != s2)
```

---

## 7. Set methods
### `add()`
Adds an element.

```python
s4.add(80)
```

### `update()`
Adds multiple elements.

```python
s4.update((11, 23))
```

### `remove()`
Removes an element; raises an error if not found.

```python
s4.remove(10)
```

### `discard()`
Removes an element without raising an error if it does not exist.

```python
s4.discard(11)
```

### `pop()`
Removes and returns an arbitrary element.

```python
s4.pop()
```

### `clear()`
Removes all elements.

```python
s4.clear()
```

---

## 8. Set operations
### `intersection()`
Returns common elements.

```python
s1.intersection(s2)
```

### `union()`
Returns all unique elements from both sets.

```python
s1.union(s2)
```

### `issubset()`
Checks whether one set is a subset of another.

```python
s1.issubset(s4)
```

### `issuperset()`
Checks whether one set contains another.

```python
s4.issuperset(s1)
```

---

## 9. Set comprehension
A set can be created using comprehension.

### Example: get vowels from a string
```python
s = input("Enter a string")
s1 = {e for e in s if e in "aeiou"}
print(s1)
```

---

## 10. Important points about sets
- Sets contain unique elements only.
- Order is not preserved.
- Sets cannot be indexed.
- Sets are useful for removing duplicates and performing mathematical set operations.

---

## 11. Summary
Sets are helpful when we need a collection of unique values.
They are commonly used for:
- removing duplicates
- checking membership
- union and intersection operations
- filtering unique characters from strings

In simple words, a set is like a collection of items where duplicates are not allowed.
