# 🐍 Python Basics — Questions & Answers

![Python](https://img.shields.io/badge/Python-Basics-blue?logo=python&logoColor=white) ![Level](https://img.shields.io/badge/Level-Beginner-brightgreen) ![Format](https://img.shields.io/badge/Format-Q%26A-purple)

A beginner-friendly collection of **140 Python questions and answers** in simple English. Each answer includes **one example**.

## 📚 Table of Contents
1. [Data Types](#1-data-types)
2. [Dictionaries](#2-dictionaries)
3. [Exception Handling](#3-exception-handling)
4. [File Handling](#4-file-handling)
5. [Function Arguments](#5-function-arguments)
6. [Functions](#6-functions)
7. [Code Editors and IDEs](#7-code-editors-and-ides)
8. [Lambda Functions](#8-lambda-functions)
9. [Lists](#9-lists)
10. [Loops](#10-loops)
11. [Voting System Project](#11-voting-system-project)
12. [Modules](#12-modules)
13. [Object-Oriented Programming](#13-object-oriented-programming)
14. [Operators](#14-operators)
15. [Packages and pip](#15-packages-and-pip)
16. [datetime Module](#16-datetime-module)
17. [Python Syntax](#17-python-syntax)
18. [Sets](#18-sets)
19. [String Methods](#19-string-methods)
20. [Strings](#20-strings)
21. [Tuples](#21-tuples)
22. [Type Casting](#22-type-casting)
23. [Variables](#23-variables)
24. [Installing Python](#24-installing-python)
25. [break, continue, and pass](#25-break-continue-and-pass)
26. [Built-in Functions](#26-built-in-functions)
27. [Comments](#27-comments)
28. [Conditional Statements](#28-conditional-statements)

---

## 1. Data Types

**1. What are data types in Python?**  
Data types tell Python what kind of value is stored. Example: `age = 20` is an integer (`int`).

**2. What is the difference between `int` and `float`?**  
`int` stores whole numbers; `float` stores decimal numbers. Example: `count = 5; price = 5.5`.

**3. Why do we use the string data type in Python?**  
Strings store text. Example: `city = "Delhi"`.

**4. What is the output type of `10 > 5` in Python?**  
It is a Boolean (`bool`), which can be `True` or `False`. Example: `type(10 > 5)` returns `bool`.

**5. What is the difference between `"25"` and `25` in Python?**  
`"25"` is text (`str`), while `25` is an integer (`int`). Example: `int("25") + 5` gives `30`.

## 2. Dictionaries

**1. What is a dictionary in Python?**  
A dictionary stores values as key-value pairs. Example: `student = {"name": "Asha", "age": 20}`.

**2. Why do we use key-value pairs in a dictionary?**  
They let us find a value using its key. Example: `student["name"]` returns `"Asha"`.

**3. What is the difference between a list and a dictionary?**  
A list uses positions; a dictionary uses keys. Example: `colors = ["red", "blue"]` and `person = {"name": "Asha"}`.

**4. What happens if we access a key that does not exist in a dictionary?**  
Square-bracket access raises a `KeyError`. Example: `{"name": "Asha"}["age"]` raises `KeyError`.

**5. What is the difference between `get()` and square-bracket access?**  
`get()` can return a default for a missing key; brackets raise `KeyError`. Example: `person.get("age", 0)` returns `0` if the key is missing.

## 3. Exception Handling

**1. What is exception handling in Python?**  
It lets a program respond to errors while running. Example: `try: print(10 / 0)\nexcept ZeroDivisionError: print("Cannot divide by zero")`.

**2. Why do we use `try` and `except` blocks?**  
They let us handle errors instead of stopping unexpectedly. Example: `try: int("abc")\nexcept ValueError: print("Enter a number")`.

**3. What is the difference between a syntax error and an exception?**  
A syntax error means code breaks Python's writing rules; an exception happens while valid code runs. Example: `10 / 0` causes `ZeroDivisionError` when executed.

**4. What is the use of the `finally` block?**  
It runs whether an exception occurs or not. Example: `try: print("Work")\nfinally: print("Finished")`.

**5. What happens if we do not handle exceptions in a program?**  
An unhandled exception usually stops the program and displays a traceback. Example: `print(5 / 0)` raises `ZeroDivisionError`.

## 4. File Handling

**1. What is file handling in Python?**  
It means reading from or writing to files. Example: `with open("notes.txt", "r") as file: text = file.read()`.

**2. Why do we use file handling in Python?**  
It saves information so it can be used later. Example: `with open("notes.txt", "w") as file: file.write("Hello")`.

**3. What is the difference between `r`, `w`, and `a` mode?**  
`r` reads, `w` writes and replaces content, and `a` adds content at the end. Example: `open("notes.txt", "a")` opens a file for appending.

**4. What happens if we open an existing file in `w` mode?**  
Its existing content is erased when the file is opened for writing. Example: `with open("notes.txt", "w") as file: file.write("New text")`.

**5. Why is `with open()` preferred in file handling?**  
It closes the file automatically after the block. Example: `with open("notes.txt", "r") as file: print(file.read())`.

## 5. Function Arguments

**1. What are function arguments in Python?**  
Arguments are values passed to a function call. Example: `greet("Asha")` passes `"Asha"`.

**2. What is the difference between a parameter and an argument?**  
A parameter is a name in the definition; an argument is the value passed in the call. Example: In `def greet(name): print(name)`, `name` is a parameter and `greet("Asha")` passes an argument.

**3. What is the difference between positional and keyword arguments?**  
Positional arguments are matched by order; keyword arguments by parameter name. Example: `show("Asha", age=20)`.

**4. What happens if we pass arguments in the wrong order?**  
The function may use incorrect values or raise an error. Example: `subtract(3, 10)` returns `-7` if the function subtracts its second parameter from its first.

**5. What is the difference between `*args` and `**kwargs`?**  
`*args` collects extra positional arguments in a tuple; `**kwargs` collects keyword arguments in a dictionary. Example: `def show(*args, **kwargs): print(args, kwargs)`.

## 6. Functions

**1. What is a function in Python?**  
A function is a reusable block of code. Example: `def greet(): print("Hello")`.

**2. Why do we use functions in programming?**  
They reduce repeated code and keep programs organised. Example: Call `greet()` whenever you want it to display `Hello`.

**3. What is the difference between a parameter and an argument?**  
A parameter is in the function definition; an argument is passed when calling it. Example: In `def double(n): return n * 2`, `n` is the parameter and `double(4)` passes argument `4`.

**4. What is the difference between `print()` and `return` in a function?**  
`print()` displays a value; `return` sends a value back to the caller. Example: `def add(): return 2 + 3` lets `result = add()` store `5`.

**5. Can a function return more than one value in Python?**  
Yes, Python can return multiple values together, usually as a tuple. Example: `def values(): return 2, 3` returns `(2, 3)`.

## 7. Code Editors and IDEs

**1. What is a code editor?**  
A code editor is an application for writing and editing code. Example: Visual Studio Code can edit Python files.

**2. What is an IDE?**  
An IDE combines a code editor with tools such as running and debugging. Example: PyCharm is a Python IDE.

**3. What is the main difference between an IDE and a code editor?**  
An IDE usually includes more development tools; a basic editor focuses on editing. Example: Notepad is a basic editor, while PyCharm is an IDE.

**4. Why do developers use VS Code for Python programming?**  
It is lightweight and supports Python through extensions. Example: The Python extension helps run and debug code.

**5. Can a code editor become powerful with extensions?**  
Yes, extensions can add language support and debugging features. Example: Install the Python extension in VS Code.

## 8. Lambda Functions

**1. What is a lambda function in Python?**  
A lambda is a short function written as one expression. Example: `square = lambda x: x * x`.

**2. What is the difference between a `def` function and a lambda function?**  
`def` creates a regular function with a block; `lambda` creates a small single-expression function. Example: `def square(x): return x * x`.

**3. Why is a lambda function called an anonymous function?**  
It can be created without a formal function name. Example: `lambda x: x + 1`.

**4. Can a lambda function have multiple arguments?**  
Yes, it can accept multiple arguments but has only one expression. Example: `add = lambda a, b: a + b`.

**5. Where should we avoid using lambda functions in real projects?**  
Avoid them for complex logic that is hard to read; use `def` instead. Example: Use `def calculate_total(price, tax, discount):` for a multi-step calculation.

## 9. Lists

**1. What is a list in Python?**  
A list is an ordered collection of items. Example: `fruits = ["apple", "banana", "mango"]`.

**2. Why do we use lists in Python?**  
They store many values in one variable. Example: `marks = [75, 82, 90]`.

**3. What is the difference between list indexing and list slicing?**  
Indexing gets one item; slicing gets a range. Example: `numbers = [10, 20, 30]; numbers[0]` gives `10`, while `numbers[0:2]` gives `[10, 20]`.

**4. Why is a list called mutable?**  
Its items can be changed after creation. Example: `numbers = [1, 2]; numbers[0] = 9`.

**5. What is the difference between `append()` and `insert()`?**  
`append()` adds at the end; `insert()` adds at a chosen position. Example: `items = [1, 3]; items.insert(1, 2)` gives `[1, 2, 3]`.

## 10. Loops

**1. What is a loop in Python?**  
A loop repeats a block of code. Example: `for i in range(3): print(i)`.

**2. What is the difference between a `for` loop and a `while` loop?**  
A `for` loop commonly goes through a sequence; a `while` loop repeats while a condition is true. Example: `while count < 3: count += 1`.

**3. Why does `range(1, 5)` not print `5`?**  
The stop value is excluded. Example: `list(range(1, 5))` gives `[1, 2, 3, 4]`.

**4. What happens if the condition in a `while` loop never becomes false?**  
The loop continues indefinitely unless stopped another way. Example: `while True: print("Running")` is an infinite loop.

**5. What is the difference between `break` and `continue`?**  
`break` exits the loop; `continue` skips to the next iteration. Example: `for n in range(5):\n    if n == 2: continue\n    print(n)` skips `2`.

## 11. Voting System Project

**1. What is the purpose of the Voting System project?**  
It demonstrates collecting votes and counting them. Example: A user selects a candidate and the program adds one vote.

**2. Why do we use a dictionary in this project?**  
A dictionary stores candidate names and vote counts. Example: `votes = {"Asha": 0, "Ravi": 0}`.

**3. What is the use of `while True` in the voting system?**  
It keeps showing the menu until an exit condition is reached. Example: `while True: choice = input("Vote or type exit: ")`.

**4. What will happen if we do not use `break` in this project?**  
The loop will not exit at that point and may keep asking for input. Example: Entering `exit` will not stop the menu if no exit logic is provided.

**5. How can we find the winner in this voting system?**  
Find the candidate with the highest vote count. Example: `winner = max(votes, key=votes.get)`.

## 12. Modules

**1. What is a module in Python?**  
A module is a Python file containing reusable code. Example: `import math`.

**2. Why do we use modules in Python?**  
They organise and reuse code. Example: `math.sqrt(25)` returns `5.0`.

**3. What is the difference between a built-in module and a user-defined module?**  
A built-in module comes with Python; a user-defined module is made by a programmer. Example: `math` is built in, while `helpers.py` can be your own module.

**4. What is the difference between `import math` and `from math import sqrt`?**  
The first imports the module; the second imports `sqrt` directly. Example: `from math import sqrt; print(sqrt(16))`.

**5. Can we create our own module in Python?**  
Yes, save code in a `.py` file and import it. Example: Create `helpers.py` with `def greet(): print("Hi")`.

## 13. Object-Oriented Programming

**1. What is Object-Oriented Programming in Python?**  
OOP organises code around classes and objects. Example: A `Car` class can describe car objects.

**2. What is the difference between a class and an object?**  
A class is a blueprint; an object is an instance of that blueprint. Example: `car = Car()` creates an object from `Car`.

**3. Why do we use the `__init__()` method in Python?**  
It sets initial values when an object is created. Example: `def __init__(self, name): self.name = name`.

**4. What is the role of `self` in a Python class?**  
`self` refers to the current object and accesses its data. Example: `self.name = name` stores a name on the object.

**5. What is the difference between inheritance and encapsulation?**  
Inheritance reuses features from another class; encapsulation groups data and methods and controls access to them. Example: `class Dog(Animal): pass` shows inheritance.

## 14. Operators

**1. What are operators in Python?**  
Operators perform actions on values. Example: `3 + 2` uses the addition operator.

**2. What is the difference between `/` and `//` in Python?**  
`/` performs normal division; `//` performs floor division. Example: `7 / 2` gives `3.5`, while `7 // 2` gives `3`.

**3. What is the difference between `=` and `==` in Python?**  
`=` assigns a value; `==` compares values. Example: `age = 20; age == 20` evaluates to `True`.

**4. What is the use of the modulus operator `%`?**  
It returns the remainder after division. Example: `7 % 2` gives `1`.

**5. What is the difference between `and` and `or` operators?**  
`and` requires both conditions to be true; `or` requires at least one. Example: `age > 18 and has_id` checks both conditions.

## 15. Packages and pip

**1. What is a package in Python?**  
A package groups related modules. Example: `import email` imports a standard-library package.

**2. What is the difference between a module and a package?**  
A module is usually one Python file; a package groups modules in a directory. Example: `random.py` can be a module, while a directory of related modules can be a package.

**3. Why do we use packages in Python projects?**  
They organise related code and make projects easier to maintain. Example: A project can keep database modules in a `database` package.

**4. What is the use of `pip` in Python?**  
`pip` installs and manages Python packages. Example: `python -m pip install requests`.

**5. What happens if we import a package that is not installed?**  
Python usually raises `ModuleNotFoundError`. Example: `import package_that_is_missing` raises an import error if it cannot be found.

## 16. datetime Module

**1. What is the use of the `datetime` module in Python?**  
It works with dates and times. Example: `import datetime; today = datetime.date.today()`.

**2. What is the difference between `date` and `datetime`?**  
`date` stores year, month, and day; `datetime` also stores time. Example: `datetime.date.today()` returns today's date.

**3. How can we get the current date and time in Python?**  
Use `datetime.now()`. Example: `from datetime import datetime; print(datetime.now())`.

**4. Why do we use `strftime()` in Python?**  
It formats a date or time as text. Example: `datetime.now().strftime("%Y-%m-%d")`.

**5. What happens if we give an invalid date like month `13`?**  
Python raises `ValueError` because month 13 is invalid. Example: `datetime.date(2025, 13, 1)` raises `ValueError`.

## 17. Python Syntax

**1. What is Python syntax?**  
Syntax is the set of rules for writing valid Python code. Example: `print("Hello")` is valid syntax.

**2. Why is indentation important in Python?**  
Indentation shows which statements belong to a block. Example: `if True:\n    print("Yes")`.

**3. What happens if indentation is wrong in Python?**  
Python may raise `IndentationError`, or code may run in an unintended block. Example: An unindented statement after `if True:` can cause `IndentationError`.

**4. Is Python case-sensitive?**  
Yes, uppercase and lowercase names are different. Example: `name` and `Name` are different variables.

**5. What is the use of comments in Python?**  
Comments explain code to readers and are ignored during execution. Example: `# Store the user's age`.

## 18. Sets

**1. What is a set in Python?**  
A set is an unordered collection of unique items. Example: `numbers = {1, 2, 3}`.

**2. Why does a set remove duplicate values automatically?**  
Sets only keep unique elements. Example: `set([1, 1, 2])` gives `{1, 2}`.

**3. What is the difference between a list and a set?**  
A list is ordered and allows duplicates; a set stores unique items and has no positional indexing. Example: `[1, 1, 2]` keeps duplicates, while `{1, 1, 2}` becomes `{1, 2}`.

**4. Why can we not access set items using an index number?**  
Sets do not support positional indexing. Example: `2 in numbers` checks membership instead of using `numbers[0]`.

**5. What is the difference between `union()` and `intersection()`?**  
`union()` combines items from both sets; `intersection()` returns shared items. Example: `{1, 2}.intersection({2, 3})` gives `{2}`.

## 19. String Methods

**1. What are string methods in Python?**  
They are built-in operations for working with text. Example: `"hello".upper()` gives `"HELLO"`.

**2. What is the difference between `upper()` and `lower()`?**  
`upper()` makes letters uppercase; `lower()` makes them lowercase. Example: `"PyThOn".lower()` gives `"python"`.

**3. Why do we use `strip()` while taking user input?**  
It removes whitespace from the beginning and end of text. Example: `name = input("Name: ").strip()`.

**4. What is the difference between `find()` and `count()`?**  
`find()` returns the first match's position; `count()` counts matches. Example: `"banana".count("a")` returns `3`.

**5. What happens if `find()` does not get the searched text?**  
It returns `-1`. Example: `"hello".find("z")` returns `-1`.

## 20. Strings

**1. What is a string in Python?**  
A string is text inside quotes. Example: `message = "Hello"`.

**2. What is the difference between single and double quotes in Python strings?**  
Both create strings; choose the one that makes the text easier to write. Example: `message = "I'm learning Python"`.

**3. Why does Python string indexing start from `0`?**  
Python uses zero-based indexing, so the first character is at position 0. Example: `"cat"[0]` returns `"c"`.

**4. What is the difference between indexing and slicing?**  
Indexing selects one character; slicing selects a range. Example: `word = "Python"; word[0]` gives `"P"`, while `word[0:2]` gives `"Py"`.

**5. What happens if we try to change one character of a string directly?**  
It raises `TypeError` because strings are immutable. Example: `word = "cat"; word[0] = "b"` raises `TypeError`.

## 21. Tuples

**1. What is a tuple in Python?**  
A tuple is an ordered collection that cannot be changed after creation. Example: `point = (3, 4)`.

**2. Why do we use tuples in Python?**  
They keep a fixed group of values together. Example: `rgb = (255, 0, 0)` stores colour values.

**3. What is the difference between a list and a tuple?**  
Lists can be changed; tuples cannot be changed after creation. Example: `[1, 2]` is a list and `(1, 2)` is a tuple.

**4. Why is a tuple called immutable?**  
Its items cannot be reassigned after creation. Example: `point = (1, 2); point[0] = 5` raises `TypeError`.

**5. Can we change a tuple item after creating it?**  
No, tuple items cannot be reassigned. Example: `values = (10, 20)` cannot have `values[0]` reassigned.

## 22. Type Casting

**1. What is type casting in Python?**  
It converts a value from one data type to another. Example: `int("25")` returns `25`.

**2. Why do we need type casting while taking user input?**  
`input()` returns text, so convert it when you need a number. Example: `age = int(input("Enter age: "))`.

**3. What is the difference between `int()` and `float()`?**  
`int()` converts to an integer; `float()` converts to a decimal number. Example: `float("4.5")` returns `4.5`.

**4. What happens if we write `int("Delhi")` in Python?**  
Python raises `ValueError` because the text is not an integer. Example: `int("Delhi")` raises `ValueError`.

**5. Why do we use `str()` while joining numbers with text?**  
It converts a value to text so it can be combined with a string. Example: `"Age: " + str(20)` gives `"Age: 20"`.

## 23. Variables

**1. What is a variable in Python?**  
A variable is a name that refers to a value. Example: `score = 100`.

**2. Why do we use variables in Python?**  
They store values that can be reused. Example: `price = 50; total = price * 2`.

**3. What are the rules for writing variable names in Python?**  
Names may contain letters, digits, and underscores; they cannot start with a digit or be a keyword. Example: `student_name = "Asha"` is valid.

**4. Can we change the value of a variable after creating it?**  
Yes, assign a new value to it. Example: `score = 10; score = 20`.

**5. What is the difference between `name`, `Name`, and `NAME` in Python?**  
They are different names because Python is case-sensitive. Example: `name = "A"; Name = "B"; NAME = "C"`.

## 24. Installing Python

**1. What is Python installation?**  
It is setting up Python on your computer so you can run programs. Example: Download it from [python.org](https://www.python.org/downloads/).

**2. Why do we select “Add python.exe to PATH”?**  
It lets you run Python from a terminal without typing the full installation path. Example: `python --version` can show the installed version.

**3. How can we install Python from Microsoft Store?**  
Open Microsoft Store, search for Python, choose a version, and select Install. Example: Search for “Python 3.12” and install it if available.

**4. How do you check the Python version?**  
Run a version command in the terminal. Example: `python --version`.

**5. What is pip?**  
`pip` is Python's package installer. Example: `python -m pip install requests`.

## 25. `break`, `continue`, and `pass`

**1. What is the use of `break` in Python?**  
It immediately exits the nearest loop. Example: `for n in range(5):\n    if n == 2: break\n    print(n)`.

**2. What is the difference between `break` and `continue`?**  
`break` ends the loop; `continue` skips the current iteration. Example: `for n in range(3):\n    if n == 1: continue\n    print(n)` prints `0` and `2`.

**3. Why do we use `pass` in Python?**  
It is a placeholder when a statement is required but no action is needed yet. Example: `def future_function(): pass`.

**4. What happens if `continue` is used before a `print()` statement inside a loop?**  
The `print()` is skipped for that iteration. Example: `for n in range(3):\n    if n == 1: continue\n    print(n)` does not print `1`.

**5. Can `pass` stop a loop like `break`?**  
No, `pass` does nothing and does not stop the loop. Example: `for n in range(2): pass` completes both iterations.

## 26. Built-in Functions

**1. What are built-in functions in Python?**  
They are functions available without importing a module. Example: `len("Python")` returns `6`.

**2. What is the use of the `print()` function?**  
It displays information on the screen. Example: `print("Hello, world!")`.

**3. Why does `input()` return a value as a string?**  
It reads what the user types as text; convert it if you need another type. Example: `age = int(input("Age: "))`.

**4. What is the difference between `type()` and `len()`?**  
`type()` tells a value's data type; `len()` gives the number of items or characters in a supported object. Example: `type("cat")` returns `str`, while `len("cat")` returns `3`.

**5. What happens if we use `len()` on an integer value?**  
Python raises `TypeError` because an integer has no length. Example: `len(123)` raises `TypeError`.

## 27. Comments

**1. What are comments in Python?**  
Comments are notes for people reading the code. Example: `# Calculate the total`.

**2. Why do we use comments in Python?**  
They explain code and make it easier to maintain. Example: `# Add the prices together`.

**3. Which symbol is used for a single-line comment in Python?**  
The hash symbol `#` starts a single-line comment. Example: `# This is a comment`.

**4. Does Python execute comments?**  
No, Python ignores comments during normal execution. Example: `# print("Hello")` does not print anything.

**5. What is the difference between a comment and a string in Python?**  
A comment is ignored by Python; a string is a value the program can use. Example: `message = "Hello"` stores a string, while `# Hello` is a comment.

## 28. Conditional Statements

**1. What are conditional statements in Python?**  
They let a program choose what to do based on a condition. Example: `if age >= 18: print("Adult")`.

**2. What is the difference between `if` and `if-else`?**  
`if` runs code when its condition is true; `if-else` also provides a path when it is false. Example: `if age >= 18: print("Adult")\nelse: print("Minor")`.

**3. Why do we use `elif` in Python?**  
It checks another condition when earlier conditions are false. Example: `if score >= 90: print("A")\nelif score >= 75: print("B")`.

**4. What happens if two `elif` conditions are true?**  
Only the first true condition in an `if`/`elif` chain runs. Example: `if score >= 50: print("Pass")\nelif score >= 40: print("Near pass")` prints `Pass` for `score = 60`.

**5. What is a nested conditional statement?**  
It is an `if` statement inside another conditional block. Example: `if age >= 18:\n    if has_id:\n        print("Entry allowed")`.

---

## 🚀 How to Upload This README to GitHub

1. Create a new repository on GitHub.
2. Add a file named `README.md`.
3. Paste this content into the file.
4. Commit the changes.

Happy learning! ⭐
