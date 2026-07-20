# Python Dictionaries – Complete Concepts

## 1. What is a dictionary?
A dictionary stores data in key-value pairs.
Each key is unique, and each key is associated with a value.

### Example
```python
d1 = {102: "rahul", 105: "payal", 106: "Arjun", 107: "Prachi"}
print(type(d1))
```

---

## 2. Creating a dictionary
### Direct creation
```python
d1 = {102: "rahul", 105: "payal"}
```

### Empty dictionary
```python
d2 = {}
print(type(d2))
```

### Creating using `dict()`
```python
d3 = dict(r="rahul", p="payal")
print(d3)
```

---

## 3. Accessing dictionary elements
You can access values using their keys.

### Example
```python
print(d1[102])
print(d1[106])
```

### Using a loop
```python
for k in d1:
    print(k)
```

This prints only the keys.

---

## 4. Adding and editing dictionary values
### Add a new key-value pair
```python
d1[110] = "rama"
print(d1)
```

### Edit an existing value
```python
d1[102] = "ravi"
print(d1)
```

---

## 5. Methods of dictionaries
### `keys()`
Returns all keys.

```python
print(d1.keys())
```

### `values()`
Returns all values.

```python
print(d1.values())
```

### `items()`
Returns all key-value pairs as tuples.

```python
print(d1.items())
```

### Iterating through items
```python
for t in d1.items():
    k = t[0]
    d = t[1]
    print(k, d)
```

You can also unpack directly:

```python
for k, d in d1.items():
    print(k, d)
```

---

## 6. Built-in functions on dictionaries
### `len()`
```python
print(len(d1))
```

### `min()`, `max()`
```python
print(min(d1))
print(max(d1))
```

### `sum()`
```python
print(sum(d1))
```

### `sorted()`
```python
print(sorted(d1))
```

---

## 7. Operators on dictionaries
### Concatenation and repetition
These are not supported.

```python
# dict + dict -> not supported
# dict * int -> not supported
```

### Comparison operators
Dictionaries can be compared using `==` and `!=`.

```python
d3 = {"r": "rahul", "p": "payal"}
d4 = {"p": "payal", "r": "rahul"}
print(d3 == d4)
```

---

## 8. Dictionary object methods
### `pop()`
Removes and returns the value for a specified key.

```python
print(d1.pop(106))
print(d1)
```

### `popitem()`
Removes and returns the last inserted key-value pair.

```python
print(d1.popitem())
print(d1)
```

### `clear()`
Removes all items from the dictionary.

```python
print(d1.clear())
print(d1)
```

---

## 9. Dictionary comprehension
A dictionary can be created using comprehension.

### Example
```python
d3 = {a: a**2 for a in range(1, 8, 1)}
print(d3)
```

This creates a dictionary where each number is mapped to its square.

---

## 10. Important points about dictionaries
- Keys must be unique.
- Values can be duplicated.
- Dictionaries are mutable.
- They are very useful for storing related data.
- Keys are used to access values quickly.

---

## 11. Summary
Dictionaries are used to store data in key-value form.
They are very helpful when we want to map one thing to another, for example:
- roll number to student name
- product id to product price
- city name to population

In simple words, a dictionary is like a real-world lookup table.
