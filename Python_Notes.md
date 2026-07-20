# Python Notes (Human-Readable)

## 1. What is Python?

Python is a high-level, easy-to-learn, and powerful programming language.
It was created by Guido van Rossum and first released in 1991.
Python is used to build websites, automation scripts, data science tools, machine learning models, AI applications, and many other software systems.

Why Python is popular:
- It is simple and readable.
- It has a clean syntax.
- It is beginner-friendly.
- It supports many libraries and frameworks.
- It is used in many industries.

In simple words:
- Python lets you write code that is close to human language.
- It reduces the complexity of programming.

---

## 2. Features of Python

Python has many useful features:

1. Easy to Learn
   - Python syntax is simple and clear.
   - Beginners can understand it quickly.

2. Interpreted Language
   - Python executes code line by line.
   - Errors are shown immediately.

3. High-Level Language
   - You do not need to manage low-level memory details directly.

4. Cross-Platform
   - Python runs on Windows, Linux, and macOS.

5. Portable
   - Same Python code can work on different platforms.

6. Object-Oriented
   - Python supports OOP concepts like classes and objects.

7. Large Standard Library
   - Python provides built-in modules for math, file handling, networking, and more.

8. Open Source
   - Python is free to use and has a big community support.

9. Dynamically Typed
   - You do not need to declare variable types explicitly.

10. Extensible and Embedded
   - Python can be integrated with other languages like C and C++.

---

## 3. How Python Works

Python works in a step-by-step process:

1. Writing Source Code
   - You write Python code in a file, such as `example.py`.

2. Compilation to Bytecode
   - Python first translates the code into bytecode.
   - Bytecode is a lower-level form that the Python interpreter can understand.

3. Execution by Python Virtual Machine (PVM)
   - The Python Virtual Machine executes the bytecode.
   - This is why Python is called an interpreted language.

### Simple Flow

Source Code -> Python Compiler/Translator -> Bytecode -> Python Virtual Machine -> Output

This means Python does not directly convert the entire code into machine code like C or C++.
Instead, Python translates it into bytecode and then runs it.

---

## 4. Interpreter and Compiler

### Compiler
A compiler is a program that translates the whole source code into machine code before execution.

Example languages:
- C
- C++
- Java (before runtime)

### Interpreter
An interpreter reads and executes the source code line by line.

Example languages:
- Python
- JavaScript
- Ruby

### Difference Between Interpreter and Compiler

| Topic | Compiler | Interpreter |
|---|---|---|
| Execution | Converts whole program first | Executes line by line |
| Speed | Usually faster | Usually slower |
| Error detection | Shows all errors after compilation | Shows errors during execution |
| Example | C, C++ | Python, JavaScript |

### Important Note
Python uses both concepts in a combined way:
- It compiles source code into bytecode.
- Then the interpreter executes that bytecode.

So Python is often called an interpreted language, but internally it uses compilation to bytecode.

---

## 5. Tokens in Python

A token is the smallest unit of a Python program.
When Python reads your code, it breaks it into tokens.

Example:
```python
x = 10
```

Tokens here are:
- `x` -> identifier
- `=` -> operator
- `10` -> literal

Python tokens are classified into different categories:
- Keywords
- Identifiers
- Literals
- Operators
- Punctuators / Delimiters

---

## 6. Identifiers

Identifiers are names given to variables, functions, classes, modules, or objects.

### Rules for identifiers
- They can contain letters, digits, and underscore `_`.
- They cannot start with a digit.
- They cannot use spaces.
- They cannot be Python keywords.
- They are case-sensitive.

### Examples
```python
name = "Ravi"
age = 20
student_name = "Amit"
```

Valid identifiers:
- `name`
- `age`
- `student_name`

Invalid identifiers:
- `2name`
- `student name`
- `class`

---

## 7. Literals

Literals are fixed values used directly in code.
They represent data.

### Types of literals

1. Numeric Literals
   - Integer: `10`, `-5`
   - Float: `3.14`, `2.0`
   - Complex: `2 + 3j`

2. String Literals
   - Single quote: `'hello'`
   - Double quote: "hello"
   - Triple quotes: `'''hello'''`

3. Boolean Literals
   - `True`
   - `False`

4. None Literal
   - `None` means no value.

5. Collection Literals
   - List: `[1, 2, 3]`
   - Tuple: `(1, 2, 3)`
   - Dictionary: `{"name": "Ravi"}`
   - Set: `{1, 2, 3}`

### Example
```python
x = 10        # integer literal
pi = 3.14     # float literal
name = "Python"  # string literal
flag = True   # boolean literal
```

---

## 8. Operators

Operators are symbols that perform operations on values or variables.

### Types of operators

