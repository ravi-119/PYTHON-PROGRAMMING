# Python Decision Making Notes

## 1. What is decision making in Python?
Decision making means choosing what action to perform based on a condition.
In Python, this is done using conditional statements.

The main decision-making statements are:
- `if`
- `if ... else`
- `if ... elif ... else`

---

## 2. Importance of indentation
Python uses indentation to define the block of code inside a condition.
If the code is not indented properly, it will not belong to the `if` block.

### Example
```python
x = -2
if x > 0:
    print("Hello duniya")
    print("Ravi")
print("puma")
```

### Explanation
- The lines inside `if x > 0:` run only if `x > 0`.
- `print("puma")` is outside the `if` block, so it always runs.

---

## 3. Simple `if` statement
The `if` statement runs a block of code only when the condition is true.

### Example
```python
x = int(input("Enter a number"))
if x > 0:
    print("number is positive")
```

### Explanation
- If the number is greater than `0`, the message prints.
- If not, nothing happens.

### Example 2
```python
x = int(input("Enter a number"))
if x < 0:
    print("number is non-zero/non positive")
```

---

## 4. `if ... else` statement
The `else` part runs when the `if` condition is false.

### Example
```python
x = int(input("Enter a number"))
if x > 0:
    print("number is positive")
else:
    print("number is non-positive/non-zero value")
```

### Explanation
- If the number is positive, the first message is printed.
- Otherwise, the second message is printed.

---

## 5. `if ... elif ... else` statement
This is used when there are multiple conditions to check.

### Example: Grade system
```python
x = int(input("Enter marks"))
if x > 90:
    print("Grade A")
elif x > 80:
    print("Grade B")
elif x > 70:
    print("Grade C")
elif x > 60:
    print("Grade D")
elif x > 50:
    print("Grade E")
else:
    print("Grade F")
```

### Explanation
- Python checks the conditions from top to bottom.
- As soon as one condition becomes true, the corresponding block runs.
- The `else` block runs if none of the previous conditions are true.

---

## 6. Single-line `if ... else` (Ternary Operator)
Python also allows a short form of `if-else` in one line.

### Example
```python
print("Even" if int(input("Enter a number")) % 2 == 0 else "odd")
```

### Explanation
- If the number is divisible by `2`, it prints `Even`.
- Otherwise, it prints `odd`.

This is called a conditional expression.

---

## 7. Taking input for decision-making
`input()` always returns a string in Python.
So, if we want to compare numbers, we must convert the input into an integer.

### Example
```python
x = int(input("Enter a number"))
```

### Why conversion is needed
Because this comparison works properly:
```python
if x > 0:
```

If we do not convert, Python will compare strings and the program may not behave as expected.

---

## 8. Type conversion (important supporting concept)
Type conversion is used when we want to change one data type into another.
This is very useful before making decisions with user input.

### Examples
```python
a = str(5) + "5"
b = 5 + int("5")
print(a)
print(b)
```

### Some common conversions
```python
a = 5
b = 4.5
print(int(b))
print(float(a))
```

```python
x = "234"
print(int(x))
```

```python
x = 2.4
print(complex(x))
print(bool(x))
```

### Explanation
- `int()` converts to integer
- `float()` converts to decimal
- `complex()` converts to complex number
- `bool()` converts to boolean value

---

## 9. Basic arithmetic example with input
```python
# Program to add two numbers
print("Enter two numbers")
a, b = int(input()), int(input())
c = a + b
print("Sum is", c)
```

### Explanation
- The program takes two numbers from the user.
- Converts them into integers.
- Adds them and prints the sum.

This is useful because many decision-based programs begin by collecting input values.

---

## 10. Summary of decision making in Python
Decision-making statements help the program choose one path or another.

### Main forms
- `if` → run code only if condition is true
- `if else` → choose between two blocks
- `if elif else` → choose among multiple blocks
- Single-line `if else` → short form for simple conditions

### Important points
- Conditions are written using comparison operators such as `>`, `<`, `==`, `!=`.
- Indentation is very important in Python.
- Input values should be converted to the correct type before comparison.

---

## 11. In simple words
Decision making in Python means:
- checking a condition
- deciding what to do next
- running one block of code instead of another

This is the basis of logic-building in programming.
