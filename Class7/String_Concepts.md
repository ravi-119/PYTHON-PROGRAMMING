# Python Strings – Complete Concepts

## 1. What is a string?
A string is a sequence of characters enclosed in single quotes `' '`, double quotes `" "`, or triple quotes.

### Example
```python
s1 = "mysirg"
print(type(s1))
```

This shows that `s1` is of type `str`.

---

## 2. Empty string
An empty string has no characters in it.

### Example
```python
s2 = ""
print(s2)
```

You can also convert other values into strings using `str()`.

### Example
```python
s2 = str([11, 22])
print(s2)
```

---

## 3. String indexing
Each character in a string has an index number.
- Index starts from `0`
- Negative index also works from the end

### Example
```python
s1 = "mysirg"
print(s1[0], s1[1], s1[2])
print(s1[-1], s1[-2], s1[-3])
```

### Important idea
You can access characters one by one using indexing.
You can also iterate through them using a loop.

```python
for e in s1:
    print(e)
```

---

## 4. Built-in functions for strings
Some built-in functions work on strings as well.

### `len()`
Returns the length of the string.

```python
print(len(s1))
```

### `min()` and `max()`
Returns the minimum and maximum character based on alphabetical order.

```python
print(min(s1))
print(max(s1))
```

### `sorted()`
Returns a sorted list of characters.

```python
print(sorted(s1))
```

---

## 5. Concatenation and repetition operators
### Concatenation `+`
Joins two strings together.

```python
s1 = "ABC"
s2 = "DE"
print(s1 + s2)
```

### Repetition `*`
Repeats a string multiple times.

```python
print(s2 * 3)
```

---

## 6. Comparison operators on strings
Strings can be compared lexicographically (alphabetically).

### Example
```python
s1 = "mysirg"
s2 = "saurabh"
print(s1 > s2)
```

This compares strings using dictionary-style order.

---

## 7. String object methods
Python provides many built-in methods for strings.

### `index()`
Finds the position of a substring.

```python
s1 = "mysirg education services"
print(s1.index("i"))
print(s1.index("sir"))
```

### `count()`
Counts how many times a character or substring appears.

```python
print(s1.count("i"))
print(s1.count(" "))
```

### `startswith()` and `endswith()`
Checks whether a string starts or ends with a given value.

```python
print(s1.startswith("my"))
print(s1.endswith("services"))
```

### `isdigit()`
Checks whether the string contains only digits.

```python
s2 = "a123"
print(s2.isdigit())

s2 = "123"
print(s2.isdigit())
```

### `islower()` and `isupper()`
Checks the case of the letters.

```python
print(s1.islower())
print(s1.isupper())
```

### `upper()` and `lower()`
Converts the string to uppercase or lowercase.

```python
print(s1.upper())
print(s1.lower())
```

### `replace()`
Replaces one substring with another.

```python
print(s1.replace("m", "M"))
print(s1.replace("i", "I", s1.count("i")))
```

---

## 8. Format function
The `format()` method is used to insert values inside a string.

### Example
```python
a, b = 10, 20
s3 = "Sum of {} and {} is {}"
print(s3.format(a, b, a + b))
```

You can also specify the order of placeholders.

```python
s3 = "Sum of {2} and {1} is {0}"
print(s3.format(a, b, a + b))
```

---

## 9. Split and join
### `split()`
Splits a string into a list of substrings.

```python
s1 = "mysirg education services private limited"
print(s1.split(" "))
```

### Taking input as comma-separated values
```python
s2 = input("Enter numbers separated by comma")
print(s2)
```

Then split the input string:

```python
l1 = s2.split(",")
print(l1)
```

Convert each item to integer:

```python
l2 = [int(x) for x in l1]
print(l2)
```

### Short way to take input and convert to list of integers
```python
l2 = [int(x) for x in input("Enter numbers separated by comma").split(",")]
print(l2)
```

### `join()`
Joins a list of strings into one string.

```python
l1 = ["mysirg", "education", "services", "provide", "limited"]
strobject = "-"
print(strobject.join(l1))
```

---

## 10. Important ideas to remember
- Strings are used to store text.
- Each character has an index.
- Strings are immutable, which means they cannot be changed directly once created.
- Python provides many helpful methods for searching, counting, converting, and formatting strings.
- `split()` converts a string into a list, while `join()` converts a list of strings back into a string.

---

## 11. Summary
Strings are one of the most important data types in Python. They help us handle text, words, sentences, and input from users. With string methods, we can:
- access characters
- count letters or words
- change case
- replace text
- split input into smaller parts
- join values to form a sentence or text

In simple words, strings are used whenever we work with text in Python.