1. Arithmetic Operators
   - `+` addition
   - `-` subtraction
   - `*` multiplication
   - `/` division
   - `%` modulus
   - `**` exponentiation
   - `//` floor division

Example:
```python
a = 10
b = 3
print(a + b)
print(a % b)
```

2. Comparison Operators
   - `==` equal to
   - `!=` not equal to
   - `>` greater than
   - `<` less than
   - `>=` greater than or equal to
   - `<=` less than or equal to

3. Assignment Operators
   - `=`
   - `+=`
   - `-=`
   - `*=`
   - `/=`

4. Logical Operators
   - `and`
   - `or`
   - `not`

5. Bitwise Operators
   - `&`, `|`, `^`, `~`, `<<`, `>>`

6. Identity Operators
   - `is`
   - `is not`

7. Membership Operators
   - `in`
   - `not in`

### Example
```python
x = 5
y = 10
print(x < y)
print(x and y)
```

---

## 9. Keywords in Python

Keywords are reserved words that have special meanings in Python.
You cannot use them as identifiers.

### Examples of keywords
```python
False, None, True, and, as, assert, async, await, break, class, continue, def, del, elif, else, except, finally, for, from, global, if, import, in, is, lambda, nonlocal, not, or, pass, raise, return, try, while, with, yield
```

### Important Note
Keywords are predefined by Python, so they cannot be used as variable names.

Example:
```python
class = 10
```
This will give an error because `class` is a keyword.

---

## 10. Punctuators (Delimiters)

Punctuators are special symbols used to separate or group code elements.
They are also called delimiters.

### Common punctuators

- `(` and `)` : parentheses
- `[` and `]` : brackets
- `{` and `}` : braces
- `,` : comma
- `:` : colon
- `;` : semicolon
- `.` : dot
- `'` and `"` : single and double quotes
- `#` : comment symbol

### Example
```python
name = "Ravi"   # string literal
print(name)     # function call
```

### Uses
- Parentheses group expressions and arguments.
- Brackets define lists.
- Braces define dictionaries and sets.
- Comma separates values.
- Colon marks blocks in `if`, `for`, `while`, and function definitions.

---

## 11. What is OOP?

OOP stands for Object-Oriented Programming.
It is a programming style where the program is organized around objects and classes.

### Why OOP is used
- It makes code reusable.
- It makes programs easier to maintain.
- It improves security and structure.
- It helps model real-world things.

---

## 12. Class and Object

### Class
A class is a blueprint or template for creating objects.
It defines what an object will contain and what actions it can perform.

### Object
An object is an instance of a class.
It is a real entity created from the class.

### Example
```python
class Car:
    def __init__(self, brand):
        self.brand = brand

    def show_brand(self):
        print("Car brand:", self.brand)

c1 = Car("Toyota")
c1.show_brand()
```

In this example:
- `Car` is a class.
- `c1` is an object.
- `brand` is an attribute.
- `show_brand()` is a method.

---

## 13. Four Pillars of OOP

The four main pillars of Object-Oriented Programming are:

1. Encapsulation
2. Inheritance
3. Polymorphism
4. Abstraction

### 1. Encapsulation
Encapsulation means binding data and methods together inside a class.
It also hides sensitive information from outside access.

Example:
```python
class BankAccount:
    def __init__(self, balance):
        self.__balance = balance

    def deposit(self, amount):
        self.__balance += amount

    def get_balance(self):
        return self.__balance
```

Here, `__balance` is protected/private inside the class.

### 2. Inheritance
Inheritance allows one class to use the properties and methods of another class.
It helps in code reuse.

Example:
```python
class Animal:
    def sound(self):
        print("Animal makes a sound")

class Dog(Animal):
    def sound(self):
        print("Dog barks")
```

Here, `Dog` inherits from `Animal`.

### 3. Polymorphism
Polymorphism means one thing can have many forms.
In Python, the same method name can behave differently in different classes.

Example:
```python
class Cat:
    def sound(self):
        print("Meow")

class Dog:
    def sound(self):
        print("Bark")
```

Both classes have a `sound()` method, but the behavior is different.

### 4. Abstraction
Abstraction means showing only the important details and hiding the internal complexity.

Example:
```python
from abc import ABC, abstractmethod

class Shape(ABC):
    @abstractmethod
    def area(self):
        pass
```

A user uses the method `area()` without knowing the internal implementation.

---

## 14. Summary

Python is a simple, powerful, and beginner-friendly programming language.
It works by converting code into bytecode and executing it through the Python Virtual Machine.
It uses tokens such as keywords, identifiers, literals, operators, and punctuators.
Python also supports OOP concepts such as classes, objects, and the four pillars:
- Encapsulation
- Inheritance
- Polymorphism
- Abstraction

These features make Python one of the most popular languages in the world.
