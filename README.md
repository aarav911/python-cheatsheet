# ==============================================================================
# THE ULTIMATE PYTHON CHEATSHEET (THE BASICS)
# ==============================================================================

# 1. HELLO WORLD & PRINTING
print("Hello, World!")  # Standard print
print("Apple", "Banana", sep=" | ")  # Custom separator -> Apple | Banana
print("No newline", end="")  # Keeps cursor on the same line


# ==============================================================================
# 2. VARIABLES & DATA TYPES
# ==============================================================================
x = 5  # Integer (int)
y = 3.14  # Floating point (float)
name = "Alice"  # String (str)
is_active = True  # Boolean (bool) - Must be capitalized True/False
nothing = None  # NoneType (represents absence of value)

# Checking types & Type Conversion (Casting)
type_of_x = type(x)  # <class 'int'>
string_five = str(5)  # Converts int to str ("5")
int_three = int(3.9)  # Truncates to int (3)
float_two = float("2.5")  # Converts str to float (2.5)


# ==============================================================================
# 3. BASIC OPERATORS
# ==============================================================================
# Arithmetic
addition = 5 + 2  # 7
subtraction = 5 - 2  # 3
multiplication = 5 * 2  # 10
division = 5 / 2  # 2.5 (Always returns a float)
floor_division = 5 // 2  # 2 (Rounds down to nearest whole number)
modulus = 5 % 2  # 1 (Remainder of division)
exponentiation = 5**2  # 25 (5 to the power of 2)

# Comparison (Returns True or False)
# == (equal), != (not equal), > (greater), < (less), >=, <=

# Logical
# and (both true), or (at least one true), not (inverts boolean)


# ==============================================================================
# 4. STRINGS & STRING METHODS
# ==============================================================================
text = "  Python Programming  "

# Slicing: text[start:stop:step] (stop index is excluded)
substring = text[2:8]  # "Python"
reversed_text = text[::-1]  # Reverses the string

# Useful Methods
stripped = text.strip()  # "Python Programming" (Removes leading/trailing whitespace)
lower_case = text.lower()  # "  python programming  "
upper_case = text.upper()  # "  PYTHON PROGRAMMING  "
replaced = text.replace("Python", "Java")  # "  Java Programming  "
split_words = "a,b,c".split(",")  # ['a', 'b', 'c'] (Returns a list)

# String Formatting (f-Strings)
age = 25
greeting = f"Hello, my name is {name} and I am {age} years old."


# ==============================================================================
# 5. DATA STRUCTURES (LISTS, TUPLES, DICTIONARIES, SETS)
# ==============================================================================

# --- LISTS (Ordered, mutable, allows duplicates) ---
fruits = ["apple", "banana", "cherry"]
fruits[0] = "blueberry"  # Modifying item
fruits.append("orange")  # Adds to the end
fruits.insert(1, "kiwi")  # Inserts at index 1
fruits.remove("banana")  # Removes item by value
popped_item = fruits.pop()  # Removes and returns last item
list_length = len(fruits)  # Gets length of list

# --- TUPLES (Ordered, IMMUTABLE, allows duplicates) ---
# Used for data that shouldn't change
coordinates = (10.0, 20.0)
# coordinates[0] = 15.0  # ERROR! Tuples cannot be changed.

# --- DICTIONARIES (Key-Value pairs, unordered, mutable, keys must be unique) ---
user = {"name": "Bob", "age": 30, "city": "New York"}
user_name = user["name"]  # Accessing value -> 'Bob'
user_age = user.get("age", 0)  # Safer access method (returns default 0 if key missing)
user["profession"] = "Engineer"  # Adding new key-value pair
user["age"] = 31  # Updating value
del user["city"]  # Removing a key

# --- SETS (Unordered, mutable, UNIQUE elements only) ---
unique_numbers = {1, 2, 3, 3, 4}  # Result: {1, 2, 3, 4}
unique_numbers.add(5)


# ==============================================================================
# 6. CONDITIONAL STATEMENTS (IF / ELIF / ELSE)
# ==============================================================================
score = 85

if score >= 90:
    print("Grade: A")
elif score >= 80:
    print("Grade: B")  # This will execute
else:
    print("Grade: C or below")

# Inline If Statement (Ternary Operator)
status = "Adult" if age >= 18 else "Minor"


# ==============================================================================
# 7. LOOPS (FOR & WHILE)
# ==============================================================================

# For Loop with range(start, stop, step)
for i in range(1, 4):  # Loops 1, 2, 3 (excludes 4)
    print(f"Iteration {i}")

# Iterating over a list
for fruit in ["apple", "banana", "cherry"]:
    if fruit == "banana":
        continue  # Skips the rest of this loop iteration
    print(fruit)

# While Loop
counter = 0
while counter < 3:
    print(f"Counter: {counter}")
    counter += 1  # Equivalent to counter = counter + 1


# ==============================================================================
# 8. FUNCTIONS
# ==============================================================================
def greet_user(username, greeting_word="Hello"):
    """This is a docstring describing the function."""
    return f"{greeting_word}, {username}!"


# Calling the function
message1 = greet_user("Charlie")  # Uses default parameter -> "Hello, Charlie!"
message2 = greet_user("Diana", greeting_word="Welcome")  # "Welcome, Diana!"

# Lambda (Anonymous) Functions - short, single-expression functions
square = lambda n: n**2
print(square(4))  # 16


# ==============================================================================
# 9. ERROR & EXCEPTION HANDLING
# ==============================================================================
try:
    result = 10 / 0
except ZeroDivisionError as e:
    print(f"Error caught: {e}")
except TypeError:
    print("Handled a different type of error")
else:
    print("Runs only if NO exceptions were raised")
finally:
    print("This ALWAYS runs, no matter what")


# ==============================================================================
# 10. FILE HANDLING (I/O)
# ==============================================================================
# Using 'with' automatically closes the file when done
# 'w' = write (overwrites), 'r' = read, 'a' = append

# Writing to a file
with open("test.txt", "w") as file:
    file.write("Line 1: Hello File!\nLine 2: Python is fun.")

# Reading from a file
with open("test.txt", "r") as file:
    content = file.read()
    print(content)


# ==============================================================================
# 11. LIST COMPREHENSIONS (Pythonic shortcuts)
# ==============================================================================
# Standard way to square numbers
squares = []
for n in range(1, 6):
    squares.append(n**2)

# List Comprehension way (Saves lines, faster)
squares_cool = [n**2 for n in range(1, 6)]  # [1, 4, 9, 16, 25]

# With a condition: only square even numbers
even_squares = [n**2 for n in range(1, 6) if n % 2 == 0]  # [4, 16]
