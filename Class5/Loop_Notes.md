# Python Loop Notes

## 1. For Loop

A for loop is used when we want to repeat an action for each item in a collection such as a string, list, or tuple.

### Example from ForLoops.py
- The program stores the string `MySirG` in variable `s1`.
- The loop `for a in s1:` runs once for every character in the string.
- Inside the loop, the code prints:
  - the character itself
  - its Unicode value using `ord(a)`

### What this teaches
- `for` loops are useful for iterating over sequences.
- `ord()` returns the ASCII/Unicode code of a character.

### In simple words
The program checks every character in the word `MySirG` and displays both the character and its numeric code.

---

## 2. While Loop

A while loop continues running as long as a given condition remains true.

### Example 1: Print a Message Five Times
- A variable `i` starts with value `1`.
- The condition `i <= 5` is checked.
- As long as the condition is true, the message `MySirG` is printed.
- The value of `i` increases each time using `i += 1`.

### What this teaches
- A while loop is best when the number of repetitions is not fixed in advance.
- The loop condition must be updated inside the loop, otherwise it may continue forever.

### Example 2: Print First N Natural Numbers
- The user enters a number `n`.
- The loop starts from `1` and continues until it reaches `n`.
- `print(i, end=" ")` prints each number on the same line.

### What this teaches
- `input()` is used to take user input.
- `end=" "` keeps the output in one line separated by spaces.

### Example 3: Sum of First N Natural Numbers
- The program asks the user for a number.
- It adds each number from `1` to `n` into a variable `s`.
- Finally, it prints the total sum.

### What this teaches
- Variables can be used to accumulate values.
- The loop can be used for calculation as well as printing.

---

## 3. Prime Number Check Using While Loop

A prime number is a number greater than `1` that has no divisors other than `1` and itself.

### Example 1: Prime Check Using `break`
- The user enters a number `n`.
- The program checks whether `n` is divisible by any number from `2` to `n-1`.
- If a divisor is found, the loop stops using `break`.
- At the end, it decides whether the number is prime or not.

### Example 2: Prime Check Using `else` with While Loop
- This version uses the `else` block attached to the loop.
- If the loop finishes without finding a divisor, the `else` block runs.
- The program prints `PRIME`.
- If a divisor is found, it prints `NOT PRIME`.

### What this teaches
- `break` is used to stop looping early.
- The `else` block with a loop runs when the loop completes normally without a break.

---

## 4. Important Python Concepts Covered

- `for` loop
- `while` loop
- `break`
- `input()`
- `print()` with `end=" "`
- `+=` shorthand operator
- `ord()` for Unicode values

---

## 5. Short Summary

These programs show the difference between `for` loops and `while` loops:
- `for` loops are ideal for going through known sequences.
- `while` loops are useful when the number of repetitions depends on a condition.

In short, loops help us repeat tasks efficiently and solve problems like printing values, summing numbers, and checking whether a number is prime.
