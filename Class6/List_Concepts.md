# Python Lists – Complete Concepts

## 1. What is a list?
A list is a collection of items stored in a single variable.
It is:
- ordered
- changeable (mutable)
- allows duplicate values
- can store different types of data

### Example
```python
employee = ["Ravi", "Rahul", "Priya"]
```

---

## 2. Creating a list
You can create a list using square brackets `[]`.

### Example
```python
fruits = ["apple", "banana", "mango"]
```

You can also create a list using the `list()` constructor.

### Example
```python
l1 = list([10, 20, 30])
l2 = list("mysirg")
l3 = list(range(5))
```

> Note: `list(10)` and `list(10, 20, 30)` are invalid because `list()` needs an iterable value like a string, range, or another list.

---

## 3. Accessing list elements
List elements are accessed with index numbers.
- Index starts from `0`
- Negative indexing also works
  - `-1` means the last element
  - `-2` means the second last element

### Example
```python
employee = ["Ravi", "Rahul", "Priya"]
print(employee[0])   # Ravi
print(employee[-1])  # Priya
```

### Accessing with loops
- `while` loop can access list items one by one
- `for` loop is also commonly used

```python
for x in employee:
    print(x)
```

---

## 4. Changing list elements
Lists are mutable, so you can replace an item.

### Example
```python
employee[1] = "gyaan"
print(employee)
```

---

## 5. Adding elements to a list
### `append()`
Adds an element at the end of the list.

```python
employee.append("Sachin")
```

### `insert()`
Adds an element at a specific position.

```python
employee.insert(2, "Ram")
```

---

## 6. Deleting elements from a list
### `del`
Deletes an element by its index.

```python
del employee[1]
```

### `remove()`
Removes the first matching element.

```python
employee.remove("Rahul")
```

### `pop()`
Removes and returns the last element by default.

```python
x = employee.pop()
```

### `clear()`
Removes all elements from the list.

```python
employee.clear()
```

---

## 7. Unpacking and packing lists
### Packing
Putting values into a list.

```python
a = 5
b = 6
c = 10
l2 = [a, b, c]
```

### Unpacking
Assigning list items to separate variables.

```python
values = [20, 30, 40, 50]
a, b, c, d = values
```

---

## 8. Built-in functions on lists
### `len()`
Returns the number of elements.

```python
len(l1)
```

### `max()`
Returns the largest element.

### `min()`
Returns the smallest element.

### `sum()`
Returns the sum of numeric values.

### `sorted()`
Returns a sorted copy of the list.

```python
sorted(l1)
```

---

## 9. Comparison operators on lists
Lists can be compared using operators like `==`, `!=`, `<`, `>`.

### Example
```python
l1 = [1, 2, 3]
l2 = [2, 3, 1]
print(l1 == l2)
print(l1 != l2)
```

Comparison is done element by element.

---

## 10. Concatenation and repetition
### Concatenation `+`
Joins two lists.

```python
l1 = [1, 5, 9]
l2 = [2, 3, 1]
l3 = l1 + l2
```

### Repetition `*`
Repeats a list multiple times.

```python
result = l1 * 5
```

---

## 11. List of lists (nested lists)
A list can contain other lists.

### Example
```python
l4 = [[1, 3, 5], [2, 1, 8], [5, 4, 4]]
print(l4[0])
print(l4[0][0])
```

This is called a nested list or a list of lists.

---

## 12. Common list methods
Some important methods are:
- `append()` – add at the end
- `insert()` – add at a chosen position
- `remove()` – remove a value
- `pop()` – remove and return last element
- `reverse()` – reverse the list
- `index()` – find the position of an element
- `count()` – count how many times an element appears
- `sort()` – sort the list in place

### Example
```python
l5 = [1, 10, 28, 90, 75]
l5.append("Ravi")
l5.insert(3, "Aman")
l5.remove(10)
print(l5.index("Aman"))
print(l5.count(90))
```

---

## 13. Sorting lists
### `sorted()`
Returns a new sorted list without changing the original.

```python
print(sorted(l12))
print(sorted(l12, reverse=True))
```

### `.sort()`
Sorts the list in place.

```python
l12.sort()
```

---

## 14. List comprehension
List comprehension is a shorter way to create lists.

### Example 1
```python
l6 = [a + 1 for a in range(5)]
```

### Example 2
```python
l10 = [a**2 for a in range(2, 10, 2)]
```

### Example 3
```python
oddnumbers = [2*e - 1 for e in range(1, int(input("Enter a number")) + 1)]
```

This is used when we want to create a list from a pattern or range.

---

## 15. Important points about lists
- Lists are mutable, so they can be changed.
- They store items in order.
- Items can be accessed by index.
- Duplicate values are allowed.
- Lists can contain strings, numbers, or even other lists.

---

## 16. Summary
Lists are one of the most important data structures in Python.
They are used to store multiple values together and perform operations like:
- storing data
- updating values
- adding/removing items
- sorting and searching
- creating patterns with list comprehension

In simple words, a list helps us manage many values in one place.
