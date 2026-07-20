# Python Tuples – Complete Concepts

## 1. What is a tuple?
A tuple is an ordered collection of items, similar to a list, but it is immutable, meaning it cannot be changed after creation.

### Example
```python
t1 = (1, 5, 7)
print(type(t1))
```

---

## 2. Creating tuples
### Empty tuple
```python
t2 = ()
print(type(t2))
```

### Single element tuple
A single value inside parentheses is not automatically a tuple.

```python
t3 = (10)
print(type(t3))
```

This is an integer, not a tuple.

To make a tuple with one element, use a comma:

```python
t4 = (10,)
print(type(t4))
```

### Tuple without parentheses
You can also create a tuple by separating values with commas:

```python
t5 = 11, 6, 3, 10
print(type(t5))
```

---

## 3. Indexing in tuples
Like strings and lists, tuple elements are accessed using index numbers.

### Example
```python
print(t1[0])
print(t1[-1], t1[-2], t1[-3])
```

- `t1[0]` gives the first item
- `t1[-1]` gives the last item

---

## 4. Accessing tuple elements
You can access tuple elements in three common ways:

### 1. Using index numbers
```python
t1 = (10, 5, 20, 15)
print(t1[0])
```

### 2. Using a while loop
```python
i = 0
while i < len(t1):
    print(t1[i])
    i = i + 1
```

### 3. Using a for loop
```python
for a in t1:
    print(a)
```

---

## 5. Built-in functions for tuples
### `len()`
Returns the number of elements.

```python
print(len(t1))
```

### `min()` and `max()`
Returns the smallest and largest values.

```python
print(min(t1))
print(max(t1))
```

### `sum()`
Returns the sum of all numeric values.

```python
print(sum(t1))
```

### `sorted()`
Returns a sorted list of the elements.

```python
print(sorted(t1))
```

---

## 6. Concatenation and repetition operators
### Concatenation `+`
Combines two tuples.

```python
t1 = (10, 5, 20, 15)
t2 = (10, 30, 40, 50, 60)
print(t1 + t2)
```

### Repetition `*`
Repeats a tuple multiple times.

```python
print(t1 * 3)
```

---

## 7. Comparison operators on tuples
Tuples can be compared using relational operators.

### Example
```python
print(t1 < t2)
```

This compares tuple elements in order.

---

## 8. Tuple methods
### `index()`
Returns the index of a value.

```python
print(t1.index(5))
print(t1.index(15))
```

### `count()`
Counts how many times a value appears.

```python
print(t1.count(5))
```

---

## 9. Slicing a tuple
Like strings, tuples support slicing.

### Example
```python
t1 = (10, 4, 3, 2, 9, 1, 3, 4, 5)
print(t1[2:8:2])
```

This starts at index `2`, ends before `8`, and takes every second element.

### Reversing a tuple
```python
print(t1[::-1])
```

This prints the tuple in reverse order.

---

## 10. Important points about tuples
- Tuples are ordered.
- Tuples are immutable.
- They can store duplicate values.
- They are faster than lists in some cases.
- They are commonly used for fixed data.

---

## 11. Summary
A tuple is a simple and safe way to store multiple values in Python.
It is useful when you want data that should not be changed.

In simple words:
- list = changeable
- tuple = not changeable

Tuples are mostly used for storing fixed values, grouped data, and return values from functions.
