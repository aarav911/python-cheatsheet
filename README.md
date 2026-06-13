
# Python Basics Cheatsheet

A concise, high-density reference guide covering the fundamental syntax and core concepts of Python 3. Designed for quick lookup and immediate implementation.

---

## 1. Hello World & Printing

```python
# Standard print
print("Hello, World!")

# Print multiple items with a custom separator
print("Apple", "Banana", "Cherry", sep=" | ")  # Output: Apple | Banana | Cherry

# Keep the cursor on the same line (override default newline character)
print("No newline ", end="")
print("continues on same line.")

```



## 2. Variables, Data Types & Casting

```python
# Core Data Types
x = 5                  # Integer (int)
y = 3.14               # Floating point (float)
name = "Alice"         # String (str)
is_active = True       # Boolean (bool) - Must be capitalized True/False
nothing = None         # NoneType (explicit absence of value)

# Inspecting Types
print(type(x))         # <class 'int'>

# Explicit Type Conversion (Casting)
string_five = str(5)   # Int to String -> "5"
int_three = int(3.9)   # Float to Int (Truncates decimal) -> 3
float_two = float("2") # String to Float -> 2.0

```

---

## 3. Operators

### Arithmetic Operators

```python
addition = 5 + 2         # 7
subtraction = 5 - 2      # 3
multiplication = 5 * 2   # 10
division = 5 / 2         # 2.5 (Always returns a float)
floor_division = 5 // 2  # 2 (Rounds down to nearest whole number)
modulus = 5 % 2          # 1 (Remainder of division)
exponentiation = 5 ** 2  # 25 (5 raised to the power of 2)

```

### Comparison & Logical Operators

```python
# Comparison (Returns True or False)
# == (Equal), != (Not Equal), > (Greater Than), < (Less Than), >=, <=

# Logical
# and (Both conditions true), or (At least one true), not (Inverts boolean)

```

---

## 4. Strings & String Methods

```python
text = "  Python Programming  "

# Slicing: text[start:stop:step] (stop index is excluded)
substring = text[2:8]        # "Python"
reversed_text = text[::-1]    # Reverses the string

# Common String Methods
stripped = text.strip()       # "Python Programming" (Removes leading/trailing whitespace)
lower_case = text.lower()     # "  python programming  "
upper_case = text.upper()     # "  PYTHON PROGRAMMING  "
replaced = text.replace("P", "J")  # "  Jython Jrogramming  "
split_words = "a,b,c".split(",")   # ['a', 'b', 'c'] (Returns a list)

# String Formatting (f-Strings)
age = 25
greeting = f"Hello, my name is {name} and I am {age} years old."

```

---

## 5. Built-in Data Structures

### Lists (Ordered, mutable, allows duplicates)

```python
fruits = ["apple", "banana", "cherry"]
fruits[0] = "blueberry"      # Modify element
fruits.append("orange")      # Add to the end
fruits.insert(1, "kiwi")     # Insert at index 1
fruits.remove("banana")      # Remove item by value
popped_item = fruits.pop()   # Remove and return last item
list_length = len(fruits)    # Get length of list

```

### Tuples (Ordered, immutable, allows duplicates)

```python
# Used for fixed, read-only data
coordinates = (10.0, 20.0)
# coordinates[0] = 15.0      # ERROR: Tuples cannot be modified after creation

```

### Dictionaries (Key-Value pairs, mutable, keys must be unique)

```python
user = {"name": "Bob", "age": 30, "city": "Mumbai"}
user_name = user["name"]     # Access value (Raises KeyError if key missing)
user_age = user.get("age", 0)# Safe access (Returns default 0 if key missing)
user["role"] = "Engineer"    # Add new key-value pair
user["age"] = 31             # Update value
del user["city"]             # Delete key-value pair

```

### Sets (Unordered, mutable, unique elements only)

```python
unique_numbers = {1, 2, 3, 3, 4}  # Evaluates to {1, 2, 3, 4}
unique_numbers.add(5)             # Add element

```

---

## 6. Control Flow (Conditionals & Loops)

### Conditionals

```python
score = 85

if score >= 90:
    print("Grade: A")
elif score >= 80:
    print("Grade: B")
else:
    print("Grade: C or below")

# Inline If (Ternary Operator)
status = "Adult" if age >= 18 else "Minor"

```

### For Loops

```python
# Loop over a range (start, stop, step) - excludes stop index
for i in range(1, 4):
    print(f"Iteration {i}")  # Prints 1, 2, 3

# Loop over iterable collections
for fruit in ["apple", "banana", "cherry"]:
    if fruit == "banana":
        continue  # Skip remaining code in loop for this item, proceed to next
    if fruit == "cherry":
        break     # Terminate loop entirely
    print(fruit)

```

### While Loops

```python
counter = 0
while counter < 3:
    print(f"Counter: {counter}")
    counter += 1  # Increment to avoid infinite loop

```

---

## 7. Functions

```python
# Define function with default arguments
def greet_user(username, greeting_word="Hello"):
    """Optional docstring explaining the function's purpose."""
    return f"{greeting_word}, {username}!"

# Calling functions
msg1 = greet_user("Aarav")                          # Uses default parameter -> "Hello, Aarav!"
msg2 = greet_user("Diana", greeting_word="Welcome") # Overrides default parameter -> "Welcome, Diana!"

# Lambda (Anonymous / One-Liner) Functions
square = lambda n: n ** 2
print(square(4))  # 16

```

---

## 8. Exception Handling

```python
try:
    result = 10 / 0
except ZeroDivisionError as e:
    print(f"Error caught: {e}")
except (TypeError, ValueError):
    print("Handled multiple potential exception types")
else:
    print("Executes ONLY if the try block ran without raising errors")
finally:
    print("This block ALWAYS runs (e.g., used for resource cleanup)")

```

---

## 9. File Input/Output (I/O)

```python
# Using 'with' context manager ensures files are closed automatically after execution
# Modes: 'w' (write/overwrite), 'r' (read), 'a' (append)

# Writing text to a file
with open("output.txt", "w") as file:
    file.write("Line 1: Structuring documentation.\nLine 2: Python scripting.")

# Reading text from a file
with open("output.txt", "r") as file:
    content = file.read()
    print(content)

```

---

## 10. List Comprehensions

```python
# Traditional approach
squares = []
for n in range(1, 6):
    squares.append(n ** 2) # [1, 4, 9, 16, 25]

# Pythonic syntax (List Comprehension)
squares_clean = [n ** 2 for n in range(1, 6)]

# List Comprehension with an active conditional filtering step
even_squares = [n ** 2 for n in range(1, 6) if n % 2 == 0] # [4, 16]

```

```

```
