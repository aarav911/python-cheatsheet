# Python Programming and Data Structures

Generated comprehensive compilation of custom Python curriculum engineering notes.

---

# Module 1: Introduction & Local Setup

# What Is Python and What Are Some Common Uses in the Industry?

Python is a general-purpose programming language known for its simplicity and ease of use. This ease of use has made Python the most popular programming language in modern times.

Python is used in many fields like data science and machine learning, web development, scripting and automation, embedded systems, IoT, and much more.

Python is the main language that most data scientist and machine learning engineers currently use. Libraries like Pandas and Numpy make data analysis less tedious, while others like Tensorflow and Scikit make machine learning and working with AI models much more accessible.

In web development, Python frameworks like Django, FastAPI, and Flask let developers build scalable and secure back-end systems with minimal effort. Many social media platforms like Instagram and Pinterest use Python on the back-end.

Cybersecurity professionals and ethical hackers use Python to detect vulnerabilities like malware and other viruses, build automated security scans, and analyze threats.

Python runs well on microcomputers like the Raspberry Pi and MicroPython-compatible boards, so you can build all kinds of IoT projects like smart home devices, weather monitoring stations, and more.

Python is widely used in DevOps for writing CI/CD scripts and managing infrastructure across development pipelines. It is also commonly used to build back-end services and internal APIs.

In software testing, Python tools such as pytest are used to create reliable test suites, while system administrators rely on Python for server monitoring, log management, and system-level tasks.

Finally, one of Python's biggest strengths is automation. You can write simple scripts to help you with repetitive tasks like extracting data from spreadsheets, sending emails, and working with files on your local machine.

Libraries like Selenium and BeautifulSoup also make it easy to interact with websites, so you can scrape public data, automate tasks through a web UI, and even manage cloud deployments for your projects.

As you can see, Python is a very powerful language, and yet, it's easy to learn. From simple automation scripts to large-scale, industrial-level applications, you can use Python for just about anything.

Python is a great choice for anyone who wants to learn programming, regardless of what they choose to specialize in later.

---

# How Do You Install, Configure and Use Python in Your Local Environment?

For all of the workshops and labs, you will be using freeCodeCamp's Python editor. But it is important to learn how to set up Python on your local machine.

The easiest way to install Python on Windows and Mac is to download the installer from the official Python website. We'll also go over running Python on Linux later in this lesson.

Go to `https://www.python.org/` and hover over "Downloads". A modal will appear showing the current version of Python for your operating system (OS).

We'll go over how to install Python on a computer running macOS first:

* Click on the button showing the current version of Python (from the previous modal), and you'll start downloading a `.pkg` installation file automatically.
* Once the `.pkg` installer is finished downloading, open it, then click "Continue" in the window that opens up.
* Continue clicking the "Continue" button until you get to the "Installation Type" section. There, click the "Install" button.
* Enter your password if necessary, then start the installation.
* After that, you should get a congratulations message saying that Python has been successfully installed.
* Click the "Close" button, and you're done!

You can verify the installation by opening up your terminal and running `python --version` or `python3 --version`.

You can also open the Python interpreter by running `python` or `python3` in the terminal. A Python interpreter is the program that reads Python code, translates it into instructions the computer understands and executes those instructions.

A terminal is a text-based interface that lets you interact with your computer by typing commands. Each operating system comes with a default terminal app. On macOS, you can use the Terminal app. On Windows, you can use Command Prompt or PowerShell. On Linux, each desktop environment has its own default terminal app, like GNOME Terminal or Konsole.

Note that, on some older macOS and Linux systems, `python` can be reserved for Python 2, while `python3` is for Python 3 specifically. If you run `python --version` and see a version of Python 2 like `Python 2.7.18`, then it's possible that your OS relies on some software that was written in the older version of Python. If that's the case, you should use `python3` to run your Python code going forward. Python 2 is end-of-life and should not be used for any new development.

To install Python on Windows, follow these steps:

* Go to `https://www.python.org/`, and hover over “Downloads“. You should see a modal that says "Download for Windows" and a download button with the current version of Python.
* Click on the version number, and you'll start downloading a Windows executable (`.exe`) file automatically.
* Once you've finished downloading the Python installer for Windows, double-click on it, and follow the instructions.
* When you see the option `Add python.exe to Path`, check that option, then click `Install Now`. Doing that will make things easier for you later.

You can verify the installation by opening up a command line shell like PowerShell and running `python --version`. You can also open the Python interpreter by running `python`.

For Python on Linux, most major distros like Ubuntu, Debian, and Fedora come with Python.

Just open a terminal and run `python --version`, or `python3 --version`:

If either command doesn't show a version of Python, you can search for an installation package for your flavor of Linux at `https://www.python.org`, or search online for the recommended way to install Python for your distro.

---

# How to Run Python Scripts

In the previous lesson, you learned how to install Python on your local device. In this lesson, you will learn how to run Python code locally.

Before you can start building your Python scripts locally, you will need to install a code editor or IDE. IDE stands for Integrated Development Environment and it has features including a code editor, testing tools, a terminal and more.

One popular code editor that many developers use is VS Code. Visit `https://code.visualstudio.com/download` to download VS Code which supports Mac, Windows and Linux environments. This is the editor that will be used in this lesson.

Other common choices for Python development include the following:

* PyCharm
* Spyder

Once you have downloaded your editor, you will need to open it. Once it is opened, you will need to open a folder. You can click on the `File` menu option in the upper left hand corner and click on `Open Folder`. From there, you can choose or create a folder for your project. For extra practice outside of the lesson, you might want a folder named `python-projects`.

Once you have your folder set up, you can open the explorer which is the left sidebar in VS Code. Click on the `New File` icon which looks like a piece of paper with a plus icon over it. Then create a file called `main.py` and press enter. The `.py` is a file extension signalling this is a Python file.

Open up your `main.py` file and type the following code:

```python
print("Hello, world!")
```

To run this code, you have a few options. The first option is to click on the run button which looks like a play button located in the upper right hand corner. That will open a terminal and run your Python script there. You should see the text `"Hello, world!"`.

Another option is to open a terminal and manually run the program using:

```python
python main.py
```

You must run this command from the folder where `main.py` is saved. For example, if `main.py` is inside a folder called `python-projects`, first use the following in the terminal:

```python
cd python-projects
```

Then run:

```python
python main.py
```

In some environments, especially on macOS and Linux systems where Python 2 and Python 3 are both installed, you may need to use `python3` instead of `python`. This is common when the `python` command either does not exist or points to an older version of Python.

```python
python3 main.py
```

As you progress throughout the course, you should try the examples from the lessons locally and see the results. You should also try to come up with your own examples to test what you have learned from the lessons.

---

# How to Use the Python Interactive Shell

In the previous lesson, you learned how to run Python scripts locally. But there might be times where you don't want to create full Python programs and just need to test out some Python code. This is where the Python interactive shell comes in.

But first, let's review what a terminal is.

A terminal is a text-based interface that lets you interact with your computer by typing commands. Each operating system comes with a default terminal app. On macOS, you can use the Terminal app. On Windows, you can use Command Prompt or PowerShell. On Linux, each desktop environment has its own default terminal app, like GNOME Terminal or Konsole.

Open up a terminal app and type in `python` and press `Enter`. This will start a Python interactive shell. An interactive shell is a program that lets you type commands one at a time and see the results.

When you start a new session, you might see this type of output initially:

```python
Python 3.12.2 (main, Mar 21 2024, 22:48:26) [Clang 14.0.3 (clang-1403.0.22.14.1)] on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>>
```

The `>>>` symbol means Python is waiting for you to type a command. Try printing `"Hello, world!"` to the terminal:

```python
print("Hello, world!")
```

You should see the text appear like this:

```python
>>> print("Hello, world!")
Hello, world!
```

After the text is printed, Python goes back to the following:

```python
>>>
```

This means you can type in another command.

The Python interpreter is following what is known as the Read, Evaluate, Print, Loop cycle. Or REPL for short. Whenever you type in commands, the interpreter will read the input, evaluate it, print the result and loop back to show the `>>>` so you can type more commands.

What happens if you try to type in an invalid command like this?

```python
>>> something random
```

Well, the Python interpreter will still follow the same REPL process. In this case, you will get an error message:

```python
>>> something random
  File "<stdin>", line 1
    something random
              ^^^^^^
SyntaxError: invalid syntax
```

If you want to leave the interactive shell you can type `exit()` or press `Ctrl + D` for (Mac/Linux) or `Ctrl + Z + Enter` for (Windows).

Using Python's interactive shell is great for small experiments with code or basic exploration. While you are going through the remaining lessons in the course, you can type in some of the new methods you learned inside an interactive shell.

If you are planning to work with longer programs or working across multiple files, then it is better to work in a code editor or IDE.

---

## Module Review Component

# Python Installation Review

Python in Your Local Environment
--------------------------------

* **Installation**: The best way to install Python on Windows, Mac, and Linux is to download the installer from the official Python website (`https://www.python.org/`).
* **Terminal**: A text-based interface that lets you interact with your computer by typing commands. Each operating system comes with a default terminal app. On macOS, you can use the Terminal app. On Windows, you can use Command Prompt or PowerShell. On Linux, each desktop environment has its own default terminal app, like GNOME Terminal or Konsole.
* **IDE**: IDE stands for Integrated Development Environment and it has features including a code editor, testing tools, a terminal and more.
* **Popular Code Editors and IDEs for Python**: VS Code, PyCharm, and Spyder
* **Running Code Locally**: To run Python code, you have a few options. The first option is to click on the run button in VS Code which looks like a play button located in the upper right hand corner. That will open a terminal and run your Python script there.

Another option is to open a terminal and manually run the program. Here is an example to run a program called `main.py`:

```python
python main.py
```

You must run this command from the folder where `main.py` is saved. For example, if `main.py` is inside a folder called `python-projects`, first use the following in the terminal:

```python
cd python-projects
```

Then run:

```python
python main.py
```

Using the Python Interactive Shell
----------------------------------

* **Definition**: An interactive shell is a program that lets you type commands one at a time and see the results. Open up a terminal app and type in `python` and press `Enter`. This will start a Python interactive shell. The `>>>` symbol means Python is waiting for you to type a command. Try printing `"Hello, world!"` to the terminal:

```python
print("Hello, world!")
```

You should see the text appear like this:

```python
>>> print("Hello, world!")
Hello, world!
```

After the text is printed, Python goes back to the following:

```python
>>>
```

This means you can type in another command.

* **Read, Evaluate, Print, Loop cycle (REPL)**: Whenever you type in commands, the interpreter will read the input, evaluate it, print the result and loop back to show the `>>>` so you can type more commands.

---

# Module 2: Python Basics - Variables, Data Types, and Numbers

# How Do You Declare Variables and What Are Naming Conventions to Name Variables?

In Python, variables are like a labelled box for storing and referencing data of different types. To declare variables in Python, you assign a value to an identifier with the assignment (`=`) operator. You don't need to use special keywords like `let` or `const` in JavaScript, or `char` in C#.

In Python, you just write the name of the variable on the left, followed by the assignment operator, and the value you want to assign the variable on the right. Here's an example of how to declare `name` and `age` variables:

```python
name = 'John Doe'
age = 25
```

In the example above, the variable `name` holds the value `'John Doe'`. This value is a string, which is a series of characters used to represent text. Strings are written with single or double quotes, for example `'Hello'` or `"Hello"`. In future lessons, you'll learn more about working with strings in Python.

When naming variables in Python, there are some important rules you should keep in mind:

* Variable names can only start with a letter or an underscore (`_`), not a number.
* Variable names can only contain alphanumeric characters (`a-z`, `A-Z`, `0-9`) and underscores (`_`).
* Variable names are case-sensitive — `age`, `Age`, and `AGE` are all considered unique.
* Variable names cannot be one of Python's reserved keywords such as `if`, `class`, or `def`.

If you break any of those rules, your Python program will throw a `SyntaxError`:

```python
    5variable_name = 5
     ^
SyntaxError: invalid syntax
```

Now let's go over some common naming conventions for variables in Python.

First, variables names should be in lowercase, with separate words separated by an underscore. This is called snake case:

```python
my_variable_name = 'freeCodeCamp'
```

Next, you should use descriptive names for variables. For example, if you want to save a user's age as a variable, `user_age` is better than `age` or an abbreviation like `ua`:

```python
user_age = 30
```

This way, you can easily communicate the purpose of a variable to other team members (or to your future self) in a large codebase.

Another convention is to avoid using single-letter variable names. This is very common in Python, but should be avoided because variable names with a single letter communicate no purpose or meaning:

```python
x = 56 # What do you mean by x?
```

The pound symbol (`#`) and the text that follows in the example above is called a comment. You might already be familiar with comments, so let's go over them quickly and explain how they work.

In Python, comments start with a pound symbol (`#`), and the language ignores everything after the `#` symbol on that line:

```python
# This is a single-line comment
```

Multi-line comments can be created by using consecutive single-line comments:

```python
# This is a
# multi-line
# comment
```

You can use comments to explain your code, leave reminders for yourself, or clarify why a line exists. Comments are especially helpful when you're learning or working in teams.

However, you shouldn't use comments to explain what your variable names mean. Instead, the names you choose for your variables should be descriptive and communicate what they're for, and follow the other naming rules mentioned earlier to prevent syntax errors.

---

# How Does the Print Function Work?

Every programming language has some way to output data to the terminal with a built-in method, function, property, or keyword. In Python, you can use the `print` function to print data to the terminal. Let's take a closer look at the `print` function so you can start using it with confidence.

One of the first things you do when you're learning any programming language is to write a simple `Hello world!` program. You can do that really easily in Python with just the `print` function.

To do that, you just need to put the string `Hello world!` in between the opening and closing parentheses you use to call the `print` function:

```python
print('Hello world!') # Hello world!
```

You will learn more about strings and functions in Python in future lessons. For now, just consider strings as a sequence of characters surrounded by either single (`'`) or double (`"`) quotation marks.

In the `print('Hello world!')` example, the string `'Hello world!'` is an **argument** passed to the `print` function. You can also use the `print` function to show multiple values, or arguments, at once by separating them with commas. For example:

```python
print('My favorite colors are', 'blue', 'green', 'red')

# Output: My favorite colors are blue green red
```

Python automatically adds a space between each item when you separate them with commas. This is helpful when you want to print several pieces of information together.

---

# What Are Common Data Types in Python?

Before working with Python variables, it's important to understand data types. A data type describes the kind of value a variable holds. For example, a number, a piece of text, or a list of items. Programming languages use data types so they know how to store and work with different kinds of information.

Python is a dynamically-typed language like JavaScript, meaning you don't need to explicitly declare types for variables. The language knows what data type a variable is based on what you assign to it.

Here are some examples:

```python
name = 'John Doe' # Python knows this is a string
age = 25 # Python knows this is an integer
```

This is in contrast to some statically-typed languages like C#, Java, and C++, where you have to declare types with variables, like this:

```python
string name = 'John Doe'
int age = 25
```

The dynamic-typing nature of Python makes coding really fast and more flexible, but it can lead to unexpected bugs because type errors are detected only when a program runs, not when the program compiles.

Since Python determines data types while your program is **running**, type-related mistakes are only discovered at that moment. When a program runs, Python executes your code line by line. If it reaches a line where a certain object is expected to behave in a way it's not able to, Python will stop and show an error.

In contrast, some languages **compile** your program before it runs. Compiling means the computer checks your code in advance and prepares it to run. During this step, those languages can catch type errors before the program even starts.

You don't need to know those languages yet. The important idea is simply:

* **In Python type errors can reveal themselves during execution**, when the program is actually running and using your code.
* **Compiled languages catch type errors during the compile step**, before the program is allowed to run.

Because of this, you might not learn about a type mistake in Python until the program reaches that specific line of code while running.

Here are the most common data types you'll use in Python:

* Integer: A whole number without decimals, for example, `10` or `-5`.

```python
my_integer_var = 10
print('Integer:', my_integer_var) # Integer: 10
```

* Float: A number with a decimal point, like `4.41` or `-0.4`.

```python
my_float_var = 4.50
print('Float:', my_float_var) # Float: 4.5
```

* String: A sequence of characters enclosed in single or double quotation marks like `'Hello world!'`.

```python
my_string_var = 'hello'
print('String:', my_string_var) # String: hello
```

* Boolean: A true or false type, written as `True` or `False`.

```python
my_boolean_var = True
print('Boolean:', my_boolean_var) # Boolean: True
```

* Set: An unordered collection of unique elements, like `{0.5, 4, 'apple'}`.

```python
my_set_var = {7, 'hello', 8.5}
print('Set:', my_set_var) # Set: {7, 'hello', 8.5}
```

* Dictionary: A collection of key-value pairs enclosed in curly braces, like `{'name': 'John Doe', 'age': 28}`.

```python
my_dictionary_var = {'name': 'Alice', 'age': 25}
print('Dictionary:', my_dictionary_var) # Dictionary: {'name': 'Alice', 'age': 25}
```

* Tuple: An immutable ordered collection, enclosed in parentheses, like `('apple', 4.5, 7)`.

```python
my_tuple_var = (7, 'hello', 8.5)
print('Tuple:', my_tuple_var) # Tuple: (7, 'hello', 8.5)
```

* Range: A sequence of numbers, often used in loops, for example, `range(5)`.

```python
my_range_var = range(5)
print('Range:', my_range_var) # Range: range(0, 5)
```

* List: An ordered collection of elements that supports different data types.

```python
my_list = [22, 'Hello world', 3.14, True]
print(my_list) # [22, 'Hello world', 3.14, True]
```

* None: A special value that represents the absence of a value.

```python
my_none_var = None
print('None:', my_none_var) # None: None
```

In future lessons, you will learn more about how to work with all of these data types.

---

# How Do the type() and isinstance() Functions Work?

In the prior lesson, you learned about common data types in Python including the string, integer, and float types. As you build out your programs, you will need to learn how to view the type for a variable.

Here is an example variable:

```python
developer = 'Devin'
```

To see what type `developer` is, you can use the `type()` function like this:

```python
developer = 'Devin'

print(type(developer)) # <class 'str'>
```

The output of `<class 'str'>` means that `developer` is a string type.

If you fail to provide any arguments to the `type()` function, then you will receive the following error message:

```python
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: type() takes 1 or 3 arguments
```

Here are all of the data types you have learned so far along with their types in the terminal:

```python
my_integer_var = 10
print(type(my_integer_var))  # <class 'int'>

my_float_var = 4.50
print(type(my_float_var))  # <class 'float'>

my_string_var = 'hello'
print(type(my_string_var))  # <class 'str'>

my_boolean_var = True
print(type(my_boolean_var))  # <class 'bool'>

my_set_var = {7, 'hello', 8.5}
print(type(my_set_var))  # <class 'set'>

my_dictionary_var = {'name': 'Alice', 'age': 25}
print(type(my_dictionary_var))  # <class 'dict'>

my_tuple_var = (7, 'hello', 8.5)
print(type(my_tuple_var))  # <class 'tuple'>

my_range_var = range(5)
print(type(my_range_var))  # <class 'range'>

my_list = [22, 'Hello world', 3.14, True]
print(type(my_list)) # <class 'list'>

my_none_var = None
print(type(my_none_var))  # <class 'NoneType'>
```

There will be times in your program where you will need to verify that a particular variable is a specific type before performing operations on it. This is where the `isinstance()` function comes in handy.

Here is an example variable with a string assigned to it:

```python
account_balance = '12'
```

If you try to do mathematical expressions like division using the `account_balance` variable, then you will receive an error message.

```python
account_balance = '12'

account_balance / 2

# Traceback (most recent call last):
#   File "<stdin>", line 1, in <module>
# TypeError: unsupported operand type(s) for /: 'str' and 'int'
```

To see if `account_balance` is an integer, you can check using the `isinstance()` function like this:

```python
account_balance = '12'

isinstance(account_balance, int) # False
```

The built-in `isinstance()` function lets you check if a variable matches a specific data type. It takes in an object and the type you want to check it against, then returns a boolean. In this case, since `account_balance` is a string, it will return `False`.

The `isinstance()` function also allows you to check for multiple types at once.

Here is an example checking if `account_balance` is an `int` or `float`:

```python
account_balance = 12
isinstance(account_balance, (int, float)) # True
```

In this example, `account_balance` is an integer so `isinstance()` returns `True`. If `account_balance` were `12.0`, `isinstance()` would still return `True` because you are checking for integers or floats.

In future workshops and labs, you will use the `type()` and `isinstance()` functions to ensure your variables contain the correct data types before performing operations on them.

---

# How Do You Work With Integers and Floating Point Numbers?

Integers and floats are the primary numeric data types in Python. With them, you can store numeric data and perform mathematical operations.

Let's look at what integers and floats are, how to perform arithmetic calculations with them, and at several methods Python provides for working with both.

Integers are whole numbers without decimal points, either positive or negative:

```python
my_int_1 = 56
my_int_2 = -4

print(type(my_int_1)) # <class 'int'>
print(type(my_int_2)) # <class 'int'>
```

Here's how to perform an addition operation with integers:

```python
my_int_1 = 56
my_int_2 = 12

sum_ints = my_int_1 + my_int_2
print('Integer Addition:', sum_ints) # Integer Addition: 68
```

Here's how to perform a subtraction with integers:

```python
my_int_1 = 56
my_int_2 = 12

# Subtraction
diff_ints = my_int_1 - my_int_2
print('Integer Subtraction:', diff_ints) # Integer Subtraction: 44
```

Here's how to perform a multiplication operation with integers:

```python
my_int_1 = 12
my_int_2 = 4

# Multiplication
product_ints = my_int_1 * my_int_2
print('Integer Multiplication:', product_ints) # Integer Multiplication: 48
```

And here's how to perform a division operation with integers:

```python
my_int_1 = 56
my_int_2 = 12

# Division
div_ints = my_int_1 / my_int_2
print('Division:', div_ints) # Division: 4.666666666666667
```

Floats are positive or negative numbers with decimal points, like `3.14`, `-0.5`, or `0.0`.

```python
my_float_1 = -12.0
my_float_2 = 4.9

print(type(my_float_1)) # <class 'float'>
print(type(my_float_2)) # <class 'float'>
```

Here's an addition operation with floats:

```python
my_float_1 = 5.4
my_float_2 = 12.0

float_addition = my_float_1 + my_float_2
print('Float Addition:', float_addition) # Float Addition: 17.4
```

Here's a subtraction operation with floats:

```python
my_float_1 = 5.4
my_float_2 = 12.0

float_subtraction = my_float_2 - my_float_1
print('Float Subtraction:', float_subtraction) # Float Subtraction: 6.6
```

Here's a multiplication operation with floats:

```python
my_float_1 = 5.4
my_float_2 = 12.0

float_multiplication = my_float_2 * my_float_1
print('Float Multiplication:', float_multiplication) # Float Multiplication: 64.80000000000001
```

And here's a division operation with floats:

```python
my_float_1 = 5.4
my_float_2 = 12.0

float_division = my_float_2 / my_float_1
print('Float Division:', float_division) # Float Division: 2.222222222222222
```

If you add an integer and a float, the result is automatically converted to a float:

```python
my_int = 56
my_float = 5.4

sum_int_and_float = my_int + my_float

print(sum_int_and_float) # 61.4
print(type(sum_int_and_float)) # <class 'float'>
```

This is true for other basic arithmetic operations, too, like subtraction, multiplication, and division. If you mix integers and floats, Python will return a float as the result.

You can also perform more complex arithmetic calculations such as getting the remainder of two numbers with the modulo operator, floor division, and exponentiation with both integers and floats.

The modulo operator (`%`) returns the remainder when the value on the left is divided by the value on the right:

```python
my_int_1 = 56
my_int_2 = 12

my_float_1 = 5.4
my_float_2 = 12.0

mod_ints = my_int_1 % my_int_2
mod_floats = my_float_2 % my_float_1

print('Integer Modulo:', mod_ints) # Integer Modulo: 8
print('Float Modulo:', mod_floats) # Float Modulo: 1.1999999999999993
```

Floor division divides two numbers and returns the greatest integer less than or equal to the result. This is done with the double forward slash operator (`//`):

```python
my_int_1 = 56
my_int_2 = 12

my_float_1 = 5.4
my_float_2 = 12.0

floor_div_ints = my_int_1 // my_int_2
floor_div_floats = my_float_2 // my_float_1

print('Integer Floor Division:', floor_div_ints) # Integer Floor Division: 4
print('Float Floor Division:', floor_div_floats) # Float Floor Division: 2.0
```

Exponentiation raises a number to the power of another, and is done with the double asterisk operator (`**`):

```python
my_int_1 = 56
my_int_2 = 12

my_float_1 = 5.4
my_float_2 = 12.0

exp_ints = my_int_1 ** my_int_2
exp_floats = my_float_1 ** my_float_2

print('Integer Exponentiation:', exp_ints) # Integer Exponentiation: 951166013805414055936
print('Float Exponentiation:',  exp_floats) # Float Exponentiation: 614787626.1765089
```

Sometimes, you might notice that the result of an operation involving floats has more decimal digits than expected. For example, the sum `0.1 + 0.2` equals `0.30000000000000004` instead of `0.3`.

This happens because numbers are stored in binary format, and some fractions cannot be represented exactly in binary. As a result, they are stored as finite approximations, in the same way the fraction `1/3` cannot be represented with a finite number of digits in decimal and is truncated after a certain number of its infinite digits (`0.33333...`).

This leads to small rounding errors.

Python also provides built-in functions for converting either numeric data or strings into integers or floats.

The `float()` function returns a floating-point number constructed from the given number:

```python
my_int_1 = 56
my_float_1 = float(my_int_1)

print(my_float_1)  # 56.0
print(type(my_float_1))  # <class 'float'>
```

The `int()` function returns an integer constructed from the given number:

```python
my_float = 12.92563
my_int = int(my_float)

print(my_int)  # 12
print(type(my_int))  # <class 'int'>
```

Also, you can use the same built-in functions to convert a string into either a float or integer:

```python
my_str_int = '45'
my_str_float = '7.8'

converted_int = int(my_str_int)
converted_float = float(my_str_float)

print(converted_int, type(converted_int))  # 45 <class 'int'>
print(converted_float, type(converted_float))  # 7.8 <class 'float'>
```

Here are some other methods Python provides for working with integers and floats.

* `round()`: Rounds a number to the specified number of decimal places. By default this function rounds to the nearest integer, and returns a whole number with no decimal places:

```python
my_int_1 = 4.798
my_int_2 = 4.253

rounded_int_1 = round(my_int_1)
rounded_int_2 = round(my_int_2, 1)

print(rounded_int_1) # 5
print(rounded_int_2) # 4.3
```

* `abs()`: returns the absolute value of a number,

```python
num = -15

absolute_value = abs(num)
print(absolute_value) # 15
```

* `pow()`: raises a number to the power of another or performs modular exponentiation.

```python
result_1 = pow(2, 3)  # Equivalent to 2 ** 3
print(result_1)  # 8

result_2 = pow(2, 3, 5)  # (2 ** 3) % 5
print(result_2)  # 3
```

---

# How Do Augmented Assignments Work?

Augmented assignment combines a binary operation with an assignment in one step. It takes a variable, applies an operation to it with another value, and stores the result back into the same variable.

If you're familiar with a language like JavaScript, you've probably heard of the addition assignment operator (`+=`) or subtraction assignment (`-=`), and others. Those exist in Python, too. The only difference is that they're referred to as **augmented assignments**.

The basic syntax of an augmented assignment looks like this:

```python
variable <operator>= value
```

Which is a more efficient way of doing this:

```python
variable = variable <operator> value
```

For example, here's an example of using augmented assignment to add `5` to an existing variable:

```python
my_var = 10
my_var += 5

print(my_var) # 15
```

And here is the same thing, but without augmented assignment:

```python
my_var = 10
my_var = my_var + 5

print(my_var) # 15
```

The advantage of augmented assignment is that it provides a concise and readable way to update a variable value without repeating the variable name. In turn, this reduces redundancy and potential errors that might arise from a typo or something similar.

Every operator can use an augmented assignment. We've looked at the addition assignment operator (`+=`), so let's look at others.

* The subtraction assignment operator (`-=`) subtracts the right operand from the left variable and stores the difference in the left variable:

```python
count = 14
count -= 3

print(count) # 11
```

* The multiplication assignment operator (`*=`) multiplies the left variable by the right operand and stores the product back in the left variable:

```python
product = 65
product *= 7

print(product) # 455
```

* The division assignment operator (`/=`) divides the left variable by the right and stores the result back in the left variable:

```python
price = 100
price /= 4

print(price) # 25.0
```

* The floor division operator (`//=`) floor‑divides the left variable by the right and stores the result back in the left variable:

```python
total_pages = 23
total_pages //= 5

print(total_pages) # 4
```

* The modulo assignment operator (`%=`) computes the remainder of the left variable divided by the right and stores it back in the left variable:

```python
bits = 35
bits %= 2

print(bits) # 1
```

* The exponentiation assignment operator (`**=`) raises the left variable to the power of the right and stores the result back in the left variable:

```python
power = 2
power **= 3

print(power) # 8
```

You can use some augmented assignment operators with strings, too. For example, the addition assignment operator makes it easy to concatenate strings:

```python
greet = 'Hello'
greet += ' World'

print(greet) # Hello World
```

And the multiplication assignment operator can be used to repeat a string:

```python
greet = 'Hello'
greet *= 3

print(greet) # HelloHelloHello
```

Other augmented assignments throw a `TypeError` when you use them with strings:

```python
greet = 'Hello'
greet -= ' World'

print(greet) # TypeError: unsupported operand type(s) for -=: 'str' and 'str'


greet = 'Hello'
greet /= 'World'

print(greet) # TypeError: unsupported operand type(s) for /=: 'str' and 'str' 
```

If you're wondering if increment and decrement operators (`++` and  `--`) work in Python, they don't. That's because Python deliberately avoids C-style increment and decrement shortcuts in order to keep the language clear and explicit.

Instead of `x++`, you can simply write `x += 1`, which makes it obvious that you're incrementing the value of `x` by `1`.

Writing `++x` in Python just applies the unary plus twice, and does not increment anything:

```python
my_var = 5

print(+my_var)   # 5
print(++my_var)  # 5
print(+++my_var) # 5

my_var += 1

print(my_var) # 6
```

---

## Module Review Component

# Python Basics Review

What is Python?
---------------

* **Introduction**: Python is a general-purpose programming language known for its simplicity and ease of use. Python is used in many fields like data science and machine learning, web development, scripting and automation, embedded systems and IoT, and much more.
* **Common Use Cases**: Python is used in data science, machine learning, web development, cybersecurity, automation and microcomputers like the Raspberry Pi and MicroPython-compatible boards.

Variables
---------

* **Declaring Variables**: To declare a variable, you start with the variable name followed by the assignment operator (`=`) and then the value. This can be a number, string, boolean, etc. Here are some examples:

```python
name = 'John Doe'
age = 25
```

* **Naming Conventions for Variables**: Here are the naming conventions you should use for variables:

  + Variable names can only start with a letter or an underscore (\_), not a number.
  + Variable names can only contain alphanumeric characters (a-z, A-Z, 0-9) and underscores (\_).
  + Variable names are case-sensitive — `age`, `Age`, and `AGE` are all considered unique.
  + Variable names cannot be one of Python’s reserved keywords such as `if`, `class`, or `def`.
  + Variables names with multiple words are separated by underscores. Ex. `snake_case`.

Comments
--------

* **Single Line Comments**: These types of comments should be used for short notes you wish to leave in your code.

```python
# This is a single line comment
```

* **Multi-line Strings**: These types of strings can be used to leave larger notes or to comment out sections of code.

```python
"""
This is a multi-line string.
Here is some code commented out.

name = 'John Doe'
age = 25
"""
```

* **`print()` Function**: To print data to the console, you can use the `print()` function like this:

```python
print('Hello world!') # Hello world!
```

Common Data Types in Python
---------------------------

* **Introduction**: Python is a dynamically-typed language like JavaScript, meaning you don't need to explicitly declare types for variables. The language knows what the type of a variable is based on what you assign to the variable.
* **Integer**: A whole number without decimals:

```python
my_integer_var = 10
print('Integer:', my_integer_var) # Integer: 10
```

* **Float**: A number with decimals:

```python
my_float_var = 4.50
print('Float:', my_float_var) # Float: 4.5
```

* **String**: A sequence of characters wrapped in quotes:

```python
my_string_var = 'hello'
print('String:', my_string_var) # String: hello
```

* **Boolean**: A value representing either `True` or `False`:

```python
my_boolean_var = True
print('Boolean:', my_boolean_var) # Boolean: True
```

* **Set**: An unordered collection of unique elements:

```python
my_set_var = {7, 5, 8}
print('Set:', my_set_var) # Set: {7, 5, 8}
```

* **Dictionary**: A collection of key-value pairs, enclosed in curly braces:

```python
my_dictionary_var = {"name": "Alice", "age": 25}
print('Dictionary:', my_dictionary_var) # Dictionary: {'name': 'Alice', 'age': 25}
```

* **Tuple**: An immutable ordered collection, enclosed in parentheses:

```python
my_tuple_var = (7, 5, 8)
print('Tuple:', my_tuple_var) # Tuple: (7, 5, 8)
```

* **Range**: A sequence of numbers, often used in loops:

```python
my_range_var = range(5)
print(my_range_var) # range(0, 5)
```

* **List**: An ordered collection of elements that supports different data types:

```python
my_list = [22, 'Hello world', 3.14, True]
print(my_list) # [22, 'Hello world', 3.14, True]
```

* **None**: A special value that represents the absence of a value:

```python
my_none_var = None
print('None:', my_none_var) # None: None
```

Immutable and Mutable Types
---------------------------

* **Immutable Types**: These types cannot change once declared, although you can point their variables at something new, which is called reassignment. They include integer, float, complex, boolean, string, tuple, range, and `None`.
* **Mutable Types**: These types can change once declared. You can add, remove, or update their items. They include collection types such as list, set, and dictionary.
* **`type()` Function**: To see the type for a variable, you can use the `type()` function like this:

```python
greeting = 'Hello there!'
age = 21

print(type(greeting)) # <class 'str'>
print(type(age)) # <class 'int'>
```

* **`isinstance()` Function**: This is used to check if a variable matches a specific data type:

```python
greeting = 'Hello world'
name = 'John Doe'

print(isinstance(greeting, str)) # True
print(isinstance(name, int)) # False
```

Working with Strings
--------------------

* **Definition**: As you recall from JavaScript, strings are immutable which means you can not change them after they have been created. In Python, you can use either single or double quotes. It is recommended to choose a rule and stick with it:

```python
developer = 'Jessica'
city = "Los Angeles"
```

* **Accessing Characters from Strings**: You can access characters from strings by using bracket notation like this:

```python
my_str = 'Hello world'

print(my_str[0])  # H
print(my_str[6])  # w

print(my_str[-1])  # d
print(my_str[-2]) # l
```

* **Escaping Strings**: You can use a backslash (`\`) if your string contains quotes like this:

```python
msg = 'It\'s a sunny day'
quote = "She said, \"Hello!\""
```

* **String Concatenation**: To concatenate strings, you can use the `+` operator like this:

```python
developer = 'Jessica'
print('My name is ' + developer + '.') # My name is Jessica.
```

Another way to concatenate strings is by using the `+=` operator. This is used to perform concatenation and assignment in the same step like this:

```python
greeting = 'My name is '
developer = 'Jessica.'

greeting += developer
print(greeting) # My name is Jessica.
```

* **`f-strings`**: This is short for formatted string literals. It allows you to handle interpolation and also do some concatenation with a compact and readable syntax:

```python
developer = 'Jessica'
greeting = f'My name is {developer}.'
print(greeting) # My name is Jessica.
```

* **String Slicing**: This is when you can extract portions of a string. Here is the basic syntax:

```python
str[start:stop:step]
```

The start position represents the index where the extraction should begin. The stop position is where the slice should end. This position is non inclusive. The step position represents the interval to increment for the slicing. Here are some examples:

```python
message = 'Python is fun!'

print(message[0:6])  # Python
print(message[7:])  # is fun!
print(message[::2])  # Pto sfn
```

* **Getting the Length of a String**: The `len()` function is used to return the number of the characters in the string:

```python
developer = 'Jessica'

print(len(developer)) # 7
```

Working with the `in` operator
------------------------------

* **`in` Operator**: This returns a boolean that specifies whether the character or characters exist in the string or not:

```python
my_str = 'Hello world'

print('Hello' in my_str)  # True
print('hey' in my_str)    # False
print('hi' in my_str)    # False
print('e' in my_str)  # True
print('f' in my_str)  # False
```

Common String Methods
---------------------

* **`str.upper()`**: This returns a new string with all characters converted to uppercase:

```python
developer = 'Jessica'

print(developer.upper()) # JESSICA
```

* **`str.lower()`**: This returns a new string with all characters converted to lowercase:

```python
developer = 'Jessica'

print(developer.lower()) # jessica
```

* **`str.strip()`**: This returns a copy of the string with specified leading and trailing characters removed (if no argument is passed to the method, it removes leading and trailing whitespace).

```python
greeting = '  hello world  '

trimmed_my_str = greeting.strip()
print(trimmed_my_str)  # 'hello world'
```

* **`replace()`**: This returns a new string with all occurrences of the old string replaced by a new one.

```python
greeting = 'hello world'

replaced_my_str = greeting.replace('hello', 'hi')
print(replaced_my_str)  # 'hi world'
```

* **`split()`**: This is used to split a string into a list using a specified separator. A separator is a string specifying where the split should happen.

```python
dashed_name = 'example-dashed-name'

split_words = dashed_name.split('-')
print(split_words)  # ['example', 'dashed', 'name']
```

* **`join()`**: This is used to join elements of an iterable into a string with a separator. An iterable is a collection of elements that can be looped over like a list, string or a tuple.

```python
example_list = ['example', 'dashed', 'name']

joined_str = ' '.join(example_list)
print(joined_str)  # example dashed name
```

* **`str.startswith(prefix)`**: This returns a boolean indicating if a string starts with the specified prefix:

```python
developer = 'Naomi'

result = developer.startswith('N')
print(result)  # True
```

* **`str.endswith(suffix)`**: This returns a boolean indicating if a string ends with the specified suffix:

```python
developer = 'Naomi'

result = developer.endswith('N')
print(result)  # False
```

* **`str.find()`**: This returns the index for the first occurrence of a substring. If one is not found, then `-1` is returned:

```python
developer = 'Naomi'

result = developer.find('N')
print(result)  # 0

city = 'Los Angeles'
print(city.find('New')) # -1
```

* **`str.count(substring)`**: This counts how many times a substring appears in a string:

```python
city = 'Los Angeles'
print(city.count('e')) # 2
```

* **`str.capitalize()`**: This returns a new string with the first character capitalized and the other characters lowercased:

```python
dessert = 'chocolate cake'
print(dessert.capitalize()) # Chocolate cake
```

* **`str.isupper()`**: This returns `True` if all letters in the string are uppercase and `False` if otherwise:

```python
dessert = 'chocolate cake'
print(dessert.isupper()) # False
```

* **`str.islower()`**: This returns `True` if all letters in the string are lowercase and `False` if otherwise:

```python
dessert = 'chocolate cake'
print(dessert.islower()) # True
```

* **`str.title()`**: This returns a new string with the first letter of each word capitalized:

```python
city = 'los angeles'
print(city.title()) # Los Angeles
```

* **`str.maketrans()`**: This method is used to create a table of 1 to 1 character mappings for translation. It is often used with the `translate()` method which applies that table to a string and return the translated result.

```python
trans_table = str.maketrans('abc', '123')
print(trans_table) # {97: 49, 98: 50, 99: 51}

result = 'abcabc'.translate(trans_table)
print(result)  # 123123
```

Common Operations used with Integers and Floats
-----------------------------------------------

* **Basic Math Operations**: In Python, you can do basic math operations with integers and floats including addition, subtraction, multiplication and division:

```python
int_1 = 56
int_2 = 12
float_1 = 5.4
float_2 = 12.0

# Addition

print('Integer Addition:', int_1 + int_2) # Integer Addition: 68
print('Float Addition:', float_1 + float_2) # Float Addition: 17.4

# Subtraction

print('Int Subtraction:', int_1 - int_2) # Int Subtraction: 44
print('Float Subtraction:',  float_2 - float_1) # Float Subtraction: 6.6

# Multiplication

print('Int Multiplication:', int_1 * int_2) # Int Multiplication: 672
print('Float Multiplication:', float_2 * float_1) # Float Multiplication: 64.80000000000001

# Division

print('Division:', int_1 / int_2) # Division: 4.666666666666667
print('Float Division:', float_2 / float_1) # Float Division: 2.222222222222222
```

When you add a float and an integer, the result will be converted to a float like this:

```python
int_1 = 56
float_1 = 5.4

print(int_1 + float_1) # 61.4
```

* **Modulo Operator (`%`)**: This returns the remainder when a number is divided by another number:

```python
int_1 = 56
int_2 = 12

print(int_1 % int_2) # 8
```

* **Floor Division (`//`)**: This operator is used to divide two numbers and round down the result to the nearest whole number:

```python
int_1 = 56
int_2 = 12

print(int_1 // int_2) # 4
```

* **Exponentiation Operator (`**`)**: This operator is used to raise a number to the power of another:

```python
int_1 = 4
int_2 = 2

print(int_1 ** int_2) # 16
```

* **`float()` Function**: You can use this function to convert an integer to float.

```python
num = 4

print(float(num)) # 4.0
```

* **`int()` Function**: You can use this function to convert an float to an integer.

```python
num = 4.0

print(int(num)) # 4
```

* **`round()` Function**: This is used to round a number to the nearest whole integer:

```python
num_1 = 3.4
num_2 = 7.7

print(round(num_1)) # 3
print(round(num_2)) # 8
```

* **`abs()` Function**: This is used to return the absolute value of a number:

```python
num = -13

print(abs(num)) # 13
```

* **`pow()` Function**: This is used to raise a number to the power of another:

```python
result = pow(2, 3) 
print(result)  # 8
```

Augmented Assignments
---------------------

* **Definition**: Augmented assignment combines a binary operation with an assignment in one step. It takes a variable, applies an operation to it with another value, and stores the result back into the same variable.

```python
# Addition assignment 
my_var = 10
my_var += 5

print(my_var) # 15

# Subtraction assignment
count = 14
count -= 3

print(count) # 11

# Multiplication assignment 
product = 65
product *= 7

print(product) # 455

# Division assignment 
price = 100
price /= 4

print(price) # 25.0

# Floor Division assignment 
total_pages = 23
total_pages //= 5

print(total_pages) # 4

# Modulo assignment 
bits = 35
bits %= 2

print(bits) # 1

# Exponentiation assignment 
power = 2
power **= 3

print(power) # 8
```

There are other augmented assignment operators too, like those for bitwise operators. They include `&=`, `^=`, `>>=`, and `<<=`.

Working with Functions
----------------------

* **Definition**: Functions are reusable pieces of code that take inputs (arguments) and returns an output. To call a function, you need to reference the function name followed by a set of parenthesis:

```python
# Defining a function

def get_sum(num_1, num_2):
    return num_1 + num_2

result = get_sum(3, 4) # function call
print(result) # 7
```

If a function does not explicitly return a value, then the default return value is `None`:

```python
def greet():
    print('hello') 

result = greet() # hello
print(result) # None
```

You can also supply default values to parameters like this:

```python
def get_sum(num_1, num_2=2):
    return num_1 + num_2

result = get_sum(3) 
print(result) # 5
```

If you call the function without the correct number of arguments, you will get a `TypeError`:

```python
def calculate_sum(a, b):
    print(a + b)

calculate_sum()

# TypeError: calculate_sum() missing 2 required positional arguments: 'a' and 'b'
```

Common Built-in Functions
-------------------------

* **`input()` Function**: This is used to prompt the user for some input:

```python
name = input('What is your name?') # User types 'Kolade' and presses Enter  
print('Hello', name) # Hello Kolade
```

* **`int()` Function**: This is used to convert a number, boolean, or a numeric string into an integer:

```python
print(int(3.14)) # 3
print(int('42')) # 42
print(int(True)) # 1
print(int(False)) # 0
```

Scope in Python
---------------

* **Local Scope**: This is when a variable declared inside a function or class can only be accessed within that function or class.

```python
def my_func():
    num = 10
    print(num)
```

* **Enclosing Scope**: This is when a function that's nested inside another function can access the variables of the function it's nested within.

```python
def outer_func():
    msg = 'Hello there!'
    
    def inner_func():
        print(msg)
    inner_func()

print(outer_func()) # Hello there!
```

* **Global Scope**: This refers to variables that are declared outside any functions or classes which can be accessed from anywhere in the program.

```python
tax = 0.70 

def get_total(subtotal):
    total = subtotal + (subtotal * tax)
    return total

print(get_total(100))  # 170.0
```

* **Built-in Scope**: Reserved names in Python for predefined functions, modules, keywords, and objects.

```python
print(str(45)) # '45'
print(type(3.14)) # <class 'float'>
print(isinstance(3, str)) # False
```

Comparison Operators
--------------------

* **Equal (`==`)**: Checks if two values are equal:

```python
print(3 == 4) # False
```

* **Not equal (`!=`)**: Checks if two values are not equal:

```python
print(3 != 4) # True
```

* **Strictly greater than (`>`)**: Checks if one value is greater than another:

```python
print(3 > 4) # False
```

* **Strictly less than (`<`)**: Checks if one value is less than another:

```python
print(3 < 4) # True
```

* **Greater than or equal(`>=`)**: Checks if one value is greater than or equal to another:

```python
print(3 >= 4) # False
```

* **Less than or equal(`<=`)**: Checks if one value is less than or equal to another:

```python
print(3 <= 4) # True
```

Working with `if`, `elif` and `else` Statements
-----------------------------------------------

* **`if` Statements**: These are conditions used to determine if something is true or not. If the condition evaluates to `True`, then that block of code will run.

```python
age = 18

if age >= 18:
    print('You are an adult') # You are an adult
```

* **`elif` Clause**: These are conditions that come after an `if` statement. An `elif` clause runs only if all previous conditions evaluate to `False` and its own condition evaluates to `True`.

```python
age = 16

if age >= 18:
    print('You are an adult')
elif age >= 13:
    print('You are a teenager')  # You are a teenager
```

* **`else` Clause**: This will run if no other conditions evaluate to `True`.

```python
age = 12

if age >= 18:
    print('You are an adult')
elif age >= 13:
    print('You are a teenager')
else:
    print('You are a child')  # You are a child
```

You can also use nested `if` statements like this:

```python
is_citizen = True
age = 25

if is_citizen:
    if age >= 18:
        print('You are eligible to vote') # You are eligible to vote
else:
    print('You are not eligible to vote')
```

Truthy and Falsy Values
-----------------------

* **Definition**: In Python, every value has an inherent boolean value, or a built-in sense of whether it should be treated as `True` or `False` in a logical context. Many values are considered truthy, that is, they evaluate to `True` in a logical context. Others are falsy, meaning they evaluate to `False`. Here are some examples of falsy values:

```python
None
False
Integer 0
Float 0.0
Empty strings ''
```

Other values like non-zero numbers, and non-empty strings are truthy.

Working with the `bool()` Function
----------------------------------

* **Definition**: If you want to check whether a value is truthy or falsy, you can use the built-in `bool()` function. It explicitly converts a value to its boolean equivalent and returns `True` for truthy values and `False` for falsy values. Here are a few examples:

```python
print(bool(False)) # False
print(bool(0))  # False
print(bool('')) # False

print(bool(True)) # True
print(bool(1)) # True
print(bool('Hello')) # True
```

Boolean Operators and Short-circuiting
--------------------------------------

* **Definition**: These are special operators that allow you to combine multiple expressions to create more complex decision-making logic in your code. There are three Boolean operators in Python: `and`, `or`, and `not`.
* **`and` Operator**: This operator takes two operands and returns the first operand if it is falsy, otherwise, it returns the second operand. Both operands must be truthy for an expression to result in a truthy value.

```python
is_citizen = True
age = 25

print(is_citizen and age) # 25
```

You can also use the `and` operator in conditionals like this:

```python
is_citizen = True
age = 25

if is_citizen and age >= 18:
    print('You are eligible to vote') # You are eligible to vote
else:
    print('You are not eligible to vote')
```

* **`or` Operator**: This operator returns the first operand if it is truthy, otherwise, it returns the second operand. An `or` expression results in a truthy value if at least one operand is truthy. Here is an example:

```python
age = 19
is_employed = False

print(age or is_employed) # 19
```

Just like with the `and` operator, you can use the `or` operator in conditionals like this:

```python
age = 19
is_student = True

if age < 18 or is_student:
    print('You are eligible for a student discount') # You are eligible for a student discount
else:
    print('You are not eligible for a student discount')
```

* **Short-circuiting**: The `and` and `or` operators are known as a short-circuit operators. Short-circuiting means Python checks values from left to right and stops as soon as it determines the final result.
* **`not` Operator**: This operator takes a single operand and inverts its boolean value. It converts truthy values to `False` and falsy values to `True`. Unlike the previous operators we looked at, `not` always returns `True` or `False`. Here are some examples:

```python
print(not '') # True, because empty string is falsy
print(not 'Hello') # False, because non-empty string is truthy
print(not 0) # True, because 0 is falsy
print(not 1) # False, because 1 is truthy
print(not False) # True, because False is falsy
print(not True) # False, because True is truthy
```

Here is an example of the `not` operator in a conditional:

```python
is_admin = False

if not is_admin:
    print('Access denied for non-administrators.') # Access denied for non-administrators.
else:
    print('Welcome, Administrator!')
```

---

# Module 3: Booleans, Conditionals, and Control Flow

# How Do Conditional Statements and Logical Operators Work?

Conditional statements, or conditionals, let you control the flow of your program based on whether certain conditions are true or false.

But before we get into all that, let's go over the basic building blocks of conditional statements, starting with comparison operators. Comparison operators are operators that let you compare two or more values, and return a boolean value.

In a previous lesson, you learned that booleans are one of the data types in Python, and can only be `True` or `False`.

Here's a table with the comparison operators in Python:

| Operator | Name | Description |
| --- | --- | --- |
| `==` | Equal | Checks if two values are equal |
| `!=` | Not equal | Checks if two values are not equal |
| `>` | Greater than | Checks if the value on the left is greater than the value on the right |
| `<` | Less than | Checks if the value on the left is less than the value on the right |
| `>=` | Greater than or equal | Checks if the value on the left is greater than or equal to the value on the right |
| `<=` | Less than or equal | Checks if the value on the left is less than or equal to the value on the right |

Here are some of those expressions that evaluate to `True` or `False`:

```python
print(3 > 4) # False
print(3 < 4) # True
print(3 == 4) # False
print(4 == 4) # True
print(3 != 4) # True
print(3 >= 4) # False
print(3 <= 4) # True
```

These operators can be used in conditionals to compare values and run certain code based on whether the conditional evaluates to `True` or `False`.

In Python, the most basic conditional is the `if` statement. Here's the basic syntax:

```python
if condition:
    pass # Code to execute if condition is True
```

* `if` statements start with the `if` keyword.
* `condition` is an expression that evaluates to `True` or `False`, followed by a colon (`:`).
* The body of the `if` statement constitutes a code block, which is a group of statements that belong together. In Python, the level of indentation is what defines a code block.

In the example above, the body of the `if` statement contains a `pass` statement. When a `pass` statement is executed, nothing happens. This is a special keyword that can be used as a placeholder for future code and it is useful when empty code blocks are not allowed.

The code within the body of the `if` statement runs only when the condition evaluates to `True`. For example:

```python
age = 18

if age >= 18:
    print('You are an adult') # You are an adult
```

Notice the indentation before `print('You are an adult')`. While other programming languages use characters like curly braces to define code blocks, and just use indentation for readability, in Python, code blocks are determined by indentation.

The following code would raise an `IndentationError`, which is Python's way to signal that indentation is required at a certain point of the code:

```python
age = 18

if age >= 18:
print('You are an adult') # IndentationError: expected an indented block after 'if' statement on line 3
```

Though you can use any number of spaces (as long as you are consistent) to determine each level of indentation, the Python style guide recommends using four spaces.

Blocks are also found in loops and functions, which you'll learn about in future lessons.

Going back to our example, if `age` is anything less than `18`, nothing is printed in the terminal:

```python
age = 12

if age >= 18:
    print('You are an adult') # Nothing shows up in the terminal
```

But what if you also want to print something if `age` is less than `18`? That's where the `else` clause comes in. The `else` clause runs when the `if` condition is false. Here's the syntax for an `if…else` statement:

```python
if condition:
   pass # Code to execute if condition is True
else:
   pass # Code to execute if condition is False
```

For example:

```python
age = 12

if age >= 18:
    print('You are an adult')
else:
    print('You are not an adult yet') # You are not an adult yet
```

Note that you cannot place any statements between the `if` block and the `else` clause. The following code would raise a `SyntaxError`:

```python
age = 12

if age >= 18:
    print('You are an adult')
print('Almost there!')
else: # SyntaxError: invalid syntax
    print('You are not an adult yet')
```

There might be situations in which you want to account for multiple conditions. To do that, Python lets you extend your if statement with the `elif` (else if) keyword.

Here's the syntax:

```python
if condition1:
   pass # Code to execute if condition1 is True
elif condition2:
   pass # Code to execute if condition1 is False and condition2 is True
else:
   pass # Code to execute if all conditions are False
```

For example:

```python
age = 12

if age >= 18:
    print('You are an adult')
elif age >= 13:
    print('You are a teenager')
else:
    print('You are a child') # You are a child
```

Note that you can use as many `elif` clauses as you want:

```python
age = 2

if age >= 65:
    print('You are a senior citizen')
elif age >= 30:
    print('You are an adult in your prime')
elif age >= 18:
    print('You are a young adult')
elif age >= 13:
    print('You are a teenager')
elif age >= 3:
    print('You are a young child')
else:
    print('You are a toddler or an infant') # You are a toddler or an infant
```

Now that you understand how comparison operators and conditional statements work in Python, you can start writing programs that make decisions based on logic and input. Whether you’re comparing values or branching through multiple conditions, these tools are the foundation to writing flexible, responsive code.

---

# What Are Truthy and Falsy Values, and How Do Boolean Operators and Short-Circuiting Work?

In the previous lesson, you learned how to use comparison operators and conditional statements to control the flow of your programs.

While those are very powerful, you will often run into situations where you need to compare multiple values at once. This can lead to nested conditional statements, for example:

```python
is_citizen = True
age = 25

if is_citizen:
    if age >= 18:
        print('You are eligible to vote') # You are eligible to vote
else:
    print('You are not eligible to vote')
```

The above example will first check if `is_citizen` is `True`. If so, it will then go to the nested `if` statement and check if `age` is greater than or equal to `18`. Since `age` is greater than or equal to `18`, the message printed to the terminal will be `You are eligible to vote`. If `is_citizen` were `False`, then the message printed to the terminal would have been `You are not eligible to vote`.

If you are working with more complex conditional statements, then you can use Python’s `and`, `or`, and `not` operators.

But before we dive into those operators, let’s take a look at what truthy and falsy values are.

In Python, every value has an inherent boolean value, or a built-in sense of whether it should be treated as `True` or `False` in a logical context. Many values are considered **truthy**, that is, they evaluate to `True` in a logical context. Others are **falsy**, meaning they evaluate to `False`.

Here are a few falsy values:

* `None`
* `False`
* Integer `0`
* Float `0.0`
* Empty strings `""`

Other values like non-zero numbers, and non-empty strings are truthy.

If you want to check whether a value is truthy or falsy, you can use the built-in `bool()` function. It explicitly converts a value to its boolean equivalent and returns `True` for truthy values and `False` for falsy values. Here are a few examples:

```python
print(bool(False)) # False
print(bool(0))  # False
print(bool('')) # False

print(bool(True)) # True
print(bool(1)) # True
print(bool('Hello')) # True
```

Now that you understand truthy and falsy values, we can take a look at Boolean operators, which are also known as logical operators. These are special operators that allow you to combine multiple expressions to create more complex decision-making logic in your code.

There are three Boolean operators in Python: `and`, `or`, and `not`.

Let’s first take a look at the `and` operator.

The `and` operator takes two operands and returns the first operand if it is falsy, otherwise, it returns the second operand. Both operands must be truthy for an expression to result in a truthy value.

Here is an example:

```python
is_citizen = True
age = 25

print(is_citizen and age) # 25
```

In the above example, the number 25 is printed to the terminal because the `and` operator will evaluate the second operand if the first operand is `True`. The `and` operator is known as a short-circuit operator. Short-circuiting means Python checks values from left to right and stops as soon as it determines the final result.

You'll often use `and` within `if` statements to check if multiple conditions are met. Here’s how you can refactor the earlier example to use the `and` operator instead of nested `if` statements:

```python
is_citizen = True
age = 25

if is_citizen and age >= 18:
    print('You are eligible to vote') # You are eligible to vote
else:
    print('You are not eligible to vote')
```

In the example above, `is_citizen` is `True`, and `age >= 18` evaluates to `True`. Since both operands of the `and` operator are truthy, the condition `is_citizen and age >= 18` evaluates to `True`, and the `print` call in the `if` block is executed.

Now let's take a look at the `or` operator. This operator returns the first operand if it is truthy, otherwise, it returns the second operand. An `or` expression results in a truthy value if at least one operand is truthy. The `or` operator is also known as a short-circuit operator. Here is an example:

```python
age = 19
is_employed = False

print(age or is_employed) # 19
```

The following code will print the number 19 because the first operand `age` is truthy.

If you need to check if one or more expressions is `True`, then you can use the `or` operator in a conditional like this:

```python
age = 19
is_student = True

if age < 18 or is_student:
    print('You are eligible for a student discount') # You are eligible for a student discount
else:
    print('You are not eligible for a student discount')
```

In this case, `age < 18` is `False`, but `is_student` is `True`. Since at least one condition is true, the entire `or` expression evaluates to `True`, and the discount message in the `if` block is printed.

The last operator we will look at is the `not` operator which takes a single operand and inverts its boolean value. It converts truthy values to `False` and falsy values to `True`. Unlike the previous operators we looked at, `not` always returns `True` or `False`.

Here are a few examples:

```python
print(not '') # True, because empty string is falsy
print(not 'Hello') # False, because non-empty string is truthy
print(not 0) # True, because 0 is falsy
print(not 1) # False, because 1 is truthy
print(not False) # True, because False is falsy
print(not True) # False, because True is truthy
```

It is common to use the `not` operator in conditionals to check if something is not `True` or `False`, like this:

```python
is_admin = False

if not is_admin:
    print('Access denied for non-administrators.') # Access denied for non-administrators.
else:
    print('Welcome, Administrator!')
```

Since `is_admin` is `False`, then `not is_admin` is saying not `False` which is `True`. So the message `Access denied for non-administrators.` will be printed.

Now that you understand truthy and falsy values, the `and`, `or`, and `not` operators, and how short-circuiting works, you can write more flexible and readable conditional logic.

---

# Module 4: Strings

# What Are Strings and What Is String Immutability?

A string is a sequence of characters surrounded by either single or double quotation marks. In some programming languages, characters surrounded by single quotes are treated differently than characters surrounded by double quotes, but in Python, they're treated equally. So, you can use either when working with strings. Here are some examples of strings:

```python
my_str_1 = 'Hello'
my_str_2 = "World"
```

If you need a multi-line string, you can use triple double quotes or single quotes:

```python
my_str_3 = """Multiline
string"""
my_str_4 = '''Another
multiline
string'''
```

If your string contains either single or double quotation marks, then you have two options:

* Use the opposite kind of quotes. That is, if your string contains single quotes, use double quotes to wrap the string, and vice versa:

```python
msg = "It's a sunny day"
quote = 'She said, "Hello World!"'
```

* Escape the single or double quotation mark in the string with a backslash (`\`). With this method, you can use either single or double quotation marks to wrap the string itself:

```python
msg = 'It\'s a sunny day'
quote = "She said, \"Hello!\""
```

Sometimes, you may need to check if a string contains one or more characters. For that, Python provides the `in` operator, which returns a boolean that specifies whether the character or characters exist in the string or not.

Here are some examples:

```python
my_str = 'Hello world'

print('Hello' in my_str)  # True
print('hey' in my_str)    # False
print('hi' in my_str)    # False
print('e' in my_str)  # True
print('f' in my_str)  # False
```

Now, let's look at how you can get the length of a string and work with the individual characters in a string, a process called **indexing**. To get the length of a string, you can use the built-in `len()` function. Here's an example:

```python
my_str = 'Hello world'
print(len(my_str))  # 11
```

Each character in a string has a position called an index. The index is zero-based, meaning that the index of the first character of a string is `0`, the index of the second character is `1`, and so on. To access a character by its index, you use square brackets (`[]`) with the index of the character you want to access inside. Here are some examples:

```python
my_str = "Hello world"

print(my_str[0])  # H
print(my_str[6])  # w
```

Negative indexing is also allowed, so you can get the last character of any string with `-1`, the second-to-last character with `-2`, and so on:

```python
my_str = 'Hello world'
print(my_str[-1])  # d
print(my_str[-2]) # l
```

Many other programming languages group data types broadly as either primitive or reference types. Primitive types are simple and immutable, meaning they can't be changed once declared. Reference types can hold multiple values, and are either mutable or immutable. But Python doesn't draw a hard line between those two groups. Instead, all data gets treated as objects, and some objects are immutable while others are mutable.

Immutable data types can't be modified or altered once they're declared. You can point their variables at something new, which is called reassignment, but you can't change the original object itself by adding, removing, or replacing any of its elements.

Strings are immutable data types in Python. This means that you can reassign a different string to a variable:

```python
greeting = 'hi'
greeting = 'hello'
print(greeting) # hello
```

But direct modification of a string isn't allowed:

```python
greeting = 'hi'
greeting[0] = 'H' # TypeError: 'str' object does not support item assignment
```

Examples of other immutable data types in Python are integer, float, boolean, tuple, and range. You'll get to know each of these types in upcoming lessons.

---

# What Is String Slicing and How Does It Work?

In a previous lesson, you learned how each character in a string can be identified by its index (starting from zero), and accessed using the bracket notation:

```python
my_str = "Hello world"

print(my_str[0])  # H
print(my_str[6])  # w
print(my_str[-1]) # d
```

**String slicing** lets you extract a portion of a string or work with only a specific part of it. Here's the basic syntax:

```python
string[start:stop]
```

If you want to extract characters from a certain index to another, you just separate the `start` and `stop` indices with a colon:

```python
my_str = 'Hello world'
print(my_str[1:4]) # ell
```

Note that the `stop` index is non-inclusive, so `[1:4]` just extracted the characters from index `1`, and up to, but not including, the character at index `4`.

You can also omit the `start` and `stop` indices, and Python will default to `0` or the end of the string, respectively. For example, here's what happens if you omit the `start` index:

```python
my_str = 'Hello world'
print(my_str[:7])  # Hello w
```

This extracts everything from index `0` up to (but not including), the character at index `7`. And here's what happens if you omit the `stop` index:

```python
my_str = 'Hello world'
print(my_str[8:])  # rld
```

This extracts everything from the character at index `8` until the end of the string.

Note that slicing a string does not modify the original string:

```python
my_str = 'Hello world'
print(my_str[8:])  # rld
print(my_str)  # Hello world
```

You can also omit both the `start` and `stop` indices, which will extract the whole string:

```python
my_str = 'Hello world'
print(my_str[:])  # Hello world
```

Apart from the `start` and `stop` indices, there's also an optional `step` parameter, which is used to specify the increment between each index in the slice.

Here's the syntax for that:

```python
string[start:stop:step]
```

In the example below, the slicing starts at index `0`, stops before `11`, and extracts every second character:

```python
my_str = 'Hello world'
print(my_str[0:11:2])  # Hlowrd
```

A helpful trick you can do with the `step` parameter is to reverse a string by setting step to `-1`, and leaving `start` and `stop` blank:

```python
my_str = 'Hello world'
print(my_str[::-1]) # dlrow olleH
```

---

# What Are String Concatenation and String Interpolation?

When working with strings, combining different pieces of text together is a common operation you'll often find yourself dealing with.

In Python, you can combine multiple strings together with the plus (`+`) operator. This process is called **string concatenation**. Here's how to concatenate two strings with the plus operator:

```python
my_str_1 = 'Hello'
my_str_2 = "World"

str_plus_str = my_str_1 + ' ' + my_str_2
print(str_plus_str) # Hello World
```

But note that this only works with strings. If you try to concatenate a string with a number, you'll get a `TypeError`:

```python
name = 'John Doe'
age = 26

name_and_age = name + age
print(name_and_age) # TypeError: can only concatenate str (not "int") to str
```

This happens because Python does not automatically convert other data types like integers into strings when you concatenate them. Python requires all elements to be strings before it can concatenate them. To fix that, you can convert the number into a string with the built-in `str()` function, which returns the string representation of the given object without modifying the original object:

```python
name = 'John Doe'
age = 26

name_and_age = name + str(age)
print(name_and_age) # John Doe26
```

You can also use the augmented assignment operator for concatenation. This is represented by a plus and equals sign (`+=`), and performs both concatenation and assignment in one step. Here's it in action:

```python
name = 'John Doe'
age = 26

name_and_age = name  # Start with the name
name_and_age += str(age)  # Append the age as string

print(name_and_age)  # John Doe26
```

The process of inserting variables and expressions into a string is called **string interpolation**. Python has a category of string called **f-strings** (short for formatted string literals), which allows you to handle interpolation with a compact and readable syntax.

F-strings start with `f` (either lowercase or uppercase) before the quotes, and allow you to embed variables or expressions inside replacement fields indicated by curly braces (`{}`). Here's an example:

```python
name = 'John Doe'
age = 26
name_and_age = f'My name is {name} and I am {age} years old'
print(name_and_age) # My name is John Doe and I am 26 years old

num1 = 5
num2 = 10
print(f'The sum of {num1} and {num2} is {num1 + num2}') # The sum of 5 and 10 is 15
```

Note how you don't need to convert non-string types with the `str()` function. In the example above, the value of the `age`, `num1`, and `num2` variables is converted under the hood into a string during the interpolation process.

---

# What Are Some Common String Methods?

Python provides a number of built-in methods that make working with strings a breeze. They include, but are not limited to, the following:

* `upper()`: Returns a new string with all characters converted to uppercase.

```python
my_str = 'hello world'

uppercase_my_str = my_str.upper()
print(uppercase_my_str)  # HELLO WORLD
```

* `lower()`: Returns a new string with all characters converted to lowercase.

```python
my_str = 'Hello World'

lowercase_my_str = my_str.lower()
print(lowercase_my_str)  # hello world
```

* `strip()`: Returns a new string with the specified leading and trailing characters removed. If no argument is passed it removes leading and trailing whitespace.

```python
my_str = '  hello world  '

trimmed_my_str = my_str.strip()
print(trimmed_my_str)  # "hello world"
```

* `replace(old, new)`: Returns a new string with all occurrences of `old` replaced by `new`.

```python
my_str = 'hello world'

replaced_my_str = my_str.replace('hello', 'hi')
print(replaced_my_str)  # hi world
```

* `split(separator)`: Splits a string on a specified separator into a list of strings. If no separator is specified, it splits on whitespace.

```python
my_str = 'hello world'

split_words = my_str.split()
print(split_words)  # ['hello', 'world']
```

* `join(iterable)`: Joins elements of an iterable into a string with a separator.

```python
my_list = ['hello', 'world']

joined_my_str = ' '.join(my_list)
print(joined_my_str)  # hello world
```

* `startswith(prefix)`: Returns a boolean indicating if a string starts with the specified prefix.

```python
my_str = 'hello world'

starts_with_hello = my_str.startswith('hello')
print(starts_with_hello)  # True
```

* `endswith(suffix)`: Returns a boolean indicating if a string ends with the specified suffix.

```python
my_str = 'hello world'

ends_with_world = my_str.endswith('world')
print(ends_with_world)  # True
```

* `find(substring)`: Returns the index of the first occurrence of `substring`, or `-1` if it doesn't find one.

```python
my_str = 'hello world'

world_index = my_str.find('world')
print(world_index)  # 6
```

* `count(substring)`: Returns the number of times a substring appears in a string.

```python
my_str = 'hello world'

o_count = my_str.count('o')
print(o_count)  # 2
```

* `capitalize()`: Returns a new string with the first character capitalized and the other characters lowercased.

```python
my_str = 'hello world'

capitalized_my_str = my_str.capitalize()
print(capitalized_my_str)  # Hello world
```

* `isupper()`: Returns `True` if all letters in the string are uppercase and `False` if not.

```python
my_str = 'hello world'

is_all_upper = my_str.isupper()
print(is_all_upper)  # False
```

* `islower()`: Returns `True` if all letters in the string are lowercase and `False` if not.

```python
my_str = 'hello world'

is_all_lower = my_str.islower()
print(is_all_lower)  # True
```

* `title()`: Returns a new string with the first letter of each word capitalized.

```python
my_str = 'hello world'

title_case_my_str = my_str.title()
print(title_case_my_str)  # Hello World
```

---

# Module 5: Functions, Scope, and Modules

# How Do Functions Work in Python?

Functions are reusable pieces of code that run when you call them. Many programming languages come with built-in functions that make it easier to get started. Python is no exception, and we've already covered some built-in functions like `print()` in previous lessons.

Another helpful built-in function is `input()`, which lets you prompt the user for input:

```python
name = input('What is your name?') # User types "Kolade" and presses Enter  
print('Hello', name) # Output: Hello Kolade
```

On the other hand, `int()` converts a number, boolean, and a numeric string into an integer:

```python
print(int(3.14)) # 3
print(int('42')) # 42
print(int(True)) # 1
print(int(False)) # 0
```

You can also write your own custom functions. To do that, you use the `def` keyword, followed by the name you want to give your function, a pair of parentheses, and a colon. Then on a new line, you write the code your function should run. The code the function runs is also referred to as the function's body.

Here's an example of a custom function named `hello` that prints the string `Hello World` to the terminal:

```python
def hello():
    print('Hello World')
```

To run the function, you need to call it with its name followed by a pair of parentheses:

```python
hello() # Hello World
```

Notice the indentation before `print('Hello World')`. As you may recall from previous lessons, Python relies on indentation to determine which groups of statements belong together. These groups of statements are called code blocks.

Here's another simple function that prints the sum of two numbers to the terminal:

```python
def calculate_sum(a, b):
    print(a + b)
```

You can see that our function, `calculate_sum`, has `a` and `b` in its parentheses, separated by a comma. Those are called parameters. Think of parameters as placeholder variables that act as "slots" for the values you pass into functions when you call them.

To use the parameters, you have to pass in "arguments". Arguments are the values you pass to a function when you call it.

Here's how to call the `calculate_sum` function to sum together the numbers `3` and `1`:

```python
calculate_sum(3, 1) # 4
```

If you call the function without the correct number of arguments, you'll get a `TypeError`:

```python
calculate_sum()

# TypeError: calculate_sum() missing 2 required positional arguments: 'a' and 'b'
```

Functions also use a special `return` keyword to exit the function and return a value. If you don't explicitly use `return`, Python will return `None` by default.

Here's an example:

```python
def calculate_sum(a, b):
    print(a + b)

my_sum = calculate_sum(3, 1) # 4
print(my_sum) # None
```

You can see that the `calculate_sum` function prints the sum of `a` and `b`, but it doesn't return anything explicitly. So when we assign its result to `my_sum`, the value is actually `None`. To fix that, you can use the `return` keyword to send back the result:

```python
def calculate_sum(a, b):
    return a + b

my_sum = calculate_sum(3, 1)
print(my_sum) # 4
```

Now, `calculate_sum` returns the sum of `a` and `b`, which gets stored in `my_sum`.

---

# What Is Scope in Python and How Does It Work?

In Python, scope determines the point at which you can access a variable. It's what controls the lifetime of a variable and how it is resolved in different parts of the code.

To correctly determine scope, Python follows the **LEGB** rule, which stands for the following:

* **Local scope (L)**: Variables defined in functions or classes.
* **Enclosing scope (E)**: Variables defined in enclosing or nested functions.
* **Global scope (G):** Variables defined at the top level of the module or file.
* **Built-in scope (B)**: Reserved names in Python for predefined functions, modules, keywords, and objects.

Python uses the LEGB rule to resolve the scope of the variables in your program. We'll dive into each of these rules so you get a better understanding of the process.

**Local scope** means that a variable declared inside a function or class can only be accessed within that function or class.

Here's an example:

```python
def my_func():
    my_var = 10
    print(my_var)
```

In this case, the `my_func` function has its own scope which cannot be accessed from outside the function. Calling `my_func` will output `10`, but printing `my_var` outside the function will lead to a `NameError`:

```python
def my_func():
    my_var = 10 # Locally scoped to my_func
    print(my_var)

my_func() # 10

print(my_var) # NameError: name 'my_var' is not defined
```

**Enclosing scope** means that a function that's nested inside another function can access the variables of the function it's nested within.

For example:

```python
def outer_func():
    msg = 'Hello there!'

    def inner_func():
        print(msg)

    inner_func()

outer_func() # Hello there!
```

In this example, the inner function, `inner_func`, can freely access the `msg` variable defined in the outer function, `outer_func`. However, note that outer functions cannot access variables defined within any nested functions:

```python
def outer_func():
    msg = 'Hello there!'
    print(res)

    def inner_func():
        res = 'How are you?'
        print(msg)

    inner_func()

outer_func() # NameError: name 'res' is not defined
```

That's because `res` is locally scoped to `inner_func`. Also, notice that `outer_func` tries to print `res` before `inner_func` is called.

One solution is to initialize `res` as an empty string in the enclosing scope, which is within `outer_func`. Then within `inner_func`, make `res` a non-local variable with the `nonlocal` keyword:

```python
def outer_func():
    msg = 'Hello there!'
    res = ""  # Declare res in the enclosing scope

    def inner_func():
        nonlocal res  # Allow modification of an enclosing variable
        res = 'How are you?'
        print(msg)  # Accessing msg from outer_func()

    inner_func()
    print(res)  # Now res is accessible and modified

outer_func()

# Output:
# Hello there!
# How are you?
```

**Global scope** refers to variables that are declared outside any functions or classes which can be accessed from anywhere in the program. Here, `my_var` can be accessed anywhere, even inside a function it's not defined in:

```python
my_var = 100

def show_var():
    print(my_var)

show_var() # 100
print(my_var) # 100
```

And if you want to make a locally scoped variable defined inside a function globally accessible, you can use the `global` keyword:

```python
my_var_1 = 7

def show_vars():
    global my_var_2
    my_var_2 = 10
    print(my_var_1)
    print(my_var_2)

show_vars() # 7 10

# my_var_2 is now a global variable and can be accessed anywhere in the program
print(my_var_2) # 10
```

You can also use the `global` keyword to modify a global variable:

```python
my_var = 10  # A global variable

def change_var():
    global my_var  # Allows modification of a global variable
    my_var = 20

change_var()

print(my_var)  # my_var is now modified globally to 20
```

Finally, **built-in scope** refers to all of Python's built-in functions, modules, and keywords, and are available anywhere in your program:

```python
print(str(45)) # '45'
print(type(3.14)) # <class 'float'>
print(isinstance(3, str)) # False
```

---

# What Are Lambda Functions and How Do They Work?

Throughout the previous lessons, you have been used to defining functions by using the `def` keyword like this:

```python
def square(num):
    return num ** 2

print(square(4)) # 16
```

But when it comes to working with high order functions like `map()` and `filter()`, you can use an anonymous inline function. This is where lambda functions come in.

Here's what the `square()` function looks like when refactored into a lambda function:

```python
lambda num: num ** 2
```

As mentioned earlier, lambda functions are anonymous, so this function no longer has the name `square` associated with it. Lambda functions are great when you need to use them in higher order functions like this:

```python
numbers = [1, 2, 3, 4, 5]

even_numbers = list(filter(lambda x: x % 2 == 0, numbers))
print(even_numbers)  # [2, 4]
```

In this example, we have a list of numbers and want to create a new list of even numbers. So we pass in a lambda function as one of the arguments to the `filter()` function to get a new list containing the numbers `2` and `4`.

When working with lambda functions it is important to be aware of best practices. For example, it is not a good practice to assign a lambda function to a variable like this:

```python
numbers = [1, 2, 3, 4, 5]

square = lambda x: x ** 2
squared_numbers = list(map(square, numbers))
print(squared_numbers) # [1, 4, 9, 16, 25]
```

This defeats the purpose of using anonymous functions. In this case, you should use a regular function, like this:

```python
numbers = [1, 2, 3, 4, 5]

def square(num):
    return num ** 2

squared_numbers = list(map(square, numbers))
print(squared_numbers) # [1, 4, 9, 16, 25]
```

Also, you should avoid creating lambda functions that are difficult to read or unnecessarily complicated, like this:

```python
result = (lambda x: (x**2 + 2*x - 1) if x > 0 else (x**3 - x + 4))(3)
print(result)  # 14
```

While this function runs fine and produces the correct result of `14`, it is not easy to read or look at. In this case, it would be better to create a separate function with an `if/else` statement, and then call that function:

```python
def calculate_expression(x):
    if x > 0:
        return x**2 + 2*x - 1
    else:
        return x**3 - x + 4

print(calculate_expression(3))  # 14
```

Both regular functions and lambda functions have their use cases in Python programs. If you are dealing with a single inline expressions, then you might consider using a lambda function. Otherwise, using a regular function would be the way to go.

---

# What Is the Python Standard Library, and How Do You Import a Module?

In software development, a library is like a toolbox for developers.

Instead of having to implement every single part of the code yourself from scratch, a library gives you pre-written and reusable code, like functions, classes, and data structures that you can use in your projects.

Python has an extensive standard library with many different built-in modules. They're all standardized, well-vetted solutions for many of the problems and tasks you'll face daily as a programmer, such as:

* Interacting with the operating system.
* Working with files.
* Networking.
* Working with date and time.
* Performing mathematical operations.
* Using regular expressions.
* Testing and debugging your code.
* And much more!

Some examples of popular built-in modules are `math`, `random`, `re` (short for "regular expressions"), and `datetime`.

The `math` module has helpful functions for performing more complex mathematical operations.

The `random` module is helpful for generating random numbers.

The `re` module is used for working with regular expressions.

And the `datetime` module is helpful for working with dates and times in Python.

But how can you access the variables, constants, functions, and classes defined in these built-in modules?

You use an import statement. These statements let you import modules into your Python script. Import statements are generally written at the top of the file. Also, you can customize them based on your needs. First, you use the `import` statement, followed by the name of the module:

```python
import module_name
```

Let's say that you want to import the `math` module. In that case, you would write this at the top of your file:

```python
import math
```

Then, if you need to call a function from that module in your Python script, you would use dot notation, with the name of the module followed by the name of the function:

```python
module_name.function_name()
```

For example, to get the square root of 36, you would write `math` followed by a dot and then `sqrt`, an abbreviation of square root, and within parentheses, you would pass any necessary arguments. In this case, we only need to pass in the number we want the square root of:

```python
math.sqrt(36)
```

This is the most basic version of an import statement, but there are other alternatives.

If you need to import the module with a different name (also known as an "alias"), you can use this syntax, with `as` followed by the alias at the end of the import statement:

```python
import module_name as module_alias
```

This is often used to shorten long module names, or to avoid naming conflicts.

For example, to refer to the `math` module as `m` in your code, you can assign an alias to it, like this:

```python
import math as m
```

Then, you can access the elements of the module using the alias:

```python
m.sqrt(36)
```

But sometimes you don't need to import everything from a module. Perhaps you only need one or two specific functions or classes. Python has exactly what you need in that case.

Now the import statement starts with `from`, followed by the name of the module, and then the `import` keyword followed by the name of the elements that you want to import:

```python
from module_name import name1, name2
```

Then, you can use these names without the module prefix in your Python script.

If you want to assign aliases to these names, you can do that by using the `as` keyword after each, followed by the alias you want to use:

```python
from module_name import name1 as alias1, name2 as alias2
```

Let's say that you only want to import the radians, sine, and cosine functions from the `math` module. You would write:

```python
from math import radians, sin, cos
```

Now you can call these functions directly in your code, without the `math` module as a prefix.

Here we have a more detailed example:

To find the sine and cosine of a specific angle initially expressed in degrees, we can call the `radians` function to convert it to radians, and then call the sine and cosine functions, passing the angle in radians:

```python
from math import radians, sin, cos

angle_degrees = 40
angle_radians = radians(angle_degrees)

sine_value = sin(angle_radians)
cos_value = cos(angle_radians)

print(sine_value) # 0.6427876096865393
print(cos_value)  # 0.766044443118978
```

Notice how we are calling the functions directly, without the name of the module as a prefix. This is because we imported the functions with this alternative syntax.

This is helpful, but it can result in naming conflicts if you already have functions or variables with the same name defined in the Python script itself. So that's something to keep in mind when choosing which type of import statement you want to use.

And finally, we find this import statement that ends with an asterisk. The asterisk is telling Python that you want to import everything in that module, but you want to import it so that you don't need to use the name of the module as a prefix:

```python
from module_name import *
```

For example, if you do this while importing the `math` module, you'll be able to call any function defined in that module without specifying the name of the module as a prefix. Here are some examples:

```python
from math import *
print(sqrt(36))  # 6.0
print(pow(5, 2)) # 25.0
print(exp(1))    # 2.718281828459045
```

However, this is generally discouraged because it can lead to namespace collisions, and make it harder to know where certain names are coming from.

Import statements work exactly the same for functions, classes, constants, variables, and any other elements defined in the module.

Here is an example of a constant from the `math` module, the number `pi`:

```python
import math
print(math.pi)
```

And here is an example of a class from the `datetime` module. We create a date object that represents July 15, 1959. Then, we assign that `date` object to a variable and access the day, month, and year individually using dot notation:

```python
import datetime
birthday = datetime.date(1959, 7, 15)
print(birthday.day)    # 15
print(birthday.month)  # 7
print(birthday.year)   # 1959
```

You can find more information about the content of the module in the official Python documentation for that module.

Great. Now that you know more about modules, you should also know about this very important idiom in Python scripts, because they are very closely related:

```python
if __name__ == '__main__': 
    # Code
```

`__name__` is a special built-in variable in Python.

When a Python file is executed directly, Python sets the value of this variable to the string `"__main__"`.

But if the Python file is imported as a module into another Python script, the value of the `__name__` variable is set to the name of that module (usually the filename without the `.py` extension).

This is why you'll often find this conditional in Python scripts. It contains the code that you want to run **only if** the Python script is running as the main program:

```python
if __name__ == '__main__': 
    # Code
```

But if the script is imported as a module, the code within that block doesn't run.

This is helpful because it allows Python scripts to have two purposes. They can be run directly to execute their main logic, or they can be imported into another module without executing their main logic.

---

# Module 6: Loops and Basic Sequences

# How Do Loops Work?

As you learned in earlier modules, loops are used to repeat a block of code for a set number of times. In this lesson you will learn how to work with different types of loops in Python.

The first loop we will go over is the `for` loop. Here is an example of using a `for` loop to iterate through a list and print each item to the console:

```python
programming_languages = ['Rust', 'Java', 'Python', 'C++']

for language in programming_languages:
    print(language)
```

The result would be:

```python
Rust
Java
Python
C++
```

Notice that the `print(language)` is indented inside of the loop. Without that indentation, you would get an `IndentationError`:

```python
"""
Traceback (most recent call last):
  File "<stdin>", line 4, in <module>
IndentationError: expected an indented block after 'for' statement on line 3
"""
```

You can also use a `for` loop to iterate through other iterables like a string. Here is an example of using a `for` loop to loop through the string `code` and print out each character:

```python
for char in 'code':
    print(char)
```

The result would be:

```python
c
o
d
e
```

Just like in JavaScript, you can also nest `for` loops in Python. Here is an example of using a nested `for` loop:

```python
categories = ['Fruit', 'Vegetable']
foods = ['Apple', 'Carrot', 'Banana']

for category in categories:
    for food in foods:
        print(category, food)
```

The outer loop will iterate through each `category` in the `categories` list. For each `category`, the inner loop will iterate through each `food` in the `foods` list. Here is the result that will be printed to the console:

```python
Fruit Apple
Fruit Carrot
Fruit Banana
Vegetable Apple
Vegetable Carrot
Vegetable Banana
```

Another type of loop you can use in Python is the `while` loop. This type of loop will repeat a block of code until the condition is `False`. Here is an example of using a `while` loop for a guessing game:

```python
secret_number = 3
guess = 0

while guess != secret_number:
    guess = int(input('Guess the number (1-5): '))
    if guess != secret_number:
        print('Wrong! Try again.')

print('You got it!')
```

In this example we have a `secret_number` variable with the value of `3` and an initial guess of `0`. Then we use the `input` function to get input from the user, then convert the input string into an integer with the `int()` function, and assign it to the `guess` variable. If the user guesses correctly by inputting `3`, the `while` loop is broken out of and the message `You got it!` is printed to the console. Otherwise, the message `Wrong! Try again.` is printed to the console, and the loop repeats, prompting the user to guess again.

Here's an example result:

```python
Guess the number (1-5): 2
Wrong! Try again.
Guess the number (1-5): 1
Wrong! Try again.
Guess the number (1-5): 3
You got it!
```

Just like in JavaScript, Python supports the `break` and `continue` statements.

The `break` statement is used to stop the execution of a loop. Here is an example of using the `break` statement for a list of `developer_names`:

```python
developer_names = ['Jess', 'Naomi', 'Tom']

for developer in developer_names:
    if developer == 'Naomi':
        break
    print(developer)
```

In this example, we iterate through a list of `developer_names` and print each name to the console. If the name is equal to `Naomi`, then we break out of the loop. This results in only the name `Jess` being printed to the console.

The `continue` statement is used to skip the current iteration of a loop and move onto the next iteration. Let's modify the example from earlier to use the `continue` statement instead of `break`:

```python
developer_names = ['Jess', 'Naomi', 'Tom']

for developer in developer_names:
    if developer == 'Naomi':
        continue
    print(developer)
```

Now the result in the console will be different. The names `Jess` and `Tom` are printed because the `continue` statement skips the second iteration of the loop when `developer` is equal to `Naomi`, and does not print that name to the console.

Both `for` and `while` loops can be combined with an `else` clause, which is executed only when the loop is not terminated by a `break` statement. Here is an example of using multiple `for` loops:

```python
words = ['sky', 'apple', 'rhythm', 'fly', 'orange']

for word in words:
    for letter in word:
        if letter.lower() in 'aeiou':
            print(f"'{word}' contains the vowel '{letter}'")
            break
    else:
        print(f"'{word}' has no vowels")
```

In this example we have a list of random words, and a `for` loop is used to loop through each word. Inside the outer `for` loop, we have another `for` loop to loop through each letter of each word. If the lowercase version of the letter is a vowel, we print the word followed by what vowels it contains, then break out of the inner loop. If the word contains no vowels, then we print a message indicating that.

Here is what the result looks like in the console:

```python
'sky' has no vowels
'apple' contains the vowel 'a'
'rhythm' has no vowels
'fly' has no vowels
'orange' contains the vowel 'o'
```

Loops are very common in Python, so it's important to get comfortable with them. In the next few lessons, you will learn how to work with the `enumerate()` and `range()` functions in loops.

---

# What Are Ranges and How Can You Use Them in a Loop?

The `range()` function is used to generate a sequence of integers. Here is the basic syntax for the `range()` function:

```python
range(start, stop, step)
```

The required `stop` argument is an integer that represents the end point for the sequence of numbers being generated. Here is an example of using the `range()` function:

```python
for num in range(3):
    print(num)
```

The following code generates a sequence of numbers between `0` and `2`. The integer `3` is not included because the `stop` argument is non-inclusive.

If a `start` argument is not specified, then the default is `0`. Otherwise, you can use the optional `start` argument to start the sequence of integers at a integer other than `0`. Here is an example of generating a sequence of integers between `1` and `4`:

```python
for num in range(1, 5):
    print(num)
```

By default the sequence of integers will increment by `1`. But if you want to change that default, then you can use the optional `step` argument. Here is an example of generating a sequence of even integers between `2` and `10`:

```python
for num in range(2, 11, 2):
    print(num)
```

As mentioned earlier, there is only one required argument for the `range()` function. If you don't provide any arguments to `range()`, then you'll get a `TypeError`:

```python
ERROR!
Traceback (most recent call last):
  File "<main.py>", line 1, in <module>
TypeError: range expected at least 1 argument, got 0
```

It is important to note that the `range()` function only accepts integers as arguments, not floats. Remember that floats are numbers with decimal points like `3.4`. If you try to pass floats as arguments, you'll get a `TypeError`:

```python
ERROR!
Traceback (most recent call last):
  File "<main.py>", line 1, in <module>
TypeError: 'float' object cannot be interpreted as an integer
```

If you want to generate a sequence of integers in decrementing order, then you can use a negative integer for the `step` argument, like this:

```python
for num in range(40, 0, -10):
    print(num)
```

The following code prints the numbers `40`, `30`, `20`, and `10` in that order to the console.

Another thing you can do with the `range()` function is create a list of integers by using it with the `list` constructor. The `list` constructor is used to convert an iterable into a list. Here is an example of generating a list of even integers between `2` and `10`:

```python
numbers = list(range(2, 11, 2))
print(numbers) # [2, 4, 6, 8, 10]
```

The `range()` function is a very handy way to generate a sequence of integers in Python. Once you get the hang of it, you'll probably find yourself using it a lot in your Python programs.

---

# What Are Lists and How Do They Work?

Over the next few lessons we are going to learn about lists, tuples, and ranges, which are three basic sequence types used in Python.

The list data type is an ordered sequence of elements that can be comprised of strings, numbers, or even other lists. Lists are mutable and use zero-based indexing, meaning that the first element of the list is at index zero.

Here is the basic syntax for a list:

```python
cities = ['Los Angeles', 'London', 'Tokyo']
```

To access an element from the `cities` list, you can reference its index number in the sequence. Here is an example of accessing the first element of the `cities` list:

```python
cities = ['Los Angeles', 'London', 'Tokyo']
cities[0] # 'Los Angeles'
```

Negative indexing is used to access elements starting from the end of the list instead of the beginning at index `0`. To access the last element of any list, you can use `-1` like this:

```python
cities = ['Los Angeles', 'London', 'Tokyo']
cities[-1] # 'Tokyo'
```

Another way to create a list is to use the `list()` constructor. The `list()` constructor is used to convert an iterable into a list like this:

```python
developer = 'Jessica'
list(developer) # ['J', 'e', 's', 's', 'i', 'c', 'a']
```

An iterable is a special type of object that can be looped over one item at a time. You will learn more about loops in Python later on.

To get the total number of elements in a list, you can use the `len()` function like this:

```python
numbers = [1, 2, 3, 4, 5]
len(numbers) # 5
```

If you wanted to update a value at a particular index, you can do something like this:

```python
programming_languages = ['Python', 'Java', 'C++', 'Rust']
programming_languages[0] = 'JavaScript'
print(programming_languages) # ['JavaScript', 'Java', 'C++', 'Rust']
```

Since lists are mutable, you can update any element in the list as long as you pass in a valid index number. If you pass in an index (either positive or negative) that is out of bounds for the list, then you will receive an `IndexError`:

```python
programming_languages = ['Python', 'Java', 'C++', 'Rust']
programming_languages[10] = 'JavaScript'

"""
Traceback (most recent call last):
  File "<stdin>", line 2, in <module>
IndexError: list assignment index out of range
"""
```

If you want to remove an element from a list you can use the `del` keyword like this:

```python
developer = ['Jane Doe', 23, 'Python Developer']
del developer[1]
print(developer) # ['Jane Doe', 'Python Developer']
```

Sometimes it is helpful to check if an element is inside the list. To do that, you can use the `in` keyword like this:

```python
programming_languages = ['Python', 'Java', 'C++', 'Rust']

'Rust' in programming_languages # True
'JavaScript' in programming_languages # False
```

Sometimes it is common to have lists nested inside of other lists like this:

```python
developer = ['Alice', 25, ['Python', 'Rust', 'C++']]
```

In this example, we have one nested list containing three popular programming languages. To access the nested list, you will need to access it using index `2` since lists are zero based indexed:

```python
developer = ['Alice', 25, ['Python', 'Rust', 'C++']]
developer[2] # ['Python', 'Rust', 'C++']
```

Then to access the second language from that nested list, you will need to access it using index `1` like this:

```python
developer = ['Alice', 25, ['Python', 'Rust', 'C++']]
developer[2][1] # 'Rust'
```

Another common technique used with lists is unpacking values.

Unpacking values from a list is a technique used to assign values from a list to new variables. Here is an example of unpacking a `developer` list into new variables called `name`, `age` and `job`.

```python
developer = ['Alice', 34, 'Rust Developer']
name, age, job = developer

print(name) # 'Alice'
print(age) # 34
print(job) # 'Rust Developer'
```

Here, `name` has the value `'Alice'`, `age` has the value `34`, and `job` has the value `'Rust Developer'`.

If you need to collect any remaining elements from a list, you can use the asterisk (`*`) operator like this:

```python
developer = ['Alice', 34, 'Rust Developer']
name, *rest = developer

print(name) # 'Alice'
print(rest) # [34, 'Rust Developer']
```

In this example, `name` will still have the value `'Alice'`, and `rest` is a list of two items: the number `34` and the string `'Rust Developer'`.

If the numbers of variables on the left side of the assignment operator doesn't match the total numbers of items in the list, then you will receive a `ValueError`:

```python
developer = ['Alice', 34, 'Rust Developer']
name, age, job, city = developer

"""
Traceback (most recent call last):
  File "<stdin>", line 2, in <module>
ValueError: not enough values to unpack (expected 4, got 3)
"""
```

The last concept we will look at is the slice operator (`:`). Similar to strings, you can access portions of a list by using the slice operator like this:

```python
desserts = ['Cake', 'Cookies', 'Ice Cream', 'Pie', 'Brownies']
desserts[1:4] # ['Cookies', 'Ice Cream', 'Pie']
```

In this example, the start index is `1` since that points to the second item in the list. Then we use the slice operator followed by an end index of `4`, which includes everything up to (but not including), the item at that index.

Another thing you can do with the slice operator `:` is specify a step interval which determines how much to increment between the indices. Let's say you had a list of numbers like this:

```python
numbers = [1, 2, 3, 4, 5, 6]
```

If you wanted to extract a list of just even numbers, you can use the slicing operator like this:

```python
numbers = [1, 2, 3, 4, 5, 6]
numbers[1::2] # [2, 4, 6]
```

The first even number is at index `1`, so that will be the start index. Since we want to go through the end of the list, then we omit the end index. Lastly, we specify `2` for the optional step interval so it will only increment by `2` instead of the default `1`.

Lists are a useful and flexible data structure that you will use a lot in your Python programs. In the next lesson, you will learn about common methods that you can use with lists.

---

# What Are Some Common Methods Used for Lists?

In the previous lesson, you were introduced to the list data type and learned how to access elements from a list as well as list slicing. In this lesson, you will continue to learn about lists and some common methods associated with them like `append()`, `pop()`, and `sort()`.

The first method we will look at is the `append()` method. This is used to add an item to the end of the list. Here is an example of using the `append()` method to add the number `6` to list of numbers:

```python
numbers = [1, 2, 3, 4, 5]
numbers.append(6)
print(numbers) # [1, 2, 3, 4, 5, 6]
```

If you want to add one list at the end of another, you can also use the `append()` method like this:

```python
numbers = [1, 2, 3, 4, 5]
even_numbers = [6, 8, 10]

numbers.append(even_numbers)
print(numbers) # [1, 2, 3, 4, 5, [6, 8, 10]]
```

Notice how the entire `even_numbers` list is nested inside of the `numbers` list.

But if you want to add all of the individual numbers from the `even_numbers` list at the end of the `numbers` list, then you can use the `extend()` method.

The `extend()` method is similar to the `append()` method, but with `extend()` you can add multiple elements from one list to another. Here's an example of adding the numbers `6`, `8`, and `10` from one list to the end of the `numbers` list:

```python
numbers = [1, 2, 3, 4, 5]
even_numbers = [6, 8, 10]

numbers.extend(even_numbers)
print(numbers) # [1, 2, 3, 4, 5, 6, 8, 10]
```

As you can see, the nested list is gone and it's just a list of numbers.

To insert an element at a specific index in a list, you can use the `insert()` method. This method accepts two arguments: the index where you wish to insert the new item and the item you want to insert.

Here is an example of using the `insert()` method:

```python
numbers = [1, 2, 3, 4, 5]
numbers.insert(2, 2.5)

print(numbers) # [1, 2, 2.5, 3, 4, 5]
```

The following code will insert the number `2.5` at index `2` in the `numbers` list.

If you want to remove an element from a list, you can use the `remove()` method. The `remove()` method takes the value of the element to remove as an argument:

```python
numbers = [10, 20, 30, 40, 50, 50]
numbers.remove(50)

print(numbers) # [10, 20, 30, 40, 50]
```

It is important to note that this method will only remove the first occurrence of an item. Not all of them:

```python
numbers = [10, 20, 30, 40, 50, 50, 50]
numbers.remove(50)

print(numbers) # [10, 20, 30, 40, 50, 50]
```

To remove an element at a specific index in the list, you can use the `pop()` method like this:

```python
numbers = [1, 2, 3, 4, 5]
numbers.pop(1) # The number 2 is returned
```

If you don't specify an element for the `pop` method, then the last element is removed.

```python
numbers = [1, 2, 3, 4, 5]
numbers.pop() # The number 5 is returned
```

If you need to empty the list, then you can use the `clear()` method like this:

```python
numbers = [1, 2, 3, 4, 5]
numbers.clear()

print(numbers) # []
```

The next method we will take a look at is the `sort()` method. This method is used to sort the elements in place. Here is an example of sorting a random list of numbers in place:

```python
numbers = [19, 2, 35, 1, 67, 41]
numbers.sort()

print(numbers) # [1, 2, 19, 35, 41, 67]
```

In contrast to the `sort()` method, there is the `sorted()` function which works for any iterable and returns a new sorted list instead of modifying the original list. For example:

```python
numbers = [19, 2, 35, 1, 67, 41]
sorted_numbers = sorted(numbers)

print(numbers) # [19, 2, 35, 1, 67, 41]
print(sorted_numbers) # [1, 2, 19, 35, 41, 67]
```

As a reminder, an iterable is a special type of object that you can loop over, allowing you to access each item one at a time. You'll learn more about how loops work in Python in a future lesson.

Both the `sort()` method and `sorted()` function accept optional `key` and `reverse` parameters. You will learn more about these optional parameters in a future lesson when you learn about tuples. You'll also learn more about other built-in functions like `sorted()` in future lessons.

The next method we will take a look at is the `reverse()` method. This method, will reverse a list of elements in place like this:

```python
numbers = [6, 5, 4, 3, 2, 1]
numbers.reverse()

print(numbers) # [1, 2, 3, 4, 5, 6]
```

The last method we will take a look at is the `index` method. This is used to find the first index where an element can be found in a list. Here is an example of using the `index` method to find the language `'Java'` in a `programming_languages` list:

```python
programming_languages = ['Rust', 'Java', 'Python', 'C++']
programming_languages.index('Java') # 1
```

If the element cannot be found, then Python throws a `ValueError`:

```python
programming_languages = ['Rust', 'Java', 'Python', 'C++']
programming_languages.index('JavaScript')

"""
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
ValueError: 'JavaScript' is not in list
"""
```

There are a few more methods for Python lists, but this initial list of methods is a good place to start.

---

# What Are List Comprehensions and What Are Some Useful Functions to Work With Lists?

For the past few lessons, you have been getting comfortable working with loops like this:

```python
even_numbers = []

for num in range(21):
    if num % 2 == 0:
        even_numbers.append(num)

print(even_numbers)
```

This example creates a new empty list called `even_numbers` and loops through a sequence of numbers between `0` and `20`. Inside the loop, there's a condition that checks if the current number has a remainder of `0` when divided by `2`. This is used to determine if the number is even. If the condition is `True`, then the current `num` is appended at the end of the `even_numbers` list. Finally, we print the `even_numbers` list to the console.

While this code works, there is a more concise way to write this that uses list comprehension instead. List comprehension allows you to create a new list in a single line by combining a loop and condition directly within square brackets. This makes the code shorter and often easier to read.

Here is the refactored example from earlier using square brackets:

```python
even_numbers = [num for num in range(21) if num % 2 == 0]
print(even_numbers)
```

In this refactored example, the `even_numbers` list is created using a single line of code. The list comprehension loops through numbers from `0` to `20`, and includes only those that are divisible by `2`. This approach is more compact and eliminates the need for a separate loop and conditional block.

Let's take a look at another example so we can better understand how list comprehension works:

```python
numbers = [1, 2, 3, 4, 5]
result = [(num, 'Even') if num % 2 == 0 else (num, 'Odd') for num in numbers]
print(result)
```

In this example, we have a list of numbers and want to create a new list of tuples indicating which numbers are even or odd. In the first part of the list comprehension, we use an `if` statement to check if the number is evenly divisible by `2`. If so, then the result is a tuple of that number followed by the word `Even`. Otherwise, the result is a tuple with the number followed by the word `Odd`.

Here is what the result looks like printed in the console:

```python
[(1, 'Odd'), (2, 'Even'), (3, 'Odd'), (4, 'Even'), (5, 'Odd')]
```

Another way to create a list starting from an existing iterable is the `filter()` function. Here is an example of creating a new list of just words longer than four characters:

```python
words = ['tree', 'sky', 'mountain', 'river', 'cloud', 'sun']

def is_long_word(word):
    return len(word) > 4

long_words = list(filter(is_long_word, words))
print(long_words) # ['mountain', 'river', 'cloud']
```

The `filter()` function is used to select elements from an iterable that meet a specific condition. The `filter()` function accepts a function and an iterable for its arguments. In this example, we are passing in an `is_long_word` function into the `filter()` function to check if the current word count is greater than `4`. All words that have a character count greater than `4` are added into a new list and assigned to the `long_words` variable.

Aside from the `filter()` function, there are a few more functions that are helpful when working with lists. Another function to be aware of is the `map()` function, which takes an iterable and applies a function to each of its elements. Here is an example of using the `map()` function to convert a list of temperatures from Celsius to Fahrenheit:

```python
celsius = [0, 10, 20, 30, 40]

def to_fahrenheit(temp):
    return (temp * 9/5) + 32

fahrenheit = list(map(to_fahrenheit, celsius))
print(fahrenheit) # [32.0, 50.0, 68.0, 86.0, 104.0]
```

Just like the `filter()` function, `map()` accepts a function and an iterable for its arguments. The `to_fahrenheit` function takes a temperature and converts it from Celsius to Fahrenheit.

The last function we will look at is the `sum()` function. This function is used to get the sum from an iterable like a list or tuple. Here is an example of using the `sum()` function:

```python
numbers = [5, 10, 15, 20]
total = sum(numbers)
print(total) # Result: 50
```

You can also pass in an optional `start` argument which sets the initial value for the summation. Here is an updated example using the `start` argument as a positional argument:

```python
numbers = [5, 10, 15, 20]
total = sum(numbers, 10) # positional argument
print(total) # 60
```

You can also choose to use the `start` argument as a keyword argument like this instead:

```python
numbers = [5, 10, 15, 20]
total = sum(numbers, start=10) # keyword argument
print(total) # 60
```

Both versions will produce the same result, but the keyword argument is a little more explicit.

List comprehension as well as other functions like `map()`, `filter()`, and `sum()` might seem a little confusing at first. But with enough practice and time, you will start to feel more comfortable using them in your Python programs.

---

# What Are Tuples and How Do They Work?

A tuple is a Python data type used to create an ordered sequence of values. Tuples can contain a mixed set of data types like this:

```python
developer = ('Alice', 34, 'Rust Developer')
```

Tuples are similar to lists, but while lists are a mutable data type, tuples are immutable. This means that the elements in a tuple cannot be changed once it's created.

If you try to update one of the items in the tuple, you will get a `TypeError`:

```python
programming_languages = ('Python', 'Java', 'C++', 'Rust')
programming_languages[0] = 'JavaScript'

"""
Traceback (most recent call last):
  File "<stdin>", line 2, in <module>
TypeError: 'tuple' object does not support item assignment
"""
```

To access an element from a tuple, you can use bracket notation and the index number:

```python
developer = ('Alice', 34, 'Rust Developer')
developer[1] # 34
```

If you need to access elements starting from the end of a tuple, then you can use negative indexing. Here is an example of using a negative index to access the second to last element in a tuple:

```python
numbers = (1, 2, 3, 4, 5)
numbers[-2] # 4
```

If you try to pass in an index number that exceeds or equals the length of the tuple, then you will receive an `IndexError` like this:

```python
numbers = (1, 2, 3, 4, 5)
numbers[7]

"""
Traceback (most recent call last):
  File "<stdin>", line 2, in <module>
IndexError: list index out of range
"""
```

Another way to create a tuple is by using the `tuple()` constructor like this:

```python
developer = 'Jessica'
tuple(developer) # ('J', 'e', 's', 's', 'i', 'c', 'a')
```

For the `tuple()` constructor, you can pass in different iterables like strings, lists and even other tuples.

To check if an item is in a tuple, you can use the `in` keyword like this:

```python
programming_languages = ('Python', 'Java', 'C++', 'Rust')

'Rust' in programming_languages # True
'JavaScript' in programming_languages # False
```

You can also unpack items from a tuple just like you did with lists:

```python
developer = ('Alice', 34, 'Rust Developer')
name, age, job = developer

print(name) # 'Alice'
print(age) # 34
print(job) # 'Rust Developer'
```

In this example, `name` has the value `'Alice'`, `age` has the value `34`, and `job` has the value `'Rust Developer'`.

If you need to collect any remaining elements from a tuple, you can use the asterisk (`*`) operator like this:

```python
developer = ('Alice', 34, 'Rust Developer')
name, *rest = developer

print(name) # 'Alice'
print(rest) # [34, 'Rust Developer']
```

Here, `name` has the value `'Alice'`, and `rest` is a list comprised of the number `34` and the string `'Rust Developer'`.

Just like with a list, you can use the slice operator on a tuple to extract a portion of it. Here is an example of extracting the items `'pie'` and `'cookies'` into a separate tuple:

```python
desserts = ('cake', 'pie', 'cookies', 'ice cream')
desserts[1:3] # ('pie', 'cookies')
```

Remember that the first number represents the starting index for the extraction while the second number represents the ending index. But note that the item at the ending index is not included in the extracted tuple.

If you need to remove an item from a tuple, that isn't possible because tuples are immutable. So this example, will produce an error:

```python
developer = ('Jane Doe', 23, 'Python Developer')
del developer[1]

"""
Traceback (most recent call last):
  File "<stdin>", line 2, in <module>
TypeError: "tuple" object doesn't support item deletion
"""
```

So when might you use a tuple over a list?

If you need a dynamic collection of elements where you can add, remove and update elements, then you should use a list. If you know that you are working with a fixed and immutable collection of data, then you should use a tuple.

In the next lesson, we will take a look at some common methods you will use when working with tuples.

---

# What Are Some Common Methods for Tuples?

In the previous lesson, you learned how to work with the tuple data type. In this lesson, you'll learn about some common methods you'll use when working with tuples.

The first method we will cover is `count()`. This method is used to determine how many times an item appears in a tuple. Here is an example of checking how many times the string `Rust` appears in a tuple named `programming_languages`:

```python
programming_languages = ('Rust', 'Java', 'Python', 'C++', 'Rust')
programming_languages.count('Rust') # 2
```

Since `Rust` appears twice in the tuple, the `count()` method returns the number `2`. If the specified item in the `count()` function is not present at all in the tuple, then the return value is `0`:

```python
programming_languages = ('Rust', 'Java', 'Python', 'C++', 'Rust')
programming_languages.count('JavaScript') # 0
```

If no arguments are passed into the `count()` function, then Python raises a `TypeError`:

```python
programming_languages = ('Rust', 'Java', 'Python', 'C++', 'Rust')
programming_languages.count()

"""
Traceback (most recent call last):
  File "<stdin>", line 2, in <module>
TypeError: tuple.count() takes exactly one argument (0 given)
"""
```

The next method we will look at is the `index()` method. This method is used to find the index where a particular item is present in a tuple. Here is an example of using the `index()` method to find the index for the string `Java`:

```python
programming_languages = ('Rust', 'Java', 'Python', 'C++', 'Rust')
programming_languages.index('Java') # 1
```

If the specified item cannot be found, then Python raises a `ValueError`:

```python
programming_languages = ('Rust', 'Java', 'Python', 'C++', 'Rust')
programming_languages.index('JavaScript')

"""
Traceback (most recent call last):
  File "<stdin>", line 2, in <module>
ValueError: tuple.index(x): x not in tuple
"""
```

Another thing you can do with the `index()` method is to pass in optional start and stop index arguments. Here is an example of passing in an optional start index:

```python
programming_languages = ('Rust', 'Java', 'Python', 'C++', 'Rust', 'Python')
programming_languages.index('Python', 3) # 5
```

In this example, we are specifying where to start searching for the string `Python`. By passing in the number `3` as the second argument to the `index()` function, we are specifying to start searching at index `3`. Since `Python` appears twice in the tuple, the `index()` function will return index `5` instead of index `2` because of the use of the optional start index argument.

You can also pass in an optional stop index. Here is a modified example of specifying a start and stop index:

```python
programming_languages = ('Rust', 'Java', 'Python', 'C++', 'Rust', 'Python', 'JavaScript', 'Python')
programming_languages.index('Python', 2, 5) # 2
```

Now the result is index `2` because we are starting the search at index `2`, and searching up to, but not including, index `5`.

Another commonly used function used with tuples is the `sorted()` function. In a previous lesson you learned about the `sort()` method for lists. Well, the `sorted()` function can be used on any iterable including tuples.

Here is an example of creating a new list of numbers using the `sorted()` function:

```python
numbers = (13, 2, 78, 3, 45, 67, 18, 7)
sorted(numbers) # [2, 3, 7, 13, 18, 45, 67, 78]
```

The `sorted()` function will always create a new list of the sorted values. This differs from the `sort()` method which sorts the elements of a list in place and does not return a new list.

If you need to customize the sorting behavior for an iterable, you can use the optional `reverse` and `key` arguments. Here is an example of using `key` argument to sort items in a tuple by length:

```python
programming_languages = ('Rust', 'Java', 'Python', 'C++', 'Rust', 'Python')
sorted(programming_languages, key=len)

# Result
# ['C++', 'Rust', 'Java', 'Rust', 'Python', 'Python']
```

If you want to create a new list of values in reverse order, then you can use the `reverse` argument like this:

```python
programming_languages = ('Rust', 'Java', 'Python', 'C++', 'Rust', 'Python')

print(sorted(programming_languages, reverse=True))

# Result
# ['Rust', 'Rust', 'Python', 'Python', 'Java', 'C++']
```

Tuples are a common data type in Python. Understanding how to work with them, along with some helpful methods and functions, will help you write more efficient code.

---

# What Are the Enumerate and Zip Functions and How Do They Work?

In previous lessons you learned how to work with the `for` loop, which is used to repeat a block of code a set number of times. Here is an example of using a `for` loop to print each language from the `languages` list to the console:

```python
languages = ['Spanish', 'English', 'Russian', 'Chinese']

for language in languages:
    print(language)
```

But what if you wanted to keep track of the index for each element? Well, one option is to create an `index` variable and increment it by `1` for each iteration of the loop, like this:

```python
languages = ['Spanish', 'English', 'Russian', 'Chinese']

index = 0

for language in languages:
    print(f'Index {index} and language {language}')
    index += 1
```

While that works, an easier way to do that is by using the `enumerate()` function. The `enumerate()` function keeps track of the index for an iterable and returns an enumerate object.

If we pass the `languages` list to the `enumerate()` function and convert its returned value into a list with the `list()` function, it looks like this:

```python
languages = ['Spanish', 'English', 'Russian', 'Chinese']

list(enumerate(languages))
# [(0, 'Spanish'), (1, 'English'), (2, 'Russian'), (3, 'Chinese')]
```

Each entry in the enumerate object (now a list) is a tuple containing a count, followed by a value from the iterable passed to the `enumerate()` function.

Now, let's refactor the example from earlier to use the `enumerate()` function:

```python
languages = ['Spanish', 'English', 'Russian', 'Chinese']

for index, language in enumerate(languages):
    print(f'Index {index} and language {language}')
```

We unpack the count and value for each tuple in the enumerate object into variables named `index` and `language`, respectively. Finally, both those variables are used in an f-string that's printed to the console in each iteration of the loop.

```python
Index 0 and language Spanish
Index 1 and language English
Index 2 and language Russian
Index 3 and language Chinese
```

This removes the need for manually creating and updating an `index` variable.

The `enumerate()` function also accepts an optional `start` argument that specifies the starting value for the count. If this argument is omitted, then the count will begin at `0`. Here is an example of using the optional `start` argument:

```python
languages = ['Spanish', 'English', 'Russian', 'Chinese']

for index, language in enumerate(languages, 1):
    print(f'Index {index} and language {language}')
```

And here is what the result will look like in the console:

```python
Index 1 and language Spanish
Index 2 and language English
Index 3 and language Russian
Index 4 and language Chinese
```

So far we've only been iterating over one list. But what if you need to iterate over multiple iterables in parallel? Well, you can use the `zip()` function for that, which combines lists into pairs of elements and returns an iterator of tuples.

If we pass a list of `developers` and `ids` to the `zip()` function and convert its returned value into a list with the `list()` function, here's what it looks like:

```python
developers = ['Naomi', 'Dario', 'Jessica', 'Tom']
ids = [1, 2, 3, 4]

list(zip(developers, ids))
# [('Naomi', 1), ('Dario', 2), ('Jessica', 3), ('Tom', 4)]
```

And here's an example of using the `zip()` function with a `for` loop to iterate over `developers` and `ids`:

```python
developers = ['Naomi', 'Dario', 'Jessica', 'Tom']
ids = [1, 2, 3, 4]

for name, id in zip(developers, ids):
    print(f'Name: {name}')
    print(f'ID: {id}')
```

In this example, `zip()` combines the two lists into pairs of elements and returns an iterator of tuples. The `for` loop then unpacks each tuple into `name` and `id`. Finally, for each print statement, we are printing each `name` and `id` from the `ids` and `developers` lists respectively. Here is what the result looks like in the console:

```python
Name: Naomi
ID: 1
Name: Dario
ID: 2
Name: Jessica
ID: 3
Name: Tom
ID: 4
```

The `enumerate()` and `zip()` functions are very powerful, and when combined with loops, can make your code much more concise.

---

## Module Review Component

# Loops and Sequences Review

Python Lists
------------

* **Introduction**: In Python, the list data type is an ordered sequence of elements that can be composed of strings, numbers or even other lists. Lists are mutable and zero based indexed.

```python
cities = ['Los Angeles', 'London', 'Tokyo']
```

* **Accessing Elements in a List**: To access an element from the `cities` list, you can reference its index number in the sequence:

```python
cities = ['Los Angeles', 'London', 'Tokyo']
cities[0] # Los Angeles
```

* **Accessing Elements Using Negative Indexing**: To access the last element of any list, you can use `-1` as the index number:

```python
cities = ['Los Angeles', 'London', 'Tokyo']
cities[-1] # Tokyo
```

* Negative indexing is used to access elements starting from the end of the list instead of the beginning at index `0`.
* **Creating Lists Using the `list()` constructor**: Lists can also be created using the `list()` constructor. The `list()` constructor is used to convert an iterable into a list:

```python
developer = 'Jessica'

print(list(developer)) 
# Result: ['J', 'e', 's', 's', 'i', 'c', 'a']
```

* **Finding the Length of a List**: You can use the `len()` function to get the length of a list:

```python
numbers = [1, 2, 3, 4, 5]
len(numbers) # 5
```

* **List Mutability**: Lists are mutable, meaning you can update any element in the list as long as you pass in a valid index number. To update lists at a particular index, you can assign a new value to that index:

```python
programming_languages = ['Python', 'Java', 'C++', 'Rust']
programming_languages[0] = 'JavaScript'
print(programming_languages) # ['JavaScript', 'Java', 'C++', 'Rust']
```

* **Index Out of Range Error**: If you pass in an index (either positive or negative) that is out of bounds for the list, then you will receive an `IndexError`:

```python
programming_languages = ['Python', 'Java', 'C++', 'Rust']
programming_languages[10] = 'JavaScript'

"""
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
IndexError: list assignment index out of range
"""
```

* **Removing Elements from a List**: Elements can be removed from a list using the `del` keyword:

```python
developer = ['Jane Doe', 23, 'Python Developer']
del developer[1]
print(developer) # ['Jane Doe', 'Python Developer']
```

* **Checking if an Element Exists in a List**: The `in` keyword can be used to check if an element exists in a list:

```python
programming_languages = ['Python', 'Java', 'C++', 'Rust']

'Rust' in programming_languages # True
'JavaScript' in programming_languages # False
```

* **Nesting Lists**: Lists can be nested inside other lists:

```python
developer = ['Alice', 25, ['Python', 'Rust', 'C++']]
```

* To access the nested list, you will need to access it using index `2` since lists are zero-based indexed.

```python
developer = ['Alice', 25, ['Python', 'Rust', 'C++']]
developer[2] # ['Python', 'Rust', 'C++']
```

* To further access the second language from that nested list, you will need to access it using index `1`:

```python
developer = ['Alice', 25, ['Python', 'Rust', 'C++']]
developer[2][1] # Rust
```

* **Unpacking Values from a List:** Unpacking values from a list is a technique used to assign values from a list to new variables. Here is an example to unpack the `developer` list into new variables called `name`, `age` and `job` like this:

```python
developer = ['Alice', 34, 'Rust Developer']
name, age, job = developer
```

* If the number of variables on the left side of the assignment operator doesn't match the total number of items in the list, then you will receive a `ValueError`.
* **Collecting Remaining Items From a List**: To collect any remaining elements from a list, you can use the asterisk (`*`) operator like this:

```python
developer = ['Alice', 34, 'Rust Developer']
name, *rest = developer
```

* **Slicing Lists**: Slicing is the concept of accessing a portion of a list by using the slice operator `:`. To slice a list that starts at index `1` and ends before index `3`, you can use the following syntax:

```python
desserts = ['Cake', 'Cookies', 'Ice Cream', 'Pie']
desserts[1:3] # ['Cookies', 'Ice Cream']
```

* **Step Intervals**: It is also possible to specify a step interval which determines how much to increment between the indices. Here is an example if you want to extract a list of just even numbers using slicing:

```python
numbers = [1, 2, 3, 4, 5, 6]
numbers[1::2] # [2, 4, 6]
```

List Methods
------------

* **append()**: Used to add an item to the end of the list. Here is an example of using the `append()` method to add the number `6` to this `numbers` list:

```python
numbers = [1, 2, 3, 4, 5]
numbers.append(6)
print(numbers) # [1, 2, 3, 4, 5, 6]
```

* **Appending lists**: The `append()` method can also be used to add one list at the end of another:

```python
numbers = [1, 2, 3, 4, 5]
even_numbers = [6, 8, 10]

numbers.append(even_numbers)
print(numbers) # [1, 2, 3, 4, 5, [6, 8, 10]]
```

* **extend()**: Used to add multiple items to the end of a list. Here is an example of adding the numbers `6`, `8`, and `10` to the end of the `numbers` list:

```python
numbers = [1, 2, 3, 4, 5]
even_numbers = [6, 8, 10]

numbers.extend(even_numbers)
print(numbers) # [1, 2, 3, 4, 5, 6, 8, 10]
```

* **insert()**: Used to insert an item at a specific index in the list. Here is an example of using the `insert()` method:

```python
numbers = [1, 2, 3, 4, 5]
numbers.insert(2, 2.5)

print(numbers) # [1, 2, 2.5, 3, 4, 5]
```

* **remove():** Used to remove an item from the list. The `remove()` method will only remove the first occurrence of an item in the list:

```python
numbers = [1, 2, 3, 4, 5, 5, 5]
numbers.remove(5)

print(numbers) # [1, 2, 3, 4, 5, 5]
```

* **pop()**: Used to remove a specific item from the list and return it:

```python
numbers = [1, 2, 3, 4, 5]
numbers.pop(1) # The number 2 is returned
```

* If you don't specify an element for the `pop` method, then the last element is removed.

```python
numbers = [1, 2, 3, 4, 5]
numbers.pop() # The number 5 is returned
```

* **clear()**: Used to remove all items from the list:

```python
numbers = [1, 2, 3, 4, 5]
numbers.clear()

print(numbers) # []
```

* **sort()**: The `sort()` method is used to sort the elements in place. Here is an example of sorting a random list of `numbers` in place:

```python
numbers = [19, 2, 35, 1, 67, 41]
numbers.sort()

print(numbers) # [1, 2, 19, 35, 41, 67]
```

* **sorted()**: A built-in function that returns a new sorted list instead of modifying the original list:

```python
numbers = [19, 2, 35, 1, 67, 41]
sorted_numbers = sorted(numbers)

print(sorted_numbers) # [1, 2, 19, 35, 41, 67]
print(numbers) # [19, 2, 35, 1, 67, 41]
```

* **reverse()**: Used to reverse the order of the elements in a list:

```python
numbers = [6, 5, 4, 3, 2, 1]
numbers.reverse()

print(numbers) # [1, 2, 3, 4, 5, 6]
```

* **index()**: Used to find the first index where an element can be found in a list:

```python
programming_languages = ['Rust', 'Java', 'Python', 'C++']
programming_languages.index('Java') # 1
```

* If the element cannot be found using the `index()` method, then the result will be a `ValueError`.

Tuples in Python
----------------

* **Definition**: A tuple is a Python data type used to create an ordered sequence of values. Tuples can contain a mixed set of data types:

```python
developer = ('Alice', 34, 'Rust Developer')
```

* Tuples are immutable, meaning the elements in the tuple cannot be changed once created. If you try to update one of the items in the tuple, you will get a `TypeError`:

```python
programming_languages = ('Python', 'Java', 'C++', 'Rust')
programming_languages[0] = 'JavaScript'

"""
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: "tuple" object does not support item assignment
"""
```

* **Accessing Elements from a Tuple**: To access an element from a tuple, use bracket notation and the index number:

```python
developer = ('Alice', 34, 'Rust Developer')
developer[1] # 34
```

* Negative indexing can be used to access elements starting from the end of the tuple:

```python
numbers = (1, 2, 3, 4, 5)
numbers[-2] # 4
```

* If you try to pass in an index number that exceeds or equals the length of the tuple, then you will receive an `IndexError`:

```python
numbers = (1, 2, 3, 4, 5)
numbers[7]

"""
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
IndexError: tuple index out of range
"""
```

* A tuple can also be created using the `tuple()` constructor. Within the constructor, you can pass in different iterables like strings, lists and even other tuples.

```python
developer = 'Jessica'

print(tuple(developer)) 
# Result: ('J', 'e', 's', 's', 'i', 'c', 'a')
```

* **Verifying Items in a Tuple**: To check if an item is in a tuple, you can use the `in` keyword like this:

```python
programming_languages = ('Python', 'Java', 'C++', 'Rust')

'Rust' in programming_languages # True
'JavaScript' in programming_languages # False
```

* **Unpacking Tuples**: Items can be unpacked from a tuple like this:

```python
developer = ('Alice', 34, 'Rust Developer')
name, age, job = developer
```

* If you need to collect any remaining elements from a tuple, you can use the asterisk (`*`) operator like this:

```python
developer = ('Alice', 34, 'Rust Developer')
name, *rest = developer
```

* **Slicing Tuples**: Slicing can be used to extract a portion of a tuple. For example, the items `pie` and `cookies` can be sliced into a separate tuple:

```python
desserts = ('cake', 'pie', 'cookies', 'ice cream')
desserts[1:3] # ('pie', 'cookies')
```

* **Removing Items from Tuples**: Removing an item from a tuple will raise a `TypeError` as tuples are immutable:

```python
developer = ('Jane Doe', 23, 'Python Developer')
del developer[1]

"""
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: "tuple" object doesn't support item deletion
"""
```

* **When to use a Tuple vs a List?**: If you need a dynamic collection of elements where you can add, remove and update elements, then you should use a list. If you know that you are working with a fixed and immutable collection of data, then you should use a tuple.

Common Tuple Methods
--------------------

* **`count()`**: Used to determine how many times an item appears in a tuple. For example, you can check how many times the language `'Rust'` appears in the tuple:

```python
programming_languages = ('Rust', 'Java', 'Python', 'C++', 'Rust')
programming_languages.count('Rust') # 2
```

* If the specified item in the `count()` method is not present at all in the tuple, then the return value will be `0`:

```python
programming_languages = ('Rust', 'Java', 'Python', 'C++', 'Rust')
programming_languages.count('JavaScript') # 0
```

* If no arguments are passed to the `count()` method, then Python will return a `TypeError`.
* **index()**: Used to find the index where a particular item is present in the tuple. Here is an example of using the `index()` method to find the index for the language `'Java'`:

```python
programming_languages = ('Rust', 'Java', 'Python', 'C++', 'Rust')
programming_languages.index('Java') # 1
```

* If the specified item cannot be found, then Python will return a `ValueError`.
* You can pass an optional start index to the `index()` method to specify where to start searching for the item in the tuple:

```python
programming_languages = ('Rust', 'Java', 'Python', 'C++', 'Rust', 'Python')
programming_languages.index('Python', 3) # 5
```

* You can also pass in an optional end index to the `index()` method to specify where to stop searching for the item in the tuple:

```python
programming_languages = ('Rust', 'Java', 'Python', 'C++', 'Rust', 'Python', 'JavaScript', 'Python')
programming_languages.index('Python', 2, 5) # 2
```

* **`sorted()`**: Used to sort the elements in any iterable and return a new sorted list. Here is an example of creating a new list of numbers using the `sorted()` function:

```python
numbers = (13, 2, 78, 3, 45, 67, 18, 7)
sorted(numbers) # [2, 3, 7, 13, 18, 45, 67, 78]
```

* **Modifying Sorting Behavior**: You can customize the sorting behavior for an iterable using the optional `reverse` and `key` arguments. Here is an example of using the `key` argument to sort items in a tuple by length:

```python
programming_languages = ('Rust', 'Java', 'Python', 'C++', 'Rust', 'Python')
sorted(programming_languages, key=len)

# Result
# ['C++', 'Rust', 'Java', 'Rust', 'Python', 'Python']
```

* You can create a new list of values in reverse order, using the `reverse` argument like this:

```python
programming_languages = ('Rust', 'Java', 'Python', 'C++', 'Rust', 'Python')

print(sorted(programming_languages, reverse=True))

# Result
# ['Rust', 'Rust', 'Python', 'Python', 'Java', 'C++']
```

Loops in Python
---------------

* **Definition**: Loops are used to repeat a block of code for a set number of times.
* **`for` loop**: Used to iterate over a sequence (like a list, tuple or string) and execute a block of code for each item in that sequence. Here is an example of using a `for` loop to iterate through a list and print each language to the console:

```python
programming_languages = ['Rust', 'Java', 'Python', 'C++']

for language in programming_languages:
    print(language)

"""
Result 

Rust
Java
Python
C++
"""
```

* Here is an example of using a `for` loop to loop through the string `code` and print out each character:

```python
for char in 'code':
    print(char)

"""
Result 

c
o
d
e
"""
```

* `for` loops can be nested. Here is an example of using a nested `for` loop:

```python
categories = ['Fruit', 'Vegetable']
foods = ['Apple', 'Carrot', 'Banana']

for category in categories:
    for food in foods:
        print(category, food)

"""
Result

Fruit Apple
Fruit Carrot
Fruit Banana
Vegetable Apple
Vegetable Carrot
Vegetable Banana
"""
```

* **`while` loop**: Repeats a block of code until the condition is `False`. Here is an example of using a `while` loop for a guessing game:

```python
secret_number = 3
guess = 0

while guess != secret_number:
    guess = int(input('Guess the number (1-5): '))
    if guess != secret_number:
        print('Wrong! Try again.')

print('You got it!')

"""
Result

Guess the number (1-5): 2
Wrong! Try again.
Guess the number (1-5): 1
Wrong! Try again.
Guess the number (1-5): 3
You got it!
"""
```

* **`break` and `continue` statements**: Used in loops to modify the execution of a loop.
* The `break` statement is used to exit the loop immediately when a certain condition is met. Here is an example of using the `break` statement for a list of `developer_names`:

```python
developer_names = ['Jess', 'Naomi', 'Tom']

for developer in developer_names:
    if developer == 'Naomi':
        break
    print(developer)
```

* The `continue` statement is used to skip that current iteration and move onto the next iteration of the loop. Here is an example to use the `continue` statement instead of a `break` statement:

```python
developer_names = ['Jess', 'Naomi', 'Tom']

for developer in developer_names:
    if developer == 'Naomi':
        continue
    print(developer)
```

* Both `for` and `while` loops can be combined with an `else` clause, which is executed only when the loop was not terminated by a `break`:

```python
words = ['sky', 'apple', 'rhythm', 'fly', 'orange']

for word in words:
    for letter in word:
        if letter.lower() in 'aeiou':
            print(f"'{word}' contains the vowel '{letter}'")
            break
    else:
        print(f"'{word}' has no vowels")
```

Ranges and Their Use in Loops
-----------------------------

* **The `range()` function**: Used to generate a sequence of integers.

```python
range(start, stop, step)
```

* The required `stop` argument is an integer(non-inclusive) that represents the end point for the sequence of numbers being generated. Here is an example of using the `range()` function:

```python
for num in range(3):
    print(num)
```

* If a `start` argument is not specified, then the default will be `0`. By default the sequence of integers will increment by `1`. You can use the optional `step` argument to change the default increment value. Here is an example of generating a sequence of even integers from 2 up to but not including 11 (i.e., includes 10)

```python
for num in range(2, 11, 2):
    print(num)
```

* If you don't provide any arguments to the `range()` function, then you will get a `TypeError`.
* The `range()` function only accepts integers for arguments and not floats. Using floats will also result in a `TypeError`:

```python
ERROR!
Traceback (most recent call last):
  File "<main.py>", line 1, in <module>
TypeError: 'float' object cannot be interpreted as an integer
```

* You can use a negative integer for the `step` argument to generate a sequence of integers in decrementing order:

```python
for num in range(40, 0, -10):
    print(num)
```

* The `range()` function can also be used to create a list of integers by using it with the `list` constructor. The `list` constructor is used to convert an iterable into a list. Here is an example of generating a list of even integers between 2 and 10 inclusive:

```python
numbers = list(range(2, 11, 2))
print(numbers) # [2, 4, 6, 8, 10]
```

`enumerate()` and `zip()` functions in Python
---------------------------------------------

* **`enumerate()`**: used to iterate over a sequence and keep track of the index for each item in that sequence. The `enumerate()` function takes an iterable as an argument and returns an `enumerate` object that consist of the index and value of each item in the iterable.

```python
languages = ['Spanish', 'English', 'Russian', 'Chinese']

for index, language in enumerate(languages):
    print(f'Index {index} and language {language}')

# Result
# Index 0 and language Spanish
# Index 1 and language English
# Index 2 and language Russian
# Index 3 and language Chinese
```

* The `enumerate()` function can also be used outside of a `for` loop:

```python
languages = ['Spanish', 'English', 'Russian', 'Chinese']

print(list(enumerate(languages)))
# [(0, 'Spanish'), (1, 'English'), (2, 'Russian'), (3, 'Chinese')]
```

* The `enumerate()` function also accepts an optional `start` argument that specifies the starting value for the count. If this argument is omitted, then the count will begin at `0`.
* **`zip()`** : Used to iterate over multiple iterables in parallel. Here's an example using the `zip()` function to iterate over `developers` and `ids`:

```python
developers = ['Naomi', 'Dario', 'Jessica', 'Tom']
ids = [1, 2, 3, 4]

for name, id in zip(developers, ids):
    print(f'Name: {name}')
    print(f'ID: {id}')


"""
Result

Name: Naomi
ID: 1
Name: Dario
ID: 2
Name: Jessica
ID: 3
Name: Tom
ID: 4
"""
```

List comprehensions in Python
-----------------------------

* **Definition**: List comprehension allows you to create a new list in a single line by combining the loop and the condition directly within square brackets. This makes the code shorter and often easier to read.

```python
even_numbers = [num for num in range(21) if num % 2 == 0]
print(even_numbers)
```

Iterable methods
----------------

* **`filter()`**: Used to filter elements from an iterable based on a condition. It returns an iterator that contains only the elements that satisfy the condition. Here is an example of creating a new list of just words longer than four characters:

```python
words = ['tree', 'sky', 'mountain', 'river', 'cloud', 'sun']

def is_long_word(word):
    return len(word) > 4

long_words = list(filter(is_long_word, words))
print(long_words) # ['mountain', 'river', 'cloud']
```

* **`map()`**: Used to apply a function to each item in an iterable and return a new iterable with the results. Here is an example of using the `map()` function to convert a list of celsius temperatures to fahrenheit:

```python
celsius = [0, 10, 20, 30, 40]

def to_fahrenheit(temp):
    return (temp * 9/5) + 32

fahrenheit = list(map(to_fahrenheit, celsius))
print(fahrenheit) # [32.0, 50.0, 68.0, 86.0, 104.0]
```

* **`sum()`**: Used to get the sum from an iterable like a list or tuple. Here is an example of using the `sum()` function:

```python
numbers = [5, 10, 15, 20]
total = sum(numbers)
print(total) # Result: 50
```

* You can also pass in an optional `start` argument which sets the initial value for the summation. Here is an updated example using the `start` argument as a positional argument:

```python
numbers = [5, 10, 15, 20]
total = sum(numbers, 10) # positional argument
print(total) # 60
```

* You can also choose to use the `start` argument as a keyword argument like this instead:

```python
numbers = [5, 10, 15, 20]
total = sum(numbers, start=10) # keyword argument
print(total) # 60
```

Lambda functions
----------------

* **Definition**: A lambda function in Python is a concise way to create a function without a name (an anonymous function).
* Lambda functions are often used as an argument to another function. Here is an example of a lambda function:

```python
numbers = [1, 2, 3, 4, 5]

even_numbers = list(filter(lambda x: x % 2 == 0, numbers))
print(even_numbers)  # [2, 4]
```

* Best practices for using lambda functions include not assigning them to a variable, keeping them simple and readable, and using them for short, one-off functions.

---

# Module 7: Dictionaries and Sets

# What Are Dictionaries, and How Do They Work?

In Python, dictionaries are built-in data structures that store collections of key-value pairs. They work very similarly to real dictionaries, where you search for a word to find its corresponding meaning.

With Python dictionaries, you use a key to find its corresponding value. You should use dictionaries when you need to associate values to unique keys. This is helpful when you need to find a value fast based on the key, and when you need to represent structured data.

This is the general syntax of a Python dictionary:

```python
dictionary = {
    key1: value1,
    key2: value2
}
```

First, we find the variable that holds the dictionary. You don't necessarily need to assign the dictionary to a variable, but it's very common to do this to keep it in memory and use it later in the code.

Then that's followed by curly braces, which are sometimes called curly brackets. And within the curly braces, there are key-value pairs.

Each key is associated with a value, so you can use the key to access that value. After each value, except the last one, there's a comma to separate the different key-value pairs. Keys must be unique in the dictionary, and they must be an immutable data type. However, the values can be repeated, and they can be of any data type.

Here we have an example of a dictionary that stores information about a Margherita pizza recipe:

```python
pizza = {
    'name': 'Margherita Pizza',
    'price': 8.9,
    'calories_per_slice': 250,
    'toppings': ['mozzarella', 'basil']
}
```

The dictionary is assigned to the `pizza` variable. It has four key-value pairs: `name`, `price`, `calories_per_slice`, and `toppings`.

Another alternative would be using the `dict()` constructor, which builds the dictionary from a sequence of key-value pairs.

This would be the equivalent syntax for our pizza example. We pass a list of tuples as argument to the `dict()` constructor. These tuples contain the key as the first element and the value as the second element.

```python
pizza = dict([('name', 'Margherita Pizza'), ('price', 8.9), ('calories_per_slice', 250), ('toppings', ['mozzarella', 'basil'])])
```

To access the value of a key-value pair, you can use this syntax, known as bracket notation. It's the name of the variable that holds the dictionary, followed by square brackets, and the key you want to access within the square brackets:

```python
dictionary[key]
```

In our pizza example, if you want to access the value of `name`, you would write the name of the variable, `pizza`, followed by square brackets, and the key, `name`, within quotes:

```python
pizza['name']
```

This will evaluate to:

```python
'Margherita Pizza'
```

To update a value, you just need to add the assignment operator, followed by the new value.

If the key doesn't exist in the dictionary, a new key-value pair will be created. In recent versions of Python, dictionaries preserve the order of insertion. This is helpful when you need to iterate over the dictionary:

```python
pizza['name'] = 'Margherita'
```

Now the value of the key `name` is `'Margherita'`:

```python
print(pizza['name']) # 'Margherita'
```

Dictionaries also have helpful methods to perform common operations.

The `.get()` method retrieves the value associated with a key. It's similar to the bracket notation that we just used, but its advantage is that you can set a default value, so you won't get an error if the key doesn't exist:

```python
dictionary.get(key, default)
```

In this example, if the `toppings` key doesn't exist, it will return an empty list, which is the default value that we are passing here as the second argument. But if `toppings` does exist, it will return that value:

```python
pizza.get('toppings', []) # ['mozzarella', 'basil']
```

The `.keys()` and `.values()` methods return a view object with all the keys and values in the dictionary, respectively:

```python
pizza.keys()
# dict_keys(['name', 'price', 'calories_per_slice'])

pizza.values()
# dict_values(['Margherita Pizza', 8.9, 250])
```

A view object is just a way to see the content of a dictionary without creating a separate copy of the data.

The `.items()` method returns a view object with all the key-value pairs in the dictionary, including both the keys and the values:

```python
pizza.items()
# dict_items([('name', 'Margherita Pizza'), ('price', 8.9), ('calories_per_slice', 250)])
```

The `.clear()` method removes all the key-value pairs from the dictionary:

```python
pizza.clear()
```

The `.pop()` method removes the key-value pair with the key that you specify as the first argument and returns its value. If the key doesn't exist, it returns the default value that you specify as the second argument. If the key doesn't exist and you don't pass a default value, a `KeyError` is raised:

```python
pizza.pop('price', 10)
pizza.pop('total_price') # KeyError
```

In Python 3.7 and more recent versions, the `.popitem()` method removes the last inserted item:

```python
pizza.popitem()
```

And finally, the `.update()` method updates the key-value pairs with the key-value pairs of another dictionary. If they have keys in common, their values are overwritten.

In this example, we are updating the `pizza` dictionary. The `price` key exists in both of them, so its value will be replaced with `15`.

But `total_time` is new, so it will be added to the `pizza` dictionary as a new key-value pair:

```python
pizza.update({ 'price': 15, 'total_time': 25 })
```

This is the new dictionary with the updated `price` and the new `total_time`. Notice how the price is now `15` and `total_time` is a new key-value pair:

```python
{
    'name': 'Margherita Pizza', 
    'price': 15, 
    'calories_per_slice': 250, 
    'toppings': ['mozzarella', 'basil'], 
    'total_time': 25
}
```

These are some of the most commonly used dictionary methods, but there are many more. Choosing the right one can be helpful for performing complex operations efficiently.

---

# What Are Some Common Techniques to Loop Over a Dictionary?

You can loop over a dictionary if you need to access and process its key-value pairs. This is helpful for updating their values or applying some logic to them.

Let's take a look at some of the techniques you can use.

Let's say that we have a `products` dictionary that associates every product with its price:

```python
products = {
    'Laptop': 990,
    'Smartphone': 600,
    'Tablet': 250,
    'Headphones': 70,
}
```

If we want to offer a 20% discount on all our products, we can loop over all the key-value pairs and modify the prices.

The `.values()`, `.keys()`, and `.items()` methods are essential for these techniques. We covered them briefly in a previous lesson.

They return a view object with the values, keys, and key-value pairs of the dictionary. You can use these view objects in `for` loops to iterate over the elements.

For example, you can iterate over all the values of the dictionary like this.

You write `for`, the loop variable (`price` in this case), `products.values()` to get all the values of the `products` dictionary, a colon, and then the body of the loop, where you can apply any logic to the values. In this case, we are printing them.

The loop variable will take each one of the values, one per iteration:

```python
for price in products.values():
    print(price)
```

And here is the output. As you can see, each value is printed to the console, one by one:

```python
990
600
250
70
```

This works exactly the same for `.keys()` if you need to iterate over the keys of a dictionary. You just need to iterate over `products.keys()` or `products` directly, and assign a descriptive name for the loop variable:

```python
for product in products.keys():
    print(product)

# Or

for product in products:
    print(product)
```

This is the output. Each key is printed to the console, one at a time:

```python
Laptop
Smartphone
Tablet
Headphones
```

And this works exactly the same for key-value pairs if you need to iterate over the keys and their corresponding values simultaneously. You just need to iterate over `products.items()`:

```python
for product in products.items():
    print(product)
```

This is the output. Now you get individual tuples with the keys and their corresponding values:

```python
('Laptop', 990)
('Smartphone', 600)
('Tablet', 250)
('Headphones', 70)
```

If you want to store the key and the value in separate loop variables, you just need to define them and separate them with a comma. Then, you can use them in the body of the loop.

Here, we are defining a `product` loop variable and a `price` loop variable. Each one will hold its corresponding value. It's important to define them in order – the key first, and then the value:

```python
for product, price in products.items():
    print(product, price)
```

This is the output. We are printing them side by side, but you can use these values as you need them in your code.

```python
Laptop 990
Smartphone 600
Tablet 250
Headphones 70
```

Now that you know more about this, we can go back to our initial example. If we want to offer a 20% discount, we would multiply each price by `0.8` and reassign it as the value of that product key.

We could also round the result down if we want to work with integers:

```python
products = {
    'Laptop': 990,
    'Smartphone': 600,
    'Tablet': 250,
    'Headphones': 70,
}

for product, price in products.items():
    products[product] = round(price * 0.8)

print(products)
```

Then, if we print the dictionary, we would get these key-value pairs with the discounted prices:

```python
{
    'Laptop': 792, 
    'Smartphone': 480, 
    'Tablet': 200, 
    'Headphones': 56
}
```

And finally, if you need to iterate over the key-value pairs while keeping track of a counter, you can call the `enumerate()` function. This counter essentially acts as a sort of "index" or "count" for that element within the loop.

The function returns an `enumerate` object, which assigns an integer to each key-value pair, like a counter. You can start the counter from any number, but by default, it starts from 0.

Here, we are iterating over the keys of the `products` dictionary:

```python
for product in enumerate(products):
    print(product)
```

But the `enumerate()` function also assigns an integer to each key, so we get tuples with the integer and the key.

Here is the output:

```python
(0, 'Laptop')
(1, 'Smartphone')
(2, 'Tablet')
(3, 'Headphones')
```

If you need to, you can assign these values to separate loop variables. Here, we have two loop variables (`index` and `product`). This is what you will commonly see and use when you work with `enumerate()`:

```python
for index, product in enumerate(products):
    print(index, product)
```

If you need to iterate over the values, you can replace `products` by `products.values()`:

```python
for price in enumerate(products.values()):
    print(price)
```

The output will have the index and the price in each tuple:

```python
(0, 990)
(1, 600)
(2, 250)
(3, 70)
```

You can assign them to separate loop variables as well:

```python
for index, price in enumerate(products.values()):
    print(index, price)
```

This will be the output. You can use them as you need to in your code:

```python
0 990
1 600
2 250
3 70
```

And with `products.items()`, you can get the entire key-value pair in addition to the "index" or "counter":

```python
for index, product in enumerate(products.items()):
    print(index, product)
```

In this example, we get the index followed by a tuple that contains the key and the value of the corresponding key-value pair:

```python
0 ('Laptop', 990)
1 ('Smartphone', 600)
2 ('Tablet', 250)
3 ('Headphones', 70)
```

To customize the initial value of the count, you can pass a second argument to `enumerate()`. For example, here we are starting the count from 1:

```python
for index, product in enumerate(products.items(), 1):
    print(index, product)
```

You can see this change in the output. Now the first integer is 1 instead of 0:

```python
1 ('Laptop', 990)
2 ('Smartphone', 600)
3 ('Tablet', 250)
4 ('Headphones', 70)
```

This works with any variation we've seen so far. You just need to pass the initial number as the second argument.

There are many techniques to loop over a dictionary. These are some common ways, and you'll need to choose the best one for your project.

---

# What Are Sets, and How Do They Work?

Sets are one of Python's built-in data structures. One of the core characteristics of sets is that they don't store duplicate values. If you try to add a duplicate value to a set, only one of them will be stored.

Sets are mutable and unordered, which means that their elements are not stored in any specific order, so you cannot use indices or keys to access them. They can only contain values of immutable data types like numbers, strings, and tuples. And they support mathematical set operations, including union, intersection, difference, and symmetric difference.

To define a set, you just need to write its elements within curly braces and separate them with commas. This is an example of a set of numbers:

```python
my_set = {1, 2, 3, 4, 5}
```

One quirk of working with sets is that, if you ever need to define an empty set, you must use the `set()` function. If you just write empty curly braces, like `{}`, Python will automatically create a dictionary.

```python
set() # Set
{}    # Dictionary
```

You can add an element to a set with the `.add()` method, and pass in the new element as argument:

```python
my_set.add(6)
```

In our example, the new set would be:

```python
{1, 2, 3, 4, 5, 6}
```

If you try to add an element that is already in the set, only one will be kept. In this case, we already have the number 5 in the set:

```python
my_set.add(5)
```

So the set will not change:

```python
{1, 2, 3, 4, 5, 6}
```

To remove an element from the set, you have two options. You can either use the `.remove()` method or the `.discard()` method, and pass in the element that you want to remove as argument.

The `.remove()` method will raise a `KeyError` if the element is not found, while the `.discard()` method will not:

```python
my_set.remove(4)
my_set.discard(4)
```

The `.clear()` method removes all the elements from the set:

```python
my_set.clear()
```

Python sets also have powerful methods that perform common mathematical set operations.

The `.issubset()` and the `.issuperset()` methods check if a set is a subset or superset of another set, respectively.

Here, we are checking if `your_set` is a subset of `my_set`, which is `False` because not all the elements of `your_set` are in `my_set`.

We are also checking if `my_set` is a superset of `your_set`. This is also `False` because `my_set` does not have all the elements of `your_set`:

```python
my_set = {1, 2, 3, 4, 5}
your_set = {2, 3, 4, 6}

print(your_set.issubset(my_set)) # False
print(my_set.issuperset(your_set)) # False
```

The `.isdisjoint()` method checks if two sets are disjoint, which means they don't have any elements in common. In this case, that's `False` because `my_set` and `your_set` do have common elements – 2, 3, and 4:

```python
print(my_set.isdisjoint(your_set)) # False
```

The union operator `|` returns a new set with all the elements from both sets:

```python
my_set | your_set # {1, 2, 3, 4, 5, 6}
```

The intersection operator `&` returns a new set with only the elements that the sets have in common:

```python
my_set & your_set # {2, 3, 4}
```

The difference operator `-` returns a new set with the elements of the first set that are not in the other sets. In this example, the numbers 1 and 5 are in `my_set` but NOT in `your_set`:

```python
my_set - your_set # {1, 5}
```

The symmetric difference operator `^` returns a new set with the elements that are either in the first or the second set, but not both. In this case, 1 and 5 are in `my_set` but not in `your_set`, so they are included. And the number 6 is in `your_set` but not in `my_set`, so it's included as well:

```python
my_set ^ your_set # {1, 5, 6}
```

Each one of these operators also has its corresponding compound assignment operator if you add the equal sign next to it. These operators automatically assign the resulting set to the first set in the expression:

```python
|= &= -= ^=
```

For example, the `-=` operator finds the difference between the sets and updates the first set with that result:

```python
my_set -= your_set
```

After this, `my_set` will be updated to `{1, 5}`:

```python
print(my_set) # {1, 5}
```

You can check if an element is in a set or not with the `in` operator. Here, we are checking if 5 is in `my_set`. The result will be a boolean value `True` or `False`:

```python
print(5 in my_set)
```

And those are the fundamentals of sets. They are very helpful when you don't need to store the values in any specific order, and when you only need to store unique values.

---

## Module Review Component

# Dictionaries and Sets Review

Dictionaries
------------

* **Dictionaries**: Dictionaries are built-in data structures that store collections of key-value pairs. Keys need to be immutable data types. This is the general syntax of a Python dictionary:

```python
dictionary = {
    key1: value1,
    key2: value2
}
```

* **`dict()` Constructor**: The `dict()` constructor is an alternative way to build the dictionary. You pass a list of tuples as an argument to the `dict()` constructor. These tuples contain the key as the first element and the value as the second element.

```python
pizza = dict([('name', 'Margherita Pizza'), ('price', 8.9), ('calories_per_slice', 250), ('toppings', ['mozzarella', 'basil'])])
```

* **Bracket Notation**: To access the value of a key-value pair, you can use the syntax known as bracket notation.

```python
dictionary[key]
```

Common Dictionary Methods
-------------------------

* **`get()` Method**: The `get()` method retrieves the value associated with a key. It's similar to the bracket notation, but it lets you set a default value, preventing errors if the key doesn't exist.

```python
dictionary.get(key, default)
```

* **`keys()` and `values()` Methods**: The `keys()` and `values()` methods return a view object with all the keys and values in the dictionary, respectively. A view object is a way to see the content of a dictionary without creating a separate copy of the data.

```python
pizza = {
    'name': 'Margherita Pizza',
    'price': 8.9,
    'calories_per_slice': 250
}

pizza.keys()
# dict_keys(['name', 'price', 'calories_per_slice'])

pizza.values()
# dict_values(['Margherita Pizza', 8.9, 250])
```

* **`items()` Method**: The `items()` method returns a view object with all the key-value pairs in the dictionary, including both the keys and the values.

```python
pizza.items()
# dict_items([('name', 'Margherita Pizza'), ('price', 8.9), ('calories_per_slice', 250)])
```

* **`clear()` Method**: The `clear()` method removes all the key-value pairs from the dictionary.

```python
pizza.clear()
```

* **`pop()` Method**: The `pop()` method removes the key-value pair with the key specified as the first argument and returns its value. If the key doesn't exist, it returns the default value specified as the second argument. If the key doesn't exist and the default value is not specified, a `KeyError` is raised.

```python
pizza.pop('price', 10)
pizza.pop('total_price') # KeyError
```

* **`popitem()` Method**: In Python 3.7 and above, the `popitem()` method removes the last inserted item.

```python
pizza.popitem()
```

* **`update()` Method**: The `update()` method updates the key-value pairs with the key-value pairs of another dictionary. If they have keys in common, their values are overwritten. New keys will be added to the dictionary as new key-value pairs.

```python
pizza.update({ 'price': 15, 'total_time': 25 })
```

Looping Over a Dictionary
-------------------------

* **Iterating Over Values**: If you need to iterate over the values in a dictionary, you can write a `for` loop with `values()` to get all the values of a dictionary.

```python
products = {
    'Laptop': 990,
    'Smartphone': 600,
    'Tablet': 250,
    'Headphones': 70,
}

for price in products.values():
    print(price)
```

Output:

```python
990
600
250
70
```

* **Iterating Over Keys**: If you need to iterate over the keys in the `products` dictionary above, you can write `products.keys()` or `products` directly.

```python
for product in products.keys():
    print(product)

# Or

for product in products:
    print(product)
```

Output:

```python
Laptop
Smartphone
Tablet
Headphones
```

* **Iterating Over Key-Value Pairs**: If you need to iterate over the keys and their corresponding values simultaneously, you can iterate over `products.items()`. You get individual tuples with the keys and their corresponding values.

```python
for product in products.items():
    print(product)
```

Output:

```python
('Laptop', 990)
('Smartphone', 600)
('Tablet', 250)
('Headphones', 70)
```

To store the key and value in separate loop variables, you need to separate them with a comma. The first variable stores the key, and the second stores the value.

```python
for product, price in products.items():
    print(product, price)
```

Output:

```python
Laptop 990
Smartphone 600
Tablet 250
Headphones 70
```

* **`enumerate()` Function**: If you need to iterate over a dictionary while keeping track of a counter, you can call the `enumerate()` function. The function returns an `enumerate` object, which assigns an integer to each item, like a counter. You can start the counter from any number, but by default, it starts from 0.

Assigning the index and item to separate loop variables is the common way to use `enumerate()`. For example, with `products.items()`, you can get the entire key-value pair in addition to the index:

```python
for index, product in enumerate(products.items()):
    print(index, product)
```

Output:

```python
0 ('Laptop', 990)
1 ('Smartphone', 600)
2 ('Tablet', 250)
3 ('Headphones', 70)
```

To customize the initial value of the count, you can pass a second argument to `enumerate()`. For example, here we are starting the count from 1.

```python
for index, product in enumerate(products.items(), 1):
    print(index, product)
```

Output:

```python
1 ('Laptop', 990)
2 ('Smartphone', 600)
3 ('Tablet', 250)
4 ('Headphones', 70)
```

Sets
----

* **Sets**: Sets are built-in data structures in Python that do not allow duplicate values. Sets are mutable and unordered, which means that their elements are not stored in any specific order, so you cannot use indices or keys to access them. Also, sets can only contain values of immutable data types, like numbers, strings, and tuples.
* **Defining a Set**: To define a set, you need to write its elements within curly brackets and separate them with commas.

```python
my_set = {1, 2, 3, 4, 5}
```

* **Defining an Empty Set**: If you need to define an empty set, you must use the `set()` function. Only writing empty curly braces will automatically create a dictionary.

```python
set() # Set
{}    # Dictionary
```

Common Set Methods
------------------

* **`add()` Method**: You can add an element to a set with the `add()` method, passing the new element as an argument.

```python
my_set.add(6)
```

* **`remove()` and `discard()` Methods**: To remove an element from a set, you can either use the `remove()` method or the `discard()` method, passing the element you want to remove as an argument. The `remove()` method will raise a `KeyError` if the element is not found while the `discard()` method will not.

```python
my_set.remove(4)
my_set.discard(4)
```

* **`clear()` method**: The `clear()` method removes all the elements from the set.

```python
my_set.clear()
```

Mathematical Set Operations
---------------------------

* **`issubset()` and `issuperset()` Methods**: The `issubset()` and the `issuperset()` methods check if a set is a subset or superset of another set, respectively.

```python
my_set = {1, 2, 3, 4, 5}
your_set = {2, 3, 4, 5}

print(your_set.issubset(my_set)) # True
print(my_set.issuperset(your_set)) # True
```

* **`isdisjoint()` Method**: The `isdisjoint()` method checks if two sets are disjoint, if they don't have elements in common.

```python
my_set = {1, 2, 3}
your_set = {4, 5, 6}

print(my_set.isdisjoint(your_set)) # True
```

* **Union Operator (`|`)**: The union operator `|` returns a new set with all the elements from both sets.

```python
my_set = {1, 2, 3}
your_set = {4, 5, 6}

my_set | your_set # {1, 2, 3, 4, 5, 6}
```

* **Intersection Operator (`&`)**: The intersection operator `&` returns a new set with only the elements that the sets have in common.

```python
my_set = {1, 2, 3, 4, 5}
your_set = {2, 3, 4, 6}

my_set & your_set # {2, 3, 4}
```

* **Difference Operator (`-`)**: The difference operator `-` returns a new set with the elements of the first set that are not in the other sets.

```python
my_set = {1, 2, 3, 4, 5}
your_set = {2, 3, 4, 6}

my_set - your_set # {1, 5}
```

* **Symmetric Difference Operator (`^`)**: The symmetric difference operator `^` returns a new set with the elements that are either in the first or the second set, but not both.

```python
my_set = {1, 2, 3, 4, 5}
your_set = {2, 3, 4, 6}

my_set ^ your_set # {1, 5, 6}
```

* **`in` Operator**: You can check if an element is in a set or not with the `in` operator.

```python
print(5 in my_set) # True
```

Python Standard Library
-----------------------

* **Python Standard Library**: A library gives you pre-written and reusable code, like functions, classes, and data structures, that you can reuse in your projects. Python has an extensive standard library with built-in modules that implement standardized solutions for many problems and tasks. Some examples of popular built-in modules are `math`, `random`, `re` (short for "regular expressions"), and `datetime`.

Import Statement
----------------

* **Import Statement**: To access the elements defined in built-in modules, you use an import statement. Import statements are generally written at the top of the file. Import statements work the same for functions, classes, constants, variables, and any other elements defined in the module.
* **Basic Import Statement**: You can use the `import` keyword followed by the name of the module:

```python
import module_name
```

Then, if you need to call a function from that module, you would use dot notation, with the name of the module followed by the name of the function.

```python
module_name.function_name()
```

For example, you would write the following in your code to import the `math` module and get the square root of 36:

```python
import math

math.sqrt(36)
```

* **Importing a Module with a Different Name**: If you need to import the module with a different name (also known as an "alias"), you can use `as` followed by the alias at the end of the import statement. This is often used for long module names or to avoid naming conflicts.

```python
import module_name as module_alias
```

For example, to refer to the `math` module as `m` in your code, you can assign an alias like this:

```python
import math as m
```

Then, you can access the elements of the module using the alias:

```python
m.sqrt(36)
```

* **Importing Specific Elements**: If you don't need everything from a module, you can import specific elements using `from`. In this case, the import statement starts with `from`, followed by the module name, then the `import` keyword, and finally the names of the elements you want to import.

```python
from module_name import name1, name2
```

Then, you can use these names without the module prefix in your Python script. For example:

```python
from math import radians, sin, cos

angle_degrees = 40
angle_radians = radians(angle_degrees)

sine_value = sin(angle_radians)
cos_value = cos(angle_radians)

print(sine_value) # 0.6427876096865393
print(cos_value)  # 0.766044443118978
```

This is helpful, but it can result in naming conflicts if you already have functions or variables with the same name. Keep it in mind when choosing which type of import statement you want to use.

If you need to assign aliases to these names, you can do so as well, using the `as` keyword followed by the alias.

```python
from module_name import name1 as alias1, name2 as alias2
```

* **Import Statement with Asterisk (`*`)**: The asterisk tells Python that you want to import everything in that module, but you want to import it so that you don't need to use the name of the module as a prefix.

```python
from module_name import *
```

For example, if you use this to import the `math` module, you'll be able to call any function defined in that module without specifying the name of the module as a prefix.

```python
from math import *
print(sqrt(36))  # 6.0
```

However, this is generally discouraged because it can lead to namespace collisions and make it harder to know where names come from.

`if __name__ == '__main__'`
---------------------------

* **`__name__` Variable**: `__name__` is a special built-in variable in Python. When a Python file is executed directly, Python sets the value of this variable to the string `"__main__"`. But if the Python file is imported as a module into another Python script, the value of the `__name__` variable is set to the name of that module.

This is why you'll often find this conditional in Python scripts. It contains the code that you only want to run **only** if the Python script is running as the main program.

```python
if __name__ == '__main__': 
    # Code
```

---

# Module 8: Error Handling and Debugging

# How Does Exception Handling Work?

In Python, exception handling is a core part of writing robust and fault-tolerant programs. It allows you to anticipate, catch, and respond to errors in a structured way.

Exception handling is the process of catching and managing errors that occur during the execution of a program, so your code doesn't crash unexpectedly.

Python provides the `try`, `except`, `else`, and `finally` blocks to gracefully handle errors. Here's a basic example:

```python
try:
    x = 10 / 0
except ZeroDivisionError:
    print("You can't divide by zero!")
```

* `try`: The block of code where you anticipate an error might occur.
* `except`: This block runs if an error of the specified type is raised inside the try.
* In this case, dividing by zero raises a `ZeroDivisionError`, which is then caught and handled.

And here's an example also showing how to use the `else` and `finally` blocks:

```python
try:
    x = 10 / 2
except ZeroDivisionError:
    print("You can't divide by zero!")
else:
    print('Division successful:', x)
finally:
    print('This block always runs.')
```

* `else`: Runs if no exception is raised in the try block.
* `finally`: Runs no matter what—whether or not an exception occurred. Useful for clean-up tasks like closing files or releasing resources.

You can also catch multiple exceptions with separate `except` blocks:

```python
try:
    number = int('abc')
    result = 10 / number
except ValueError:
    print('That was not a valid number.')
except ZeroDivisionError:
    print("Can't divide by zero.")
```

By using separate `except` clauses, you can make your error responses more specific and useful.

You can also use the exception object, which is typically aliased to another name with the `as` keyword. Here we're using `e` as an alias for the error object:

```python
try:
    x = 1 / 0
except ZeroDivisionError as e:
    print(f'Error occurred: {e}')
```

Using `e` lets you access the actual error message or object for logging or debugging.

You can also catch multiple exceptions in a single `except` clause by specifying the exceptions as a tuple:

```python
try:
    number = int(input('Enter a number: '))
    result = 10 / number
except (ValueError, ZeroDivisionError) as e:
    print(f'Error occurred: {e}')
```

Exception handling allows your programs to recover from errors gracefully. By using `try`, `except`, `else`, and `finally`, you can anticipate potential issues and build more resilient applications.

---

# What Are Some Common Error Messages in Python?

When writing Python code, it's common to run into errors. Understanding these errors is key to debugging your code quickly and efficiently. These messages tell you exactly what went wrong, if you know how to read them.

Common Python errors include `SyntaxError`, `NameError`, `TypeError`, `IndexError`, and `AttributeError`. These occur when Python doesn't understand your code, or when your logic doesn't match the data you're working with.

Here is an example of a `SyntaxError`:

```python
print("Hello, world!"
# SyntaxError: unexpected EOF while parsing
```

This line is missing a closing parenthesis. Python raises a `SyntaxError` because the code doesn't follow proper syntax rules.

Here is an example of a `NameError`:

```python
print(name)
# NameError: name 'name' is not defined
```

You're trying to print a variable that hasn't been defined yet. Python raises a `NameError` when it can't find a variable by that name.

Here is an example of a `TypeError`:

```python
5 + "5"
# TypeError: unsupported operand type(s) for +: 'int' and 'str'
```

You can't add an integer and a string together. Python raises a `TypeError` when you try to perform an operation on incompatible data types.

Here is an example of an `IndexError`:

```python
my_list = [1, 2, 3]
print(my_list[5])
# IndexError: list index out of range
```

You're trying to access an index that doesn't exist in the list. Python raises an `IndexError` when you go out of bounds.

Here is an example of an `AttributeError`:

```python
num = 42
num.append(5)
# AttributeError: 'int' object has no attribute 'append'
```

The `int` object doesn't have an `append()` method. Python raises an `AttributeError` when you try to use a method or property that doesn't exist for that data type.

Recognizing common Python error messages helps you fix problems faster. Instead of guessing, read the error message carefully. It often tells you exactly what went wrong and where to look.

---

# What Is the Raise Statement and How Does It Work?

In Python, the `raise` statement is a powerful tool that allows you to manually trigger exceptions in your code. It gives you control over when and how errors are generated, enabling you to create custom error conditions and enforce specific program behavior.

The `raise` statement is used to explicitly throw an exception at any point in your program, allowing you to signal that an error condition has occurred or that certain requirements haven't been met.

Python's `raise` statement can be used in several ways to trigger exceptions. At its most basic, you can raise built-in exceptions or create custom error messages. Here's a simple example:

```python
def check_age(age):
    if age < 0:
        raise ValueError('Age cannot be negative')
    return age

try:
    check_age(-5)
except ValueError as e:
    print(f'Error: {e}') # Error: Age cannot be negative
```

You can see here that `raise` is the keyword that triggers an exception.

In this example, we're raising a `ValueError` with a custom message when an invalid age is provided.

The `raise` statement can also be used to re-raise the current exception, which is particularly useful in exception handling:

```python
def process_data(data):
    try:
        result = int(data)
        return result * 2
    except ValueError:
        print('Logging: Invalid data received')
        raise  # Re-raises the same ValueError

try:
    process_data('abc')
except ValueError:
    print('Handled at higher level')
```

Here the keyword `raise` (without arguments), re-raises the current exception that's being handled.

This allows you to log or perform cleanup while still propagating the error up the call stack.

You can create and raise custom exceptions by defining your own exception classes:

```python
class InsufficientFundsError(Exception):
    def __init__(self, balance, amount):
        self.balance = balance
        self.amount = amount
        super().__init__(f'Insufficient funds: ${balance} available, ${amount} requested')

def withdraw(balance, amount):
    if amount > balance:
        raise InsufficientFundsError(balance, amount)
    return balance - amount

try:
    new_balance = withdraw(100, 150)
except InsufficientFundsError as e:
    print(f'Transaction failed: {e}')
```

Here you can see custom exception classes inherit from `Exception` or its subclasses.

You'll learn more about classes and inheritance in future lessons. For now, know that this is a way to create your own exceptions with custom logic.

The `raise` statement can also be used with the `from` keyword to chain exceptions, showing the relationship between different errors:

```python
def parse_config(filename):
    try:
        with open(filename, 'r') as file:
            data = file.read()
            return int(data)
    except FileNotFoundError:
        raise ValueError('Configuration file is missing') from None
    except ValueError as e:
        raise ValueError('Invalid configuration format') from e

config = parse_config('config.txt')
```

Here you can see that `raise ... from None`, suppresses the original exception context:

```python
Traceback (most recent call last):
  File "main.py", line 12, in <module>
    config = parse_config('config.txt')
             ^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "main.py", line 7, in parse_config
    raise ValueError('Configuration file is missing') from None
ValueError: Configuration file is missing
```

And `raise ... from e`, chains the new exception to the original one, preserving the error trail.

```python
Traceback (most recent call last):
  File "main.py", line 5, in parse_config
    return int(data)
           ^^^^^^^^^
ValueError: invalid literal for int() with base 10: ''

The above exception was the direct cause of the following exception:

Traceback (most recent call last):
  File "main.py", line 12, in <module>
    config = parse_config('config.txt')
             ^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "main.py", line 9, in parse_config
    raise ValueError('Invalid configuration format') from e
ValueError: Invalid configuration format
```

You can also raise exceptions conditionally using `assert` statements, which are essentially shorthand for `raise` with `AssertionError`:

```python
def calculate_square_root(number):
    assert number >= 0, 'Cannot calculate square root of negative number'
    return number ** 0.5

try:
    result = calculate_square_root(-4)
except AssertionError as e:
    print(f'Assertion failed: {e}')
```

The `raise` statement is essential for creating robust applications where you need to enforce business rules, validate input, and provide meaningful error messages. By strategically using `raise`, you can make your code more predictable and easier to debug, while giving users clear feedback about what went wrong.

---

# What Are Some Good Debugging Techniques in Python?

Debugging is an essential skill for any Python developer. Understanding foundational techniques can help you identify and fix issues efficiently.

Debugging is the process of identifying and resolving errors or bugs in your code. It involves examining the code, understanding the flow, and using tools to pinpoint the source of problems.

In this lesson, we'll go over common debugging techniques you can use in your next Python project.

Using the `print()` function and f-strings
------------------------------------------

First, using the `print()` function and f-strings at various points in your code can help you understand the flow and state of variables. For example:

```python
def add(a, b):
    result = a + b
    print(f'Adding {a} and {b} gives {result}')
    return result
```

By printing the values of `a`, `b`, and `result`, you can verify that the function behaves as expected.

Interactive debugging with the `pdb` module
-------------------------------------------

Next, you can utilize Python's built-in `pdb` module for interactive debugging:

```python
import pdb

def divide(a, b):
    pdb.set_trace()
    return a / b

print(divide(10, 2))
```

By setting a trace with the `set_trace()` function, you can step through the code, inspect variables, and understand the program's behavior.

If you run the code above, you'll see some output showing the location of the file you're running, the line where you called the `set_trace()` function and the code immediately after it, and an interactive `pdb` prompt:

```python
> /Users/fcc/Desktop/debugging.py(5)divide()
-> return a / b
(Pdb)
```

If you enter `help` into the prompt, you'll see a list of commands you can use:

```python
(Pdb) help

Documented commands (type help <topic>):
========================================
EOF    c          d        h         list      q        rv       undisplay
a      cl         debug    help      ll        quit     s        unt      
alias  clear      disable  ignore    longlist  r        source   until    
args   commands   display  interact  n         restart  step     up       
b      condition  down     j         next      return   tbreak   w        
break  cont       enable   jump      p         retval   u        whatis   
bt     continue   exit     l         pp        run      unalias  where    

Miscellaneous help topics:
==========================
exec  pdb
```

Then you can use the commands to debug your code.

For example, if you want to look at the type of elements throughout your code at that moment, you can use the `whatis` command:

```python
(Pdb) whatis a
<class 'int'>
(Pdb) whatis divide
Function divide
```

As you can see, by the time you run `.set_trace()`, the type of the parameter `a` is an integer, and `divide` is a function.

Then to continue execution of your code, you can use the `continue` command, or one of its aliases, `cont` or `c`:

```python
(Pdb) continue
5.0
```

IDE debugging tools
-------------------

Many Integrated Development Environments (IDEs) offer advanced debugging tools, such as breakpoints, step execution, and variable inspection.

Using VS Code debugger
----------------------

If you use VS Code, you can set breakpoints in your code and run the debugger to pause execution at those points. Here's how to debug the same `divide` function:

**Step 1: Set up your code**

Create a file called `main.py` with the following content:

```python
def divide(a, b):
    result = a / b
    return result

print(divide(10, 2))
print(divide(15, 3))
```

**Step 2: Set a breakpoint**

1. Click in the gutter (left margin) next to line 2 (`result = a / b`) to set a breakpoint
2. A red dot will appear, indicating the breakpoint is set

**Step 3: Start debugging**

1. Press `F5` or go to Run > Start Debugging
2. Select "Python File" when prompted
3. The debugger will pause execution at your breakpoint

**Step 4: Inspect variables**

* Hover over variables to see their current values
* Use the Variables panel on the left to see all local variables
* Use the Debug Console at the bottom to evaluate expressions

**Step 5: Step through code**

Use the debug toolbar to:

* **Continue (F5)**: Resume execution until the next breakpoint
* **Step Over (F10)**: Execute the current line and move to the next
* **Step Into (F11)**: Enter into function calls
* **Step Out (Shift+F11)**: Exit the current function

IDE debugging tools provide a visual interface to examine the state of your program, making it easier to identify and fix issues compared to using print statements alone.

By mastering these foundational debugging techniques - using `print()` statements, the `pdb` module, and IDE tools - you can effectively identify and resolve issues in your Python code. Each technique has its place: `print()` statements for quick checks, `pdb` for interactive exploration, and IDE debuggers for visual inspection.

---

## Module Review Component

# Error Handling Review

Common Errors in Python
-----------------------

* **SyntaxError**: The error Python raises when your code does not follow its syntax rules. For example, the code `print("Hello there"` will lead to a syntax error with the message, `SyntaxError: '(' was never closed`, because the code is missing a closing parenthesis.
* **NameError**: Python raises a `NameError` when you try to access a variable or function you have not defined. For instance, if you have the line `print(username)` in your code without having a `username` variable defined first, you will get a name error with the message `NameError: name 'username' is not defined`.
* **TypeError**: This is the error Python throws when you perform an operation on two or more incompatible data types. For example, if you try to add a string to a number, you'll get the error `TypeError: can only concatenate str (not "int") to str`.
* **IndexError**: You'll get an `IndexError` if you access an index that does not exist in a list or other sequences like tuple and string. For example, in a `Hello world` string, the index of the last character is `11`. If you go ahead and access a character this way, `greet = "hello world"; print(greet[12])`, you'll get an error with the message `IndexError: string index out of range`.
* **AttributeError**: Python raises this error when you try to use a method or property that does not exist in an object of that type. For example, calling `.append()` on a string like `"hello".append("!")` will lead to an error with the message `AttributeError: 'str' object has no attribute 'append'`.

Good Debugging Techniques in Python
-----------------------------------

* **Using the `print` function**: Inserting `print()` statements around various points in your code while debugging helps you see the values of variables and how your code flows.
* **Using Python's Built-in Debugger (`pdb`)**: Python provides a `pdb` module for debugging. It's a part of the Python's standard library, so it's always available to use. With `pdb`, you can set a trace with the `set_trace()` function so you can start stepping through the code and inspect variables in an interactive way.
* **Leveraging IDE Debugging Tools**: Many integrated development environments (IDEs) and code editors like Pycharm and VS Code offer debugging tools with breakpoints, step execution, variable inspection, and other debugging features.

Exception Handling
------------------

* **`try...except`**: This is used to execute a block of code that might raise an exception. The `try` block is where you anticipate an error might occur, while the `except` block takes a specified exception and runs if that specified error is raised. Here's an example:

  ```
  try:
    print(22 / 0)
  except ZeroDivisionError:
    print('You can\'t divide by zero!')
    # You can't divide by zero!
  ```

  You can also chain multiple `except` blocks so you can handle more types of exceptions:

  ```
  try:
    number = int(input('Enter a number: '))
    print(22 / number)
  except ZeroDivisionError:
    print('You cannot divide by zero!')
    # You cannot divide by zero! prints when you enter 0
  except ValueError:
    print('Please enter a valid number!')
    # Please enter a valid number! prints when you enter a string
  ```
* **`else` and `finally`**: These blocks extend `try...except`. If no exception occurs, the `else` block runs. The `finally` block always runs regardless of errors.

  ```
  try:
    result = 100 / 4
  except ZeroDivisionError:
    print('You cannot divide by zero!') # This will not run
  else:
    print(f'Result is {result}') # Result is 25.0
  finally:
    print('Execution complete!') # Execution complete!
  ```
* **Exception Object**: This lets you access the exception itself for better debugging and printing the direct error message. To access the exception object, you need to use the `as` keyword. Here's an example:

  ```
  try:
      value = int('This will raise an error')
  except ValueError as e:
      print(f'Caught an error: {e}')
      # Caught an error: invalid literal for int() with base 10: 'This will raise an error'
  ```
* **The `raise` Statement**: This allows you to manually raise an exception. You can use it to throw an exception when a certain condition is met. Here's an example:

  ```
  def divide(a, b):
      if b == 0:
          raise ZeroDivisionError('You cannot divide by zero')
      return a / b
  ```

Exception Signaling
-------------------

The `raise` statement is also useful when you create your own custom exceptions, as you can use it to throw an exception with a custom message. Here's an example of that:

```python
class InvalidCredentialsError(Exception):
    def __init__(self, message="Invalid username or password"):
        self.message = message
        super().__init__(self.message)

def login(username, password):
    stored_username = "admin"
    stored_password = "password123"
    
    if username != stored_username or password != stored_password:
        raise InvalidCredentialsError()
    
    return f"Welcome, {username}!"
```

Here's a how you can use the `login` function with the `InvalidCredentialsError` exception:

```python
# failed login attempt
try:
    message = login("user", "wrongpassword")
except InvalidCredentialsError as e:
    print(f"Login failed: {e}")
else:
    print(message)

# successful login attempt
try:
    message = login("admin", "password123")
except InvalidCredentialsError as e:
    # This block is not executed because the login was successful
    print(f"Login failed: {e}")
else:
    # The else block runs if the 'try' block completes without an exception
    print(message)
```

The `raise` statement can also be used with the `from` keyword to chain exceptions, showing the relationship between different errors:

```python
def parse_config(filename):
  try:
      with open(filename, 'r') as file:
          data = file.read()
          return int(data)
  except FileNotFoundError:
      raise ValueError('Configuration file is missing') from None
  except ValueError as e:
      raise ValueError('Invalid configuration format') from e

config = parse_config('config.txt')
```

---

# Module 9: Classes, Objects, and Object-Oriented Programming (OOP)

# How Do Classes Work and How Do They Differ From Objects?

In Python, classes and objects work hand in hand to organize and manage data. You build a class to define shared behavior, then create objects that use those behaviors.

In other words, a class is like a blueprint or template you use to create objects with.

Let's look at what classes are, and how to use them to create objects.

To create a class, you use the `class` keyword followed by the name of the class and a colon. Then within the class, you can add an initializer, along with any attributes and methods.

Attributes are like variables within a class, and are used to store data. Methods are functions defined within a class, and are the actions objects created with a class can perform.

Here's the basic syntax of a class:

```python
class ClassName:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def sample_method(self):               
        print(self.name.upper())
```

* `class ClassName` is made up of the `class` keyword to create a class, followed by the name of the class, here called `ClassName`. It is common in Python to use the **PascalCase** convention when naming classes.
* `def __init__(self, name, age)` is the special method automatically called when a new object is created. It initializes the attributes of the objects that will be created with the class.

  In addition to that, the first parameter of `__init__` is always a reference to the specific object being created or used. By convention, this parameter is named `self`, but technically, you can use any name. `self` lets you access the object's own attributes and methods.
* `self.name = name` and `self.age = age` are the attributes the objects will have.
* `def sample_method(self):` is the method each object created can call.
* `print(self.name.upper())` is what the `sample_method` method will do, in this case, it prints the name in uppercase.

If that all sounds like a lot, don't worry. Let's take a look at a similar example of a `Dog` class, and how you can create objects from that:

```python
class Dog:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def bark(self):
        print(f"{self.name.upper()} says woof woof!")
```

With this `Dog` class, you can create an object. Here's the basic syntax for creating objects from a class:

```python
object_1 = ClassName(attribute_1, attribute_2)
object_2 = ClassName(attribute_1, attribute_2)
```

You can also call any of the methods defined in the class from each object:

```python
object_1.method_name()
object_2.method_name()
```

Now let's create two dogs by using the `Dog` class as the blueprint:

```python
class Dog:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def bark(self):
        print(f"{self.name.upper()} says woof woof! I'm {self.age} years old!")

dog_1 = Dog("Jack", 3)
dog_2 = Dog("Thatcher", 5)

# Call the bark method
dog_1.bark()  # JACK says woof woof! I'm 3 years old!
dog_2.bark()  # THATCHER says woof woof! I'm 5 years old!
```

As you can see, we create two dog objects using the `Dog` class. When initializing `dog_1`, the string `Jack` and the number `3` are passed, which sets the `name` and `age` attributes for that instance. And `dog_2` is initialized with the string `Thatcher` and number `5` as its `name` and `age`, respectively.

Then when you call the `.bark()` method on `dog_1` and `dog_2`, you can see how both outputs differ, and use the unique `name` and `age` attributes you passed in when creating each object.

In summary, the difference between a class and an object is that a class is the template or the blueprint, and an object is what is created using that template.

Also, a class defines what data and behavior the object should have, and an object holds the actual data and uses that behavior. You write a class once, and you can make many objects from it, each with different data.

---

# What Are Methods and Attributes, and How Do They Work?

In the last lesson, you learned about classes and how they act as blueprints for creating objects.

Here, we will dive deeper into attributes and methods.

Let's take a closer look at attributes first, then methods.

Attributes are variables that belong to an object, so they hold data. There are two kinds of attributes: instance attributes and class attributes.

Instance attributes are unique to each object created from a class, and you usually set them with the `__init__` method. Class attributes, on the other hand, belong to the class itself and are shared by all instances of that class.

To access an attribute, you use dot notation.

Here are examples of both instance and class attributes, and how to access them from objects:

```python
class Dog:
    species = "French Bulldog" # Class attribute

    def __init__(self, name):
        self.name = name # Instance attribute

print(Dog.species) # French Bulldog

dog1 = Dog("Jack")
print(dog1.name)    # Jack
print(dog1.species) # French Bulldog

dog2 = Dog("Tom")
print(dog2.name)    # Tom
print(dog2.species) # French Bulldog
```

Note that you can access class attributes directly from the class itself, but you need to create an object and pass it data first before you can access instance attributes.

Cars are another good example, since all cars have a model and color:

```python
class Car:
    def __init__(self, color, model):
        self.color = color
        self.model = model

car_1 = Car("red", "Toyota Corolla")
car_2 = Car("green", "Lamborghini Revuelto")

print(car_1.model) # Toyota Corolla
print(car_2.model) # Lamborghini Revuelto

print(car_1.color) # red
print(car_2.color) # green
```

Methods are functions defined inside a class. With them, any object defined from a class can perform actions that operate on or modify its own data. You also access a method with dot notation.

For example, dogs can bark. So we can have a `bark` method in the `Dog` class like you saw in a previous lesson:

```python
class Dog:
   species = "French Bulldog"

   def __init__(self, name):
     self.name = name

   def bark(self):
       return f"{self.name} says woof woof!"

jack = Dog("Jack")
jill = Dog("Jill")

print(jack.bark()) # Jack says woof woof!
print(jill.bark()) # Jill says woof woof!
```

A `Car` class can also have a `describe` method:

```python
class Car:
    def __init__(self, color, model):
        self.color = color  # Instance attribute
        self.model = model  # Instance attribute

    def describe(self):
        return f"This car is a {self.color} {self.model}"

car_1 = Car("red", "Toyota Corolla")
car_2 = Car("green", "Lamborghini Revuelto")

print(car_1.describe()) # This car is a red Toyota Corolla
print(car_2.describe()) # This car is a green Lamborghini Revuelto
```

---

# What Are Special Methods and What Are They Used For?

Special methods in Python, also known as "magic methods" or "dunder methods", are special Python methods that start and end with double underscores (`__`). The word "dunder" itself comes from double underscores (**d** for double, **under** for underscores).

You've probably used special methods already without knowing it. Every time you write something like `3 + 4`, Python quietly runs `3.__add__(4)` under the hood. That's a special method in action. So while you *can* call special methods directly, you rarely do. Something like `3 + 4` is much clearer and easier to read than calling `3.__add__(4)` yourself.

Apart from `__add__`, `__init__()` is another special method you'll see and use the most, as it's a class initializer. There are also others like `__len__()` and `__str__()`.

Think of special methods as the directors of the activities between a person programming and the Python language interpreter itself.

Remember, you don't need to call special methods directly. Instead, Python automatically calls them when certain actions happen. These operations include:

* **Arithmetic operations like addition, subtraction, multiplication, division, and others**. For addition, `__add__()` is called, `__sub__()` for subtraction, `__mul__()` for multiplication, and `__truediv__()` for division.
* **String operations like concatenation, repetition, formatting, and conversion to text**. `__add__()` is called for concatenation, `__mul__()` for repetition, `__format__()` for formatting, `__str__()` and `__repr__()` for text conversion, and so on.
* **Comparison operations like equality, less-than, greater-than, and others**. `__eq__()` is called for equality checks, `__lt__()` for less-than, `__gt__()` for greater-than, and so on.
* **Iteration operations like making an object iterable and advancing through items**. `__iter__()` is called to return an iterator and  `__next__()` to fetch the next item.

Normally, Python data types like strings and numbers already know how to add things, do concatenation, compare for equality, be used in loops, and others.

But when you create your own class, Python won't know how to handle things automatically.

This is where special methods come in — they let you customize Python's built-in behavior.

Let's say you want to get the number of pages in book objects created with the class below, or compare them and get a readable string of the objects. Here's what happens without special methods:

```python
class Book:
   def __init__(self, title, pages):
       self.title = title
       self.pages = pages

book1 = Book("Built Wealth Like a Boss", 420)
book2 = Book("Be Your Own Start", 420)

print(len(book1)) # TypeError: object of type 'Book' has no len()
print(str(book1)) # <__main__.Book object at 0x102ed2900>
print(book1 == book2) # False even though they have the same number of pages
```

In the example:

* `len(book1)` failed because Python doesn't know how to get the length of your book object without `__len__()`
* `str(book1)` printed something like `<__main__.Book object at 0x102ed2900>` because that's the default representation when you don't use `__str__()`
* `book1 == book2` resulted in `False` because Python just checks if both objects are the same in memory, not by content.

Here's how you can define your own `__len__()`, `__str__()`, and `__eq__()` special methods to make working with objects created from the `Book` class easier:

```python
class Book:
   def __init__(self, title, pages):
       self.title = title
       self.pages = pages

   def __len__(self):
       return self.pages

   def __str__(self):
       return f"'{self.title}' has {self.pages} pages"

   def __eq__(self, other):
       return self.pages == other.pages
  
book1 = Book("Built Wealth Like a Boss", 420)
book2 = Book("Be Your Own Start", 420)

print(len(book1)) # 420
print(len(book2)) # 420
print(str(book1)) # 'Built Wealth Like a Boss' has 420 pages
print(str(book2)) # 'Be Your Own Start' has 420 pages
print(book1 == book2) # True
```

Another example is a shopping cart where you do the following:

* Add items to the cart
* Remove items from the cart
* Get the number of items in the cart
* Check what items are in the cart
* Check if a specific item is in the cart
* Return or display an item at a specific index in the cart

While you might have a method that adds items to the cart and removes certain items from the cart, you can create special methods for all the other functionality:

* `__len__()` to get the length of the items in the cart
* `__iter__()` to loop through the items in the cart so you can see them
* `__contains__()` to check if a specific item is in the cart
* `__getitem__()` to return or display an item at a specific index in the cart

Here's an example of a `Cart` class with these user-defined methods and special methods:

```python
class Cart:
   def __init__(self):
       self.items = []

   def add(self, item):
       self.items.append(item)

   def remove(self, item):
       if item in self.items:
           self.items.remove(item)
       else:
           print(f'{item} is not in cart')

   def list_items(self):
       return self.items

   def __len__(self):
       return len(self.items)

   def __getitem__(self, index):
       return self.items[index]

   def __contains__(self, item):
       return item in self.items

   def __iter__(self):
       return iter(self.items)
```

And here's how you can use them:

```python
cart = Cart()
cart.add('Laptop')
cart.add('Wireless mouse')
cart.add('Ergo keyboard')
cart.add('Monitor')

for item in cart:
   print(item, end=' ') # Laptop Wireless mouse Ergo keyboard Monitor

print(len(cart)) # 4
print(cart[3]) # Monitor

print('Monitor' in cart) # True
print('banana' in cart) # False

cart.remove('Ergo keyboard')

print(cart.list_items()) # ['Laptop', 'Wireless mouse', 'Monitor']

cart.remove('banana') # banana is not in cart
```

And those are a few ways you'll use special methods in Python in the real-world.

---

# How to Handle Object Attributes Dynamically?

In a previous lesson, you learned about attributes being the variables that belong to an object. That means they hold data that describes the state or behavior of the object.

For example, a car would normally have a brand and model. The brand and model could make attributes for a `Car` class:

```python
class Car: 
    def __init__(self, brand, model): 
        self.brand = brand 
        self.model = model 

my_car = Car('Lamborghini', 'Gallardo') 
print(my_car.brand) # Lamborghini 
print(my_car.model) # Gallardo
```

But sometimes, you might not know which attributes you need until your program is running. Imagine you're writing a script that receives attribute names from a user or a configuration file. Those are not attributes you can hardcode ahead of time.

That's where handling attributes dynamically comes in. This way, you can access, modify, check, or even delete attributes using their names as variables, and not as fixed names in your code. This gives your program the flexibility to respond to different data or user input on the fly.

Python gives you four handy built-in functions to dynamically work with object attributes. They are `getattr()`, `setattr()`, `hasattr()`, and `delattr()`.

They let you access, create, check, and remove attributes using variable names. Let's take a look at each one in action.

`getattr()` makes it possible to read an attribute from an object when you don't know its name until runtime. If the attribute doesn't exist, it raises an `AttributeError`, unless you provide a default value.

To use it, you pass in the object, attribute name, and an optional default value:

```python
getattr(object, attribute_name, default_value)
```

Here's an example:

```python
class Person: 
    def __init__(self, name, age): 
        self.name = name 
        self.age = age 

person = Person('John Doe', 30) 
 
print(getattr(person, 'name')) # John Doe 
print(getattr(person, 'age')) # 30 
print(getattr(person, 'city', 'Milano')) # Milano
```

In the example above, `Milano` is a default value because `city` doesn't exist in the `Person` class.

As we said earlier, the real power of `getattr()` is apparent when the attribute name comes from a variable, such as from user input or some file.

In that case, you can't use the regular `object.attribute_name` syntax because the attribute name is not fixed.

```python
class Person: 
    def __init__(self, name, age): 
        self.name = name 
        self.age = age 

person = Person('John Doe', 30)

attr_name = input('Enter the attribute you want to see: ')
print(getattr(person, attr_name, 'Attribute not found'))
```

In this case, if the user types in `name`, they see `John Doe`, and if they type in `age`, they see `30`. And if they type something that doesn't exist in the class like `email`, they see `Attribute not found`.

This is exactly where dynamic attribute handling shines. It lets your code respond to input and data it hasn't seen before.

In addition, you might want to look through all the attributes an object has, not just the ones you already know. The built-in `dir()` function lets you do that. It returns a list of all attribute names on the object. Here's how to use it:

```python
class Person: 
    def __init__(self, name, age): 
        self.name = name 
        self.age = age 

person = Person('John Doe', 30)

# Loop through all attributes of the person object with dir() function
for attr in dir(person):
    # Ignore dunder methods like __init__ or __str__ and regular methods
    if not attr.startswith('__') and not callable(getattr(person, attr)): 
        value = getattr(person, attr)
        print(f'{attr}: {value}')

# Output
# age: 30
# name: John Doe
```

In the loop above, `callable()` is a built-in function that returns `True` if the object passed to it can be called like a function or method, and `False` otherwise. By checking `not callable(getattr(person, attr))`, the loop skips over methods and only prints the data attributes like `name` and `age`.

The `setattr()` function lets you create a new attribute or update an existing one dynamically. The syntax looks like this:

```python
setattr(object, attribute_name, value)
```

Here's an example that sets config attributes based on data from some config or environment variable file:

```python
class Configuration:
    pass

# Data loaded at runtime (like from a config or env file)
settings_data = {
    'server_url': 'https://api.example.com',
    'timeout_sec': 30,
    'max_retries': 5
}

config_obj = Configuration()

# Dynamically set attributes using dictionary keys and values
for attr_name, attr_value in settings_data.items():
    setattr(config_obj, attr_name, attr_value)

print(config_obj.server_url) # https://api.example.com
print(config_obj.timeout_sec) # 30
```

There is also `hasattr()`. Before you do something with an attribute or delete it, it's a good practice to check if it exists. That's what `hasattr()` lets you do. It checks if an attribute exists and returns `True` or `False` based on the result.

Here's the basic syntax:

```python
hasattr(object, attribute_name)
```

And here's an example that dynamically checks for the existence of attributes in a `Product` class instance:

```python
class Product:
    def __init__(self, name, price):
        self.name = name
        self.price = price

product_a = Product('T-Shirt', 25)

required_attributes = ['name', 'price', 'inventory_id']

for attr in required_attributes:
    if not hasattr(product_a, attr):
        print(f"ERROR: Product is missing the required attribute: '{attr}'")
    else:
        # Access the attributes dynamically once their existence is confirmed
        print(f'{attr}: {getattr(product_a, attr)}')

# Output:
# name: T-Shirt
# price: 25
# ERROR: Product is missing the required attribute: 'inventory_id'
```

The ERROR output occurred because `inventory_id` is missing from the `Product` class and its instance.

Lastly, `delattr()` lets you remove an attribute dynamically:

```python
delattr(object, attribute_name)
```

For example, imagine an object has been fully processed, then you decide to clean up any sensitive or temporary attributes that might exist before saving the final version. After that, you can use `dir()` to loop through the remaining attributes:

```python
class UserSession:
    def __init__(self, user_id, token):
        self.user_id = user_id
        self.auth_token = token # sensitive
        self.temp_counter = 0 # temporary

session = UserSession(101, 'a1b2c3d4e5')

# List of attributes to remove dynamically before "saving" the session
attributes_to_clean = ['auth_token', 'temp_counter']

# Dynamically remove specified attributes
for attr in attributes_to_clean:
    if hasattr(session, attr):
        delattr(session, attr)
        print(f'Removed attribute: {attr}')

print('\nFinal attributes remaining:')

# Loop through the remaining attributes with dir()
for attr in dir(session):
    # Ignore dunder methods like __init__ or __str__ and regular methods
    if not attr.startswith('__') and not callable(getattr(session, attr)):
        print(f' - {attr}: {getattr(session, attr)}')

# Output:
# Removed attribute: auth_token
# Removed attribute: temp_counter

# Final attributes remaining:
#  - user_id: 101
```

And that's how you can handle attributes dynamically!

---

# What is Object-Oriented Programming, and How Does Encapsulation Work?

Object-oriented programming, also known as OOP, is a programming style in which developers treat everything in their code like a real-world object.

A class is like a blueprint for creating objects. Every single object created from a class has attributes that define data and methods that define the behaviors of the objects.

In a previous lesson, you learned how to create classes. Here's a reminder of the syntax:

```python
class ClassName:
   def __init__(self, parameters):
       attribute = value

   def method_name(self):
       # method logic
```

Here's an example of a class that uses the `__init__` special method to initialize the brand and color attributes whenever an object is created using the class:

```python
class Car:
   def __init__(self, brand, color):
       self.brand = brand
       self.color = color

# create two objects from the Car class
car1 = Car('Toyota', 'red')
car2 = Car('Lambo', 'green')

print('Car 1 Brand:', car1.brand) # Car 1 Brand: Toyota
print('Car 1 Color:', car1.color) # Car 1 Color: red

print('Car 2 Brand:', car2.brand) # Car 2 Brand: Lambo
print('Car 2 Color:', car2.color) # Car 2 Color: green
```

Object-oriented programming has four key principles that help you organize and manage code effectively. They are encapsulation, inheritance, polymorphism, and abstraction.

The rest of this lesson will focus on how encapsulation works.

Encapsulation is the bundling of the attributes and methods of an object into a single unit, the class.

With encapsulation, you can hide the internal state of the object behind a simple set of public methods and attributes that act like doors. Behind those doors are private attributes and methods that control how the data changes and who can see it.

Let's say you want to track a wallet balance. You want to allow people to deposit or withdraw money from the wallet, but no one should be able to tamper with the balance directly.

In that case, you can make `deposit()` and `withdraw()` public methods, and you hide the balance under the `_balance` attribute:

```python
class Wallet:
   def __init__(self, balance):
       self._balance = balance # For internal use by convention

   def deposit(self, amount):
       if amount > 0:
           self._balance += amount # Add to the balance safely

   def withdraw(self, amount):
       if 0 < amount <= self._balance:
           self._balance -= amount # Remove from the balance safely
```

By convention, prefixing attribute and methods with a single underscore means they are meant for internal use. No one should directly access them from outside the class since it defies the principles of encapsulation, which can lead to bugs.

While a single underscore prefix is just a convention, prefixing attributes and methods with a double underscore effectively prevents them to be accessed from the outside of their class, making those attributes and methods private.

```python
class Wallet:
   def __init__(self, balance):
       self.__balance = balance # Private attribute

   def deposit(self, amount):
       if amount > 0:
           self.__balance += amount # Add to the balance safely

   def withdraw(self, amount):
       if 0 < amount <= self.__balance:
           self.__balance -= amount # Remove from the balance safely

account = Wallet(500)
print(account.__balance) # AttributeError: 'Wallet' object has no attribute '__balance'
```

To get the current value of `__balance`, you can define a `get_balance` method. For example:

```python
class Wallet:
   def __init__(self, balance):
       self.__balance = balance

   def deposit(self, amount):
       if amount > 0:
           self.__balance += amount

   def withdraw(self, amount):
       if 0 < amount <= self.__balance:
           self.__balance -= amount
  
   def get_balance(self):
       return self.__balance


acct_one = Wallet(100)
acct_one.deposit(50)
print(acct_one.get_balance()) # 150

acct_two = Wallet(450)
acct_two.withdraw(28)
print(acct_two.get_balance()) # 422

acct_two.deposit(150)
print(acct_two.get_balance()) # 572
```

You can also define a private `__validate` method to check if every deposit or withdrawal amount is a positive number:

```python
class Wallet:
   def __init__(self):
       self.__balance = 0

   def __validate(self, amount):
       if amount < 0:
           raise ValueError('Amount must be positive')

   def deposit(self, amount):
       self.__validate(amount)
       self.__balance += amount

   def withdraw(self, amount):
       self.__validate(amount)
       if amount > self.__balance:
           raise ValueError('Insufficient funds')
       self.__balance -= amount

   def get_balance(self):
       return self.__balance

acct_one = Wallet()
acct_one.deposit(3)
print(acct_one.get_balance()) # 3

acct_one.deposit(50)
print(acct_one.get_balance()) # 53

acct_one.deposit(-4)  # ValueError: Amount must be positive
acct_one.withdraw(-8) # ValueError: Amount must be positive
acct_one.withdraw(58) # ValueError: Insufficient funds
```

As you can see, the `__validate` method is private, and runs behind the scenes in the `deposit()` and `withdraw()` public methods to make sure the amount is always valid.

In a coming lesson, you will learn more about how attributes prefixed with a double underscore works.

In summary, encapsulation locks down internal data behind clear public methods. That's how you keep your classes safe from tampering and centralize validation in one place. You can update or extend your code freely, knowing that outside code only touches the interfaces you expose.

---

# What are Getters and Setters

Getters and setters are methods that let you control how the attributes of a class are accessed and modified. With getters you retrieve a value, and with setters you set a value.

These actions are done through what's known as properties. They are what connect getters and setters, and allow access to data.

Properties act like attributes but behave like methods under the hood. Think of them as data you define like methods, but work like attributes. This means you can access properties with dot notation instead of parentheses or round brackets.

The main thing properties do is that they run extra logic behind the scenes when you get, set, or delete values with them. This makes them the perfect choice when you want to access or manipulate data within objects.

So why use properties for that instead of methods? It's mostly about readability and convention. They make your code cleaner and easier to read.

When you use a method, you always have to call it with parentheses. But with a property, you can access it just like a normal attribute using dot notation. That makes your code look simple even when it is doing extra work behind the scenes.

For example, you might want to calculate a value or check that a new value is valid before saving it. Instead of calling a method for that, you can use an attribute-like way to do that.

In Python, a decorator is a function that modifies the functionalities of other functions, or classes, without changing their original code.

While it is possible to create custom decorators, this is beyond the scope of this lesson. Just know that to create a property, you define a method and place the `@property` decorator above it. This turns the method into a property, so it can be accessed like an attribute while internally calling the decorated method.

That takes us to getters. Here's how to create one with the `@property` decorator:

```python
class Circle:
    def __init__(self, radius):
        self._radius = radius

    @property
    def radius(self): # A getter to get the radius
        return self._radius
  
    @property
    def area(self):  # A getter to calculate area
        return 3.14 * (self._radius ** 2)

my_circle = Circle(3)

print(my_circle.radius) # 3
print(my_circle.area) # 28.26
```

This example gets a radius and the area of a circle.

Notice how we used `_radius` instead of radius inside the class. The underscore is a common Python convention to show that an attribute is meant to be private. In other words, it signifies that it's for internal use and should not be accessed directly from outside the class.

To make a setter to create the radius, for example, you have to define another method with the same name and use `@<property_name>.setter` above it:

Using `self.radius` inside `__init__` ensures the setter runs during object creation, so invalid radius values are caught immediately.

```python
class Circle:
    def __init__(self, radius):
        self.radius = radius # Calling the setter

    @property
    def radius(self):  # A getter to get the radius
        return self._radius

    @radius.setter
    def radius(self, value):  # A setter to set the radius
        if value <= 0:
            raise ValueError('Radius must be positive')
        self._radius = value

my_circle = Circle(3)
print('Initial radius:', my_circle.radius) # Initial radius: 3

my_circle.radius = 8
print('After modifying the radius:', my_circle.radius) # After modifying the radius: 8
```

In this example, the radius setter is not just setting the radius for the circle, it's also running a validation that makes sure the radius is not a negative number.

Once you define getters and setters, Python automatically calls them under the hood whenever you use normal attribute syntax:

```python
my_circle.radius # This will call the getter
my_circle.radius = 4 # This will call the setter
```

Note that inside the setter, you cannot use same name of the property when assigning a new value. That's because `self.radius = value` will call the setter within the setter method itself, leading to infinite recursion and a `RecursionError`. So you must always use the underscore-prefixed form `self._radius = value`.

Just like you can control how an attribute is accessed through getter and how it is modified with setter, you can also control how it is deleted using a deleter.

A deleter runs custom logic when you use the del statement on a property. To create one, you use the `@<property_name>.deleter` decorator:

```python
class Circle:
    def __init__(self, radius):
        self.radius = radius

    # Getter
    @property
    def radius(self):
        return self._radius

    # Setter
    @radius.setter
    def radius(self, value):
        if value <= 0:
            raise ValueError("Radius must be positive")
        self._radius = value

    # Deleter
    @radius.deleter
    def radius(self):
        print("Deleting radius...")
        del self._radius
```

Here's how the deleter can be put to use:

```python
# Create circle object with a radius
my_circle = Circle(33)
print("Initial radius:", my_circle.radius)  # 33

# Delete the radius
# This calls the deleter
del my_circle.radius # Deleting radius...
print("Radius deleted!") # Radius deleted!

# Try to access radius after deletion
try:
    print(my_circle.radius)
except AttributeError as e:
    print("Error:", e) # Error: 'Circle' object has no attribute '_radius'
```

The takeaway from this is that:

* Getters let you retrieve a value or even compute a value on the fly.
* Setters let you modify the values safely by running checks before assignment.
* Properties are what tie these getters and setters together so you can write logic while still using dot notation.
* Deleters let you define what happens when an attribute is deleted.

---

# What Is Inheritance and How Does It Promote Code Reuse?

Inheritance is the next key concept of object-oriented programming (OOP) we'll cover.

Let's take a deeper look at this concept and how it lets you write reusable code.

With inheritance, a subclass (or child class) can use the attributes and methods of a base class (or parent class). This allows you to reuse code, create clear class hierarchies, and customize behavior without rewriting everything. You can customize by extending existing methods or overriding them in the child class.

Here's the basic syntax for inheritance:

```python
class Parent:
    # Parent attributes and methods

class Child(Parent):
    # Child inherits, extends, and/or overrides where necessary
```

For the `Child` class to inherit from the `Parent` class, you have to pass the Parent to the Child.

This style is called single inheritance, since a child class inherits from exactly one parent class.

Here's an example:

```python
class Animal:
    def __init__(self, name):
        self.name = name

    def sound(self):
        return f'{self.name} makes a sound'

class Dog(Animal):
    bark = 'woof! woof!! woof!!!'

jack = Dog('Jack')
print(jack.sound())  # Jack makes a sound
print(jack.bark)  # woof! woof!! woof!!!
```

You can see that we're able to reuse the `self.name` attribute and the `sound()` method from the parent `Animal` class in the child `Dog` class.

Let's override the `sound()` method from the parent `Animal` class in the child `Dog` class so we can have `sound()` use the `bark` class variable:

```python
class Animal:
    def __init__(self, name):
        self.name = name

    def sound(self):
        return f'{self.name} makes a sound.'

class Dog(Animal):
    bark = 'woof! woof!! woof!!!'

    # Override sound() to use bark class variable
    def sound(self):
        return f'{self.name} barks {self.bark}'

jack = Dog('Jack')
print(jack.sound())  # Jack barks woof! woof!! woof!!!
```

If you want to keep the return value of `sound()` and add the bark class variable later, you can extend `sound()` by using the `super()` function:

```python
class Animal:
    def __init__(self, name):
        self.name = name

    def sound(self):
        return f'{self.name} makes a sound'

class Dog(Animal):
    bark = 'woof! woof!! woof!!!'

    # Call Animal.sound(), then append bark
    def sound(self):
        base = super().sound()
        return f'{base}, then {self.name} barks {self.bark}'

jack = Dog('Jack')
print(jack.sound())  # Jack makes a sound, then Jack barks woof! woof!! woof!!!
```

In this example, `base` is the result of calling the `sound()` method from the `Animal` class, and then we append the `Dog` class's specific sound to it. This way, you can extend the functionality of the parent `Animal` class while still keeping its original behavior.

There's also multiple inheritance, where a child class can inherit from more than one parent class.

Here's the basic syntax of multiple inheritance:

```python
class Parent:
    # Attributes and methods for Parent

class Child:
    # Attributes and methods for Child

class GrandChild(Parent, Child):
    # GrandChild inherits from both Parent and Child
    # GrandChild can combine or override behavior from each
```

A simple way to demonstrate multiple inheritance is with a frog, which can both walk on land and swim in water:

```python
class Walker:
    def walk(self):
        return 'I can walk on land'

class Swimmer:
    def swim(self):
        return 'I can swim in water'

# Amphibian inherits from both Walker and Swimmer
class Amphibian(Walker, Swimmer):
    def __init__(self, name):
        self.name = name

    def introduce(self):
        return f"I'm {self.name} the frog. {self.walk()} and {self.swim()}."

frog = Amphibian('Freddy')
print(frog.introduce())
# Output: I'm Freddy the frog. I can walk on land and I can swim in water.
```

---

# What is Name Mangling and How Does it Work?

In a previous lesson, you learned about prefixing attributes with a single underscore and a double underscore.

To remind you of the difference between them, a single underscore is a convention that means the attribute is meant for internal use in the class and should not be directly accessed from outside the class. Double underscore, on the other hand, prevents that attribute from being accessed directly from outside the class.

Here's an example that demonstrates how the two work:

```python
class Example:
    def __init__(self):
        self._internal = 'I can be accessed from outside the class, but should not'
        self.__private = 'You cannot access me directly from outside the class'

obj = Example()

print(obj._internal) # I can be accessed from outside the class, but should not
print(obj.__private)  # AttributeError: 'Example' object has no attribute '__private'
```

Prefixing an attribute with a double underscore triggers Python's name mangling process, in which Python internally renames the attribute by adding an underscore and the class name as a prefix, turning `__attribute` into `_ClassName__attribute`.

To see this in action, you create an instance of the class and use the `__dict__` special attribute of that instance, which is a dictionary containing the object's attributes:

```python
class Example:
    def __init__(self, internal, private):
        self._internal = internal
        self.__private = private

example1 = Example(
    'I can be accessed from outside the class, but should not',
    'I cannot be accessed directly from outside the class'
)

print(example1.__dict__)
```

The result would be:

```python
{
  '_internal': 'I can be accessed from outside the class, but should not',
  '_Example__private': 'I cannot be accessed directly from outside the class'
}
```

As you can see, the `__private` attribute is stored as `_Example__private`. This means you can still access that attribute outside the class this way:

```python
class Example:
    def __init__(self, internal, private):
        self._internal = internal
        self.__private = private

example1 = Example(
    'I can be accessed from outside the class, but should not',
    'I cannot be accessed directly from outside the class'
)
example2 = Example(
    'I should not be accessed from outside the class',
    'But I can be accessed from outside the class with name mangling'
)

print(example1._Example__private) # I cannot be accessed directly from outside the class
print(example2._Example__private) # But I can be accessed from outside the class with name mangling
```

So, why does Python do name mangling?

The main purpose of name mangling is to prevent accidental attribute and method overriding when you use inheritance. Here's an example that makes that clear:

```python
class Parent:
    def __init__(self):
        self.__data = 'Parent data'

class Child(Parent):
    def __init__(self):
        super().__init__()
        self.__data = 'Child data'

c = Child()
print(c.__dict__) # {'_Parent__data': 'Parent data', '_Child__data': 'Child data'}
```

You can see that both the `Parent` class and the `Child` that inherits from it have their separate `_class__data` attributes. This is made possible with name mangling. Otherwise, the `Child` would have overwritten the Parent data by accident.

Here's what would have happened without allowing Python to do the name mangling, that is if you don't prefix the attributes in both classes with double underscore:

```python
class Parent:
   def __init__(self):
       self.data = 'Parent data'

class Child(Parent):
   def __init__(self):
       super().__init__()
       self.data = 'Child data'

c = Child()
print(c.__dict__)  # {'data': 'Child data'}
```

So, which should you use to prefix attributes between single underscore (`_`) and double underscore (`__`)? It depends. If an attribute is only meant for internal use within the class, stick with a single underscore.

But if you're working with a class that will be inherited, you should use a double underscore so the attribute from the parent doesn't get overridden.

---

# What Is Polymorphism and How Does It Promote Code Reuse?

Polymorphism is the next key concept of object-oriented programming (OOP) we will talk about.

With polymorphism, you have access to an interface where you can interact with many objects of the same kind.

Let's take a deeper look at polymorphism and how it lets you reuse code.

Polymorphism allows methods in different classes to share the same name but perform different tasks. You call the same method name on different objects, and each responds in its own way.

Here's the basic example of polymorphism:

```python
class A:
   def action(self): ...

class B:
   def action(self): ...

class C:
   def action(self): ...

Class().method()  # Works for A, B, or C
```

Here's an example using different animal sounds to depict polymorphism:

```python
class Cat:
   def speak(self):
       return "A cat meow"

class Bird:
   def speak(self):
       return "A bird tweet"
  
class Monkey:
   def speak(self):
       return "A monkey ooh ooh aah aah ooh ooh aah aah"

def animal_sound(animal):
   print(animal.speak())

animal_sound(Cat())
animal_sound(Bird())
animal_sound(Monkey())
```

In this example, `animal_sound()` is a function that takes any object with a `speak()` method.

When you pass in a `Cat`, `Bird`, or `Monkey`, it calls the `speak()` method of the object and prints the result. Because each class defines `speak()` differently, you get different outputs from the same function. That's polymorphism in action.

Here's another example, this time with instances and an attribute:

```python
class Twitter:
   def __init__(self, content):
       self.content = content

   def post(self):
       return f"🐦 Tweet: '{self.content}' (280 chars max)"

class Instagram:
   def __init__(self, content):
       self.content = content

   def post(self):
       return f"📸 Instagram Post: '{self.content}' + ✨ filters"

class LinkedIn:
   def __init__(self, content):
       self.content = content

   def post(self):
       return f"💼 LinkedIn Article: '{self.content}' (Professional Mode)"

def start(social_media):
   print(social_media.post())  # Calls .post() on any object

# Instances
tweet = Twitter('Just learned Python polymorphism!')
photo = Instagram('Sunset vibes 🌅')
article = LinkedIn('Why OOP matters in 2024')

# The polymorphic calls - same function, different outputs
start(tweet) # 🐦 Tweet: 'Just learned Python polymorphism!' (280 chars max)
start(photo) # 📸 Instagram Post: 'Sunset vibes 🌅' + ✨ filters
start(article) # 💼 LinkedIn Article: 'Why OOP matters in 2024' (Professional Mode)
```

There's also a kind of polymorphism called **inheritance-based polymorphism**.

In inheritance-based polymorphism, a parent class defines a method, and multiple child classes override that method in their own way. You can then call the same method on any child object, and it behaves differently depending on which child class it is.

Here's an example:

```python
class Animal:
   def speak(self):
       return 'Some generic sound'

class Cat(Animal):
   def speak(self):
       return 'A cat meow'

class Dog(Animal):
   def speak(self):
       return 'A dog barks woof woof'

class Monkey(Animal):
   def speak(self):
       return 'A monkey ooh ooh aah aah ooh ooh aah aah'
  
print(Cat().speak()) # A cat meow
print(Dog().speak()) # A dog barks woof woof
print(Monkey().speak()) # A monkey ooh ooh aah aah ooh ooh aah aah
print(Animal().speak()) # Some generic sound
```

You can see that each child class of the parent `Animal` class overrides the `speak()` method to provide its own implementation. So when you call the `speak()` method on an instance of each subclass, it returns the specific sound associated with that animal.

You can also take things further and do the calling in a list, then loop through the list to display what the `speak()` method returns for each:

```python
animals = [Cat(), Dog(), Monkey()]

for animal in animals:
   print(animal.speak())

# Output:
# A cat meow
# A dog barks woof woof
# A monkey ooh ooh aah aah ooh ooh aah aah
```

---

## Module Review Component

# Classes and Objects Review

Python Classes and Objects
--------------------------

* **Class Definition**: A class is a blueprint for creating objects. It defines the behavior an object will have through its attributes and methods. Here is a basic example of a class definition in Python:

```python
class Dog:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def bark(self):
        print(f'{self.name.upper()} says woof woof!')
```

* **Creating Objects**: Objects are instances of a class. They are created by calling the class with the necessary arguments.

```python
dog1 = Dog('Jack', 3)
dog2 = Dog('Thatcher', 5)

dog1.bark()  # JACK says woof woof!
dog2.bark()  # THATCHER says woof woof!
```

* **Calling Methods on Objects**: You can call methods on objects to perform actions or retrieve information.

```python
object_name1.method_name()
object_name2.method_name()
```

* **Difference Between Class and Object**: A class is a reusable template, while an object is a specific instance of that class with actual data.

Attributes
----------

* **Instance Attributes**: Defined in `__init__()` using `self`, and unique to each object.
* **Class Attributes**: Defined directly inside the class and shared by all instances.

```python
class Dog:
    species = 'French Bulldog'  # Class attribute

    def __init__(self, name):
        self.name = name  # Instance attribute

print(Dog.species) # French Bulldog

jack = Dog('Jack')
print(jack.name)     # Jack
print(jack.species)  # French Bulldog
```

Methods
-------

* **Methods**: Functions defined inside a class that operate on the object's attributes.

```python
class Car:
    def __init__(self, color, model):
        self.color = color
        self.model = model

    def describe(self):
        return f'This car is a {self.color} {self.model}'

my_car_1 = Car('red', 'Tesla Model S')
print(my_car_1.describe())  # This car is a red Tesla Model S
```

* **Accessing Methods**: Call methods on objects using the dot notation. Here is an example of calling the `describe` method on two different car objects:

```python
class Car:
    def __init__(self, color, model):
        self.color = color  
        self.model = model  

    def describe(self):
        return f'This car is a {self.color} {self.model}'

my_car_1 = Car('red', 'Tesla Model S')
my_car_2 = Car('green', 'Lamborghini Revuelto')

print(my_car_1.describe()) # Calling method using the dot notation

print(my_car_2.describe()) # Calling method using the dot notation
```

Dunder (Magic) Methods
----------------------

* **Definition**: Special methods that start and end with a double underscore (e.g., `__init__`, `__len__`, `__str__`, `__eq__`). Python uses them internally for built-in operations.

```python
class Book:
    def __init__(self, title, pages):
        self.title = title
        self.pages = pages

    def __len__(self):
        return self.pages

    def __str__(self):
        return f"'{self.title}' has {self.pages} pages"

    def __eq__(self, other):
        return self.pages == other.pages

book1 = Book('Built Wealth Like a Boss', 420)
print(len(book1))        # 420
print(str(book1))        # 'Built Wealth Like a Boss' has 420 pages
```

* **Calling dunder methods indirectly**: You don't need to call dunder methods directly. Instead, Python automatically calls them when certain actions happen. These operations include:

  + **arithmetic operations like addition, subtraction, multiplication, division, and others**. In addition, `__add__()` is called, `__sub__()` for subtraction, `__mul__()` for multiplication, and `__truediv__()` for division.
  + **string operations like concatenation, repetition, formatting, and conversion to text**. `__add__()` is called for concatenation, `__mul__()` for repetition, `__format__()` for formatting, `__str__()` and `__repr__()` for text conversion, and so on.
  + **comparison operations like equality, less-than, greater-than, and others**. `__eq__()` is called for equality checks, `__lt__()` for less-than, `__gt__()` for greater-than, and so on.
  + **iteration operations like making an object iterable and advancing through items**. `__iter__()` is called to return an iterator and  `__next__()` to fetch the next item.

Real World Example: Shopping Cart
---------------------------------

* **Cart Class with Dunder Methods**: Allows adding, removing, iterating, and checking contents with built-in behavior.

```python
class Cart:
    def __init__(self):
        self.items = []

    def add(self, item):
        self.items.append(item)

    def remove(self, item):
        if item in self.items:
            self.items.remove(item)
        else:
            print(f'{item} is not in cart')

    def list_items(self):
        return self.items

    def __len__(self):
        return len(self.items)

    def __getitem__(self, index):
        return self.items[index]

    def __contains__(self, item):
        return item in self.items

    def __iter__(self):
        return iter(self.items)

cart = Cart()
cart.add('Laptop')
print(len(cart))        # 1
print('Laptop' in cart) # True
```

---

# Object Oriented Programming Review

What is Object-Oriented Programming?
------------------------------------

* **Object-oriented programming**: A programming style in which developers treat everything in their code like a real-world object. It is popularly called OOP. The four key principles that help you organize and manage code effectively are **encapsulation**, **inheritance**, **polymorphism**, and **abstraction**
* **Classes**: The blueprint for creating objects. Every single object created from a class has attributes that define data and methods that determine the behaviors of the objects.

What is Encapsulation?
----------------------

* **Encapsulation**: The bundling of the attributes and methods of an object into a single unit. It lets you hide the internal state of the object behind a simple set of public methods and attributes that act like doors. Behind those doors are private attributes and methods that control how the data changes and who can see it.
* **Example of Encapsulation**: If you want to track a wallet balance, you will allow deposit and withdrawal, but you won't want anyone to tamper with the wallet balance itself:

```python
class Wallet:
   def __init__(self, balance):
       self.__balance = balance # Private attribute

   def deposit(self, amount):
       if amount > 0:
           self.__balance += amount # Add to the balance safely

   def withdraw(self, amount):
       if 0 < amount <= self.__balance:
           self.__balance -= amount # Remove from the balance safely

account = Wallet(500)
print(account.__balance) # AttributeError: 'Wallet' object has no attribute '__balance'
```

* **Difference Between Prefixing Attributes with Single and Double Underscore**: Prefixing attributes and methods with a single underscore means they are meant for internal use. This is a convention, and it doesn't enforce accessing attributes from the outside. Prefixing attributes and methods with a double underscore effectively prevents them from being accessed from outside of their class.

What Are Getters and Setters?
-----------------------------

* **Getters and Setters**: Methods that let you control how the attributes of a class are accessed and modified. You retrieve values with getters and you set values with setters.
* **Properties**: They connect getters and setters, and allow access to data. They run extra logic behind the scenes when you get, set, or delete values.
* **Why Properties Instead of Methods**: Properties are used instead of methods for better readability and cleaner code. They let you access values with dot notation, like regular attributes, without parentheses.
* **Creating a Getter**: To create a getter, you use the `@property` decorator. Here's a getter that gets the radius of a circle:

```python
class Circle:
    def __init__(self, radius):
        self._radius = radius

    @property
    def radius(self): # A getter to get the radius
        return self._radius
  
    @property
    def area(self):  # A getter to calculate area
        return 3.14 * (self._radius ** 2)

my_circle = Circle(3)

print(my_circle.radius) # 3
print(my_circle.area) # 28.26
```

* **Creating a Setter**: To create the setter that will set the radius, you have to define another method with the same name and use `@<property_name>.setter` above it:

```python
class Circle:
    def __init__(self, radius):
        self._radius = radius

    @property
    def radius(self):  # A getter to get the radius
        return self._radius

    @radius.setter
    def radius(self, value):  # A setter to set the radius
        if value <= 0:
            raise ValueError('Radius must be positive')
        self._radius = value

my_circle = Circle(3)
print('Initial radius:', my_circle.radius) # Initial radius: 3

my_circle.radius = 8
print('After modifying the radius:', my_circle.radius) # After modifying the radius: 8
```

* **How Python Handles Getters and Setters**: Once you define getters and setters, Python automatically calls them under the hood whenever you use normal attribute syntax this way:

```python
my_circle.radius # This will call the getter
my_circle.radius = 4 # This will call the setter
```

When setting a value, you should not assign to the property name itself because that will cause a `RecursionError`. Use a separate internal name, often with an underscore, to store the value.

* **Deleter**: After setting and getting a value with setter and getter, you can control how it is deleted with a `deleter`. A deleter runs custom logic when you use the `del` statement on a property. To create a deleter, you use the `@<property_name>.deleter` decorator.

```python
  # Deleter
    @radius.deleter
    def radius(self):
        print("Deleting radius...")
        del self._radius
```

What Is Inheritance and How Does It Promote Code Reuse?
-------------------------------------------------------

* **Inheritance**: The process by which a child class uses the attributes and methods of a parent class. Inheritance promotes code reuse, provides clear hierarchies, and customizes behavior without rewriting everything. To implement inheritance, a child class takes in the name of a parent class:

```python
class Parent:
    # Parent attributes and methods

class Child(Parent):
    # Child inherits, extends, and/or overrides where necessary
```

* **Single and Multiple Inheritance**: When a child class inherits properties and methods from a single parent, as you can see above, the process is called **single inheritance**. When a child class inherits properties and methods from more than one parent, that is **multiple inheritance**. Here's the syntax for that:

```python
class Parent:
    # Attributes and methods for Parent

class Child:
    # Attributes and methods for Child

class GrandChild(Parent, Child):
    # GrandChild inherits from both Parent and Child
    # GrandChild can combine or override behavior from each
```

* **`super()` Function**: A function that lets you **call** a method from a parent class, when a class has a different implementation of that method, or it extends the method, without duplicating code.

What Is Polymorphism and How Does It Promote Code Reuse?
--------------------------------------------------------

* **Polymorphism**: The OOP principle that lets different classes use the same method name, but each class implements it differently when called. Here's the syntax for it:

```python
class A:
   def action(self): ...

class B:
   def action(self): ...

class C:
   def action(self): ...

Class().method()  # Works for A, B, or C
```

* **Inheritance-based polymorphism**: A parent sets up a method, and each child class twists it to their use.

What is Name Mangling and How Does it Work?
-------------------------------------------

* **Name Mangling**: A process in which Python internally renames an attribute prefixed with a double underscore by adding an underscore and the class name as a prefix, turning `__attribute` into `_ClassName__attribute`.
* **The Purpose of Name Mangling**: The main purpose of name mangling is to prevent accidental attribute and method overriding when you use inheritance. Here's a code that makes that more understandable:

```python
class Parent:
    def __init__(self):
        self.__data = 'Parent data'

class Child(Parent):
    def __init__(self):
        super().__init__()
        self.__data = 'Child data'

c = Child()
print(c.__dict__) # {'_Parent__data': 'Parent data', '_Child__data': 'Child data'}
```

What Is Abstraction and How Does It Help Keep Complex Systems Organized?
------------------------------------------------------------------------

* **Abstraction**: A programming concept in which complex implementation details of object or system are hidden and only the essential features are shown. In Python and other programming languages, abstraction simplifies complex systems by increasing reusability.
* **Example of Abstraction**: A good example of abstraction in everyday life is a car letting you just use the wheel, pedals, and shifter without knowing how the engine or brakes work.
* **How Python Implements Abstraction**: Python implements abstraction through the `abc` module. The module provides the `ABC` class (abstract base class) and the `@abstractmethod` decorator. An abstract base class (ABC) defines the common methods and properties subclasses must implement. It can't be instantiated.
* **How Abstract Method is Defined**: An abstract method is defined with `@abstractmethod` and must be overridden in subclasses, even if it has a default implementation. The basic syntax of abstraction looks like this:

```python
from abc import ABC, abstractmethod

# Define an abstract base class
class AbstractClass(ABC):
    @abstractmethod
    def abstract_method(self):
        pass

# Concrete subclass that implements the abstract method
class ConcreteClassOne(AbstractClass):
    def abstract_method(self):
        print('Implementation in ConcreteClassOne')

# Another concrete subclass
class ConcreteClassTwo(AbstractClass):
    def abstract_method(self):
        print('Implementation in ConcreteClassTwo')
```

---

# Module 10: Foundational Algorithms & Data Structures Concepts

# What Is an Algorithm and How Does Big O Notation Work?

Every computer program that runs on your device has a specific set of instructions, which are executed in a specific order to complete a task.

The task could be sorting a set of numbers, modifying an image, tracking inventory, or even running your favorite video game.

This is where algorithms come into play. An **algorithm** is a set of unambiguous instructions for solving a problem or carrying out a task.

You can think of algorithms as "recipes". When you cook, recipes list all the ingredients that you'll need, and provide step by step instructions on how to prepare a dish.

Equivalently, you can think of algorithms as "recipes" that tell computers exactly what should be done and how to do it.

Algorithms have two key characteristics:

* They cannot continue indefinitely. They must finish in a finite number of steps.
* Each step must be precise and unambiguous.

They may have zero, one, or more inputs, and generate one or more outputs.

The steps of an algorithm are independent from any programming language.

But to actually make them run on a computer, you need to implement them in a programming language, like Python or JavaScript.

If an algorithm is correct, the output for any valid input should match the expected output.

In addition to being correct, algorithms should also be efficient.

Algorithm efficiency can be measured in terms of how long they take to run and how much space they require in memory to complete the task.

Knowing an algorithm's efficiency is very important because it gives you an idea of how well it will perform as the input size grows.

For example, sorting 15 integers is not the same as sorting 1 million integers.

As the process grows in size and complexity, if the algorithm is not efficient enough to handle it, you might end up with a very slow computer program that may even crash the entire system.

That's why it's very important to develop and choose the most efficient algorithms possible.

This is where Big O notation becomes very important.

Big O notation describes the worst-case performance, or growth rate, of an algorithm as the input size increases.

The growth rate of an algorithm refers to how the resources it requires increase as the input size grows.

Big O notation focuses on the worst-case performance because this case is very important to understand how efficient the algorithm can be, even in the worst case scenario, regardless of the input.

Going back to our sorting example, sorting 1 million integers should intuitively take more time and resources than sorting 15 integers.

But how much more?

This really depends on the algorithm that you choose to sort them.

Big O notation will not give you an exact number to describe the algorithm's efficiency, but it will give you an idea of how it scales as the input size grows, based on the number of operations performed by the algorithm.

In Big O notation, we usually denote input size with the letter `n`. For example, if the input is a list, `n` would denote the number of elements in that list.

Constant factors and lower-order terms are not taken into account to find the time complexity of an algorithm based on the number of operations. That's because as the size of `n` grows, the impact of these smaller terms in the total number of operations performed will become smaller and smaller.

The term that will dominate the overall behavior of the algorithm will be the highest order term with `n`, the input size.

For example, if an algorithm performs `7n + 20` operations to be completed, the impact of the constant `20` on the final result will be smaller and smaller as `n` grows. The term `7n` will tend to dominate and this will define the overall behavior and efficiency of the algorithm.

Another example would be an algorithm that takes `20n² + 15n + 7` operations to be completed. The term `20n²` will tend to dominate as `n` grows, so this algorithm would have a quadratic time complexity because the dominant term has `n²`.

Quadratic time complexity is one of many different types of time complexities that you can find in the world of algorithms.

Let's learn about some of the most common ones.

**`O(1)`** is known as "Constant Time Complexity". When an algorithm has constant time complexity, it takes the same amount of time to run, regardless of input size.

For example, checking if a number is even or odd will always take the same amount of time, regardless of the number itself.

```python
def check_even_or_odd(number):
    if number % 2 == 0:
        return 'Even'
    else:
        return 'Odd'
```

**`O(log n)`** is known as "Logarithmic Time Complexity". This means that the time required by the algorithm increases slowly as the input size grows. This is common in problems in which the size of the problem is repeatedly reduced by a constant fraction.

For example, a popular search algorithm called Binary Search has `O(log n)` worst-case time complexity. This is because it eliminates half of the remaining elements in each comparison, which makes it more efficient overall.

**`O(n)`** is known as "Linear Time Complexity". The running time of algorithms with this time complexity increases proportionally to the input size.

For example, a `for` loop that iterates over all the elements of a list will perform more iterations as the number of list elements increases. If the list is doubled in size, the number of operations will approximately double as well.

```python
for grade in grades:  # grades is a list.
    print(grade)
```

**`O(n log n)`** is known as "Log-Linear Time Complexity". This is a common time complexity of efficient sorting algorithms, like Merge Sort and Quick Sort.

**`O(n²)`** is known as "Quadratic Time Complexity". The running time of these algorithms increases quadratically relative to the input size, which is generally not efficient for real-world problems.

Nested loops are a common example of quadratic time complexity. The inner loop will perform `n` iterations for each one of the `n` iterations of the outer loop, resulting in `n` squared iterations.

```python
for i in range(n):
    for j in range(n):
        print("Hello, World!")
```

Other time complexities include "Exponential Time Complexity", denoted as `O(2^n)`, and "Factorial Time Complexity", denoted as `O(n!)`. Both are inefficient for real-world scenarios.

In this graph, you can compare the growth of the mathematical functions that represent the most common time complexities. Think of the x-axis (horizontal) as the input size and the y-axis (vertical) as the running time of the algorithm.

You can see that the Quadratic Time Complexity (`O(n²)`) (yellow) grows much faster than the other ones, while the Constant Time Complexity (`O(1)`) (red) stays constant, even if the input gets larger.

![graph comparing time complexity](https://cdn.freecodecamp.org/curriculum/lecture-transcripts/what-is-an-algorithm-and-how-does-big-o-notation-work-1.png)

Great. So far, you've learned about Big O notation in terms of time requirements, but this notation can also be applied to the context of space requirements.

In this context, it describes how the memory space required by the algorithm grows as the input size grows.

Algorithms with "Constant Space Complexity" `O(1)` always require a constant amount of memory space, even as the input gets larger.

An example would be an algorithm that only creates and stores a few variables in memory.

In contrast, the space required by algorithms with "Linear Space Complexity" `O(n)` increases proportionally as the input size grows.

An example of this would be an algorithm that creates and stores a copy of a list of length `n`.

And finally, the space requirements of an algorithm with "Quadratic Space Complexity" `O(n²)` increase quadratically as the input size grows.

An example of this would be creating a 2D matrix, where the dimensions are determined by the input size, storing all possible pairs.

Algorithms are the building-blocks of computer programs, while Big O notation is a powerful framework for analyzing how efficient they are, based on how their time and space requirements in the worst-case scenario scale as the input size grows. Understanding their efficiency is very important for developing software that works efficiently in real-world scenarios.

---

# What Are Good Problem-Solving Techniques and Ways to Approach Algorithmic Challenges?

During your learning journey, you should work on developing strong problem-solving skills. These core skills will be essential for tackling real-world problems in your daily work.

Solving algorithmic challenges is a great way to practice. It requires an analytical way of thinking, being able to break the problem down into its core components, and finding a solution that generates the right output efficiently.

But where do you start?

There are several problem-solving techniques that you can use to start approaching these challenges.

As an example, we'll reverse a string in Python.

This is the challenge:

"Given a string, write an algorithm that returns a new string with the characters in reverse order."

The first thing that you should do when you come across this type of problem is to read the description multiple times to make sure that you understand what it says. You may miss critical information if you skip this step or read it too fast.

Then, once you are familiar with the problem, start breaking it down into its core components.

Ask yourself:

* "What is the input?"
* "What is the expected output?"
* "How can I transform the input into the expected output?"

In this problem, you can determine that the input is a string because the challenge starts with "Given a string…"

The output is "a new string with the characters in reverse order."

So you need to take the original string and reverse it.

This initial analysis might seem a bit repetitive at first, but it's very helpful to make sure that you fully understand the requirements.

Then, you should start thinking about how the algorithm that you will develop will transform the input into the output.

During this planning and analysis phase, it's common to use pseudocode to map out the necessary steps.

**Pseudocode** is a high-level description of the algorithm's logic that is general in nature, and is not based on any specific programming language.

Pseudocode is not as formal as actual code, since it's only intended for humans to read. It should be easy to understand at a glance. Its main purpose is to give a clear idea of the sequence of steps that will be performed.

Pseudocode is usually a mixture of a common written language, like English, with programming constructs, like `IF`, `ELSE`, `FOR`, and `WHILE`.

This is an example of pseudocode that you may write to solve the "Reverse a String" challenge.

```python
GET original_string

SET reversed_string = ""

FOR EACH character IN original_string:
  ADD character TO THE BEGINNING OF reversed_string

DISPLAY reversed_string
```

Note how the steps are outlined in a way that is easy to understand. The words and constructs themselves might vary depending on the standards that you are following.

If you wanted to, you could implement these steps in multiple programming languages following the same logic, since the pseudocode is independent of the programming language.

By this point, you may have already realized that this problem can be solved in many different ways. This isn't the only way to reverse a string.

But remember that choosing the right algorithm is important.

In a previous lesson, you learned about algorithmic complexity and why it is important to choose algorithms that are efficient in terms of time and space.

That's where you will play a vital role as a developer. You will need to choose the most efficient algorithm to solve the challenge.

Thinking through different available algorithms is an important problem-solving skill that you should practice. Take a moment to ask yourself if the solution that you are proposing in your pseudocode is the best one or not.

For example, there are many different algorithms for sorting elements, but some of them are more efficient than others. Bubble sort, for example, is very inefficient for sorting large lists, while Quick Sort is usually more efficient.

For our "Reverse a String" challenge, we could use either one of these approaches, assuming that we are planning to implement our algorithm in Python:

* Using the extended slice syntax `[::-1]` to get a new reversed string.
* Looping over the characters from left to right and adding the new character to the beginning of the new string.
* Calling the `reversed()` function to get an iterator with all the characters in reverse order, and then the `““.join()` method to concatenate them back into a string.

Which one should you use? That's your choice.

Making these decisions based on your knowledge and experience can make a huge difference in the final performance of your application. Consider different approaches, their efficiency, implications, and implementation.

Ask yourself:

* "How will I approach this problem?"
* "What data structures will I use?"
* "Are the data structures that I chose the most efficient ones for the problem at hand?"
* "Am I covering all possible edge cases?"

Edge cases are specific, valid inputs or conditions that occur at the boundaries of what an algorithm should handle.

For example, in the "Reverse a String" challenge, an edge case would be taking an empty string as input. Are you handling this correctly? If not, consider the best way to handle this edge case and add it to your pseudocode.

Then, once you are happy with your plan, you can move on to the implementation phase. At this phase, you will implement your algorithm in a programming language.

When structuring your program, you should write modular code that is easy to read and understand.

Use the tools of the programming language based on your current knowledge. Some programming languages include built-in solutions for common problems and tasks. Use them if possible.

To be consistent, follow the best practices of the programming language of your choice.

Test your code as you write it and make sure that you are handling edge cases appropriately.

Once your solution is implemented, check if it works correctly for all the examples and potentially refactor your code to make it clearer or simpler.

Going back to your solution is very important. Development is not necessarily a linear, step-by-step process. You can always go back to your code and use your critical thinking skills to improve it.

These are some common problem-solving techniques that you can follow to approach algorithmic challenges. If you practice consistently, you will gradually develop your problem-solving skills.

---

# What Is Abstraction and How Does It Help Keep Complex Systems Organized?

Now that we've looked at encapsulation, inheritance, and polymorphism, let's discuss the next key concept of object-oriented programming – abstraction.

Abstraction is the process of hiding complex implementation details and showing only the essential features of an object or system. Think of it as focusing on what something does rather than how it does it.

Abstraction is not limited to Python. It's a programming concept that can be implemented in many languages that support object-oriented programming.

To illustrate abstraction, imagine you're driving a car. When you're in the driver's seat, you interact with essential parts like the steering wheel, shifter, and the accelerator and brake pedals. You don't need to know the intricate details of how engine works, how the transmission shifts gears, or the physics behind the braking system, as all of those are the complex implementation details.

That's an abstraction at work! It provides you with a simplified interface to interact with a complex system.

In the case of a car again, the simplified interface is the steering wheel, brakes, and accelerator, while the complex system is the car itself.

As for how Python implements abstraction, it does so through the `abc` module.

This module provides the `ABC` class (standing for “abstract base class”) and the `@abstractmethod` decorator.

`ABC` is the class that is meant to be inherited from, but you cannot create direct objects from it. It is what defines a common interface of methods and properties that its subclasses must implement.

On the other hand, an abstract method is a method declared in an Abstract Base Class (ABC) using the `@abstractmethod` decorator. It may have no implementation or a basic default one. However, any subclass must override it to be considered concrete and instantiable, even if a default implementation is provided.

Here's the basic syntax of abstract class in Python:

```python
from abc import ABC, abstractmethod

# Define an abstract base class
class AbstractClass(ABC):
    @abstractmethod
    def abstract_method(self):
        pass

# Concrete subclass that implements the abstract method
class ConcreteClassOne(AbstractClass):
    def abstract_method(self):
        print('Implementation in ConcreteClassOne')

# Another concrete subclass
class ConcreteClassTwo(AbstractClass):
    def abstract_method(self):
        print('Implementation in ConcreteClassTwo')
```

Here's a basic example:

```python
from abc import ABC, abstractmethod

class Animal(ABC): # Inherits from abstract base class
   @abstractmethod # Abstract method decorator
   def make_sound(self):  # The method subclasses must override
       pass

# Concrete class that will override the abstract method
class Dog(Animal):
   def make_sound(self):
       print('Woof!')

# Another concrete class that will override the abstract method
class Cat(Animal):
   def make_sound(self):
       print('Meow!')

# Another concrete class that will override the abstract method
class Monkey(Animal):
   def make_sound(self):
       print('Ooh ooh aah aah!')

# Create instances of each concrete class
animals = [Dog(), Cat(), Monkey()]

# Loop through the instances to call the make_sound method
for animal in animals:
   animal.make_sound()

# Output:
# Woof!
# Meow!
# Ooh ooh aah aah!
```

In this example:

* We are importing the `ABC` class and `abstractmethod` from the `abc` module.
* We then create an `Animal` class that inherits from `ABC`, and create an abstract method `make_sound` in it that each subclass of `Animal` must override.
* We create the concrete classes `Dog`, `Cat`, and `Monkey`, which must override the `make_sound` abstract method.
* We instantiate the concrete classes and call their `make_sound` method to show how each of them implements the `make_sound` abstract method in its own way.

Remember that you cannot create an instance of the Animal class. Here's what happens if you try to do that:

```python
dog = Animal() 
# TypeError: Can't instantiate abstract class Animal 
# without an implementation for abstract method 'make_sound'
```

The same rule applies to subclasses that don't provide an implementation for the abstract method. Even if you define a subclass of Animal, you can't instantiate it until it overrides make\_sound. Here's an example showing that:

```python
class Bird(Animal):
    pass

bird = Bird()
# TypeError: Can't instantiate abstract class Bird 
# without an implementation for abstract method 'make_sound'
```

Here's another example, this time with an instance attribute you can pass to the instances of the concrete methods:

```python
from abc import ABC, abstractmethod

# The blueprint for any toy that can speak
class TalkingToy(ABC):
   def __init__(self, name):
       self.name = name
   @abstractmethod
   def speak(self):
       pass

class RobotToy(TalkingToy):
   def speak(self):
       print(f'{self.name} says beep boop! I am a robot!')

class TeddyBearToy(TalkingToy):
   def speak(self):
       print(f"{self.name} says hug me! I'm cuddly!")

class DinosaurToy(TalkingToy):
   def speak(self):
       print(f'{self.name} says ROOOOAR!')

# Create toys
rusty = RobotToy('Rusty')
fluffy = TeddyBearToy('Fluffy')
rex = DinosaurToy('Rex')

toys = [rusty, fluffy, rex]
for toy in toys:
   toy.speak()

# Output:
# Rusty says beep boop! I am a robot!
# Fluffy says hug me! I'm cuddly!
# Rex says ROOOOAR!
```

In this example:

* We have an abstract base class `TalkingToy` that defines a blueprint for any toy that can speak.
* The subclasses `RobotToy`, `TeddyBearToy`, and `DinosaurToy` implement the `speak` method in their own way.
* When we create instances of these subclasses and call the `speak` method, each toy speaks in its own unique way.

In conclusion, abstraction in Python simplifies complex systems by increasing reusability.

You've seen how you can reuse a single method from an abstract class across multiple subclasses while forcing each subclass to provide its specific behavior.

This approach keeps your code organized, flexible, and easier to maintain, especially as your application grows.

---

# Module 11: Linear Data Structures

# How Do Dynamic Arrays Differ From Static Arrays?

Arrays are a fundamental data structure in computer science. All arrays store ordered collections of data, but depending on their type, they may work differently behind the scenes.

Their underlying behavior can have an important effect in the program's efficiency, so let's learn about dynamic and static arrays and their differences, so you can choose the most efficient one for your program.

We'll start with static arrays.

**Static arrays** have a fixed size. They store elements in adjacent memory locations.

The size of a static array is determined when the array is initialized. Once that specific block of memory is allocated, it's fixed, and cannot be changed while the program is running. This is a key characteristic of static arrays.

Storing elements in adjacent memory locations makes the data retrieval process more efficient because the program can store the location of the first element and then use indices to make simple calculations and find the other elements in memory.

Thanks to this, accessing the values of a static array takes constant time `O(1)`, which is very efficient.

You can use a static array when you know the number of elements that will be stored in advance. It's also helpful when the values will be accessed very frequently, since the access operation is very efficient.

However, this data structure cannot grow or shrink, so if the number of elements that will be stored can vary, you should use a dynamic array instead.

Trying to increase the size of a static array would involve creating a new array and copying all the elements from the old array to a new one, which is inefficient. In that case, a dynamic array would be much better because it handles this process automatically.

Python does not include traditional static arrays as built-in data structures.

But other programming languages, like Java, do support them. This is an example of a static array in Java that can store three integers:

```python
int[] numbers = new int[3];
```

Arrays in Python are dynamic, so let's take a look at those.

**Dynamic arrays** are more flexible because they can grow or shrink automatically while the program is running.

They work through an automatic resizing mechanism that copies the elements into a new array when the original array is full. The process is done efficiently because the size of the new array is chosen in an efficient way that makes these computationally expensive operations less frequent.

Accessing the elements of a dynamic array takes constant time `O(1)`, so this operation is very efficient.

Inserting an element in the middle of the array takes linear time `O(n)` because the elements after it need to be relocated.

Inserting an element at the end of the array takes constant time `O(1)` if there is still space available in the dynamic array, but if the array is full and needs resizing, this operation has a `O(n)` complexity.

You should use dynamic arrays when you don't know in advance the number of values that you will need to store in the array. They are also helpful when you will be frequently inserting and deleting elements.

Python's built-in `list` data structure works as a dynamic array. You can create a list by writing the elements within square brackets, separated by commas.

```python
numbers = [3, 4, 5, 6]
```

You can access an element by writing the name of the variable that holds the list, followed by square brackets, and within the square brackets, the corresponding index.

Indices start from 0 for the first element and are incremented by 1 for each subsequent element:

```python
numbers[0]  # 3
numbers[1]  # 4
numbers[2]  # 5
numbers[3]  # 6
```

To update a value, you just need to reassign it:

```python
numbers[2] = 16
```

You can append elements to the list with the `.append()` method:

```python
numbers.append(7)
```

You can insert elements at a specific index with the `.insert()` method, passing the index as the first argument and the element itself as the second argument.

```python
numbers.insert(3, 15)
```

You can remove an element at a specific index with the `.pop()` method:

```python
numbers.pop(2)
```

If you don't specify the index, `.pop()` will remove the last element.

There are other built-in list methods that you can check in the documentation for adding and removing elements quite easily.

That's the power of dynamic arrays, or lists in this case.

In general, you should use static arrays when you know the number of elements in advance and you need to access them frequently, and use dynamic arrays when the number of elements is unknown or variable over time.

You should always consider the tradeoff between the simplicity of static arrays and the flexibility of dynamic arrays. They are both helpful for specific use cases and scenarios. Being able to choose the best one for a given problem is part of the problem-solving skills that you will gradually develop with practice.

---

# How Do Singly Linked Lists Work and How Do They Differ From Doubly Linked List?

A **linked list** is a linear data structure in which each node is connected to the next node in the sequence.

These connections create a data structure that looks like a chain of nodes, where each node stores data and a reference to the next node in the linked list.

![linked list basic structure visualization](https://cdn.freecodecamp.org/curriculum/lecture-transcripts/how-do-singly-linked-lists-work-and-how-do-they-differ-from-doubly-linked-list-1.png)

We use these references to go from the first node to the next node and so on.

Linked lists are commonly used for implementing other data structures, such as stacks, queues, and deques. They can also be used to implement essential graph algorithms, such as depth-first search and breadth-first search.

Singly Linked Lists
-------------------

A **singly linked list** is a type of linked list in which each node is connected to the next node in the sequence.

Each node is connected to the next one by storing a reference to it.

This single reference per node allows you to traverse the linked list in one direction, from start to end.

The search can only move forward, not backwards.

In this example, you would start at the head node, node A.

The **head** node is the first node in the linked list.

In a singly linked list, the head node is usually the only node that is directly accessible. This is where the search process will start when you're trying to find a specific node.

![singly linked list traversal visualization](https://cdn.freecodecamp.org/curriculum/lecture-transcripts/how-do-singly-linked-lists-work-and-how-do-they-differ-from-doubly-linked-list-2.webp)

The process will start at node A, then it will continue to node B, then node C, and finally node D, the **tail** node. It may also stop before that if you implement specific logic in your code.

The **tail** node is the last node. It's used to determine when the process has reached the end of the linked list.

### **Inserting Nodes**

One of the great things about linked lists is that they do not have a fixed size. They can be expanded or shrunk as needed by simply updating the connections between the nodes.

You can **insert** a node at the start, middle, and end of a linked list.

Linked lists don't necessarily need to store the nodes in a specific order. The order will be determined by the connections between the nodes.

However, if you do need to keep the nodes in a specific order for your particular use case, you can do so by implementing that logic in your code and the criteria you implement will determine if the node is inserted at the start, middle, or end.

To insert a node at the start of the linked list, you just need to create a connection between the new node and the node that used to be the head node and make the new node the head node instead.

This is an example, where we insert node E at the start and make this new node the head node of the linked list.

![singly linked list insert at beginning visualization](https://cdn.freecodecamp.org/curriculum/lecture-transcripts/how-do-singly-linked-lists-work-and-how-do-they-differ-from-doubly-linked-list-3.png)

Inserting a node at the beginning of the linked list has a constant time complexity `O(1)` because it only requires updating the reference to the head node and the connection between the new head node and the next node in the sequence.

In this example, we are inserting node E at the start of the linked list. This will work correctly. But if we wanted to keep the linked list sorted in alphabetical order, node E would have to be inserted at the end of the linked list instead.

To insert a node at the end of the linked list, first you need to reach the end and then add a connection to the new node to make it the new tail node.

This operation has linear time complexity, `O(n)`, where n is the number of nodes stored in the linked list, because first you need to reach the end of the linked list to make the insertion and this would require going from one node to the next and so on until the end is reached.

![singly linked list insert at end visualization](https://cdn.freecodecamp.org/curriculum/lecture-transcripts/how-do-singly-linked-lists-work-and-how-do-they-differ-from-doubly-linked-list-4.png)

If the node has to be inserted somewhere in the middle of the linked list, the connections between the nodes will have to be updated too. The previous node in the sequence should be connected to the new node and the new node should be connected to the next node, like in the following diagram.

![singly linked list insert in middle visualization](https://cdn.freecodecamp.org/curriculum/lecture-transcripts/how-do-singly-linked-lists-work-and-how-do-they-differ-from-doubly-linked-list-5.webp)

The insertion operation has a constant space complexity `O(1)`, since inserting a new node only requires creating it and updating the connections between the nodes. This operation doesn't depend on the size of the linked list itself.

### **Removing Nodes**

Just as you can insert nodes, you can also remove them from the start, middle, and end of the linked list.

To remove a node from the start, you need to update the reference to the head node, which should be the next node in the sequence.

This operation has a constant time complexity `O(1)`, because it only requires updating the linked list's reference to the head node.

![singly linked list remove from beginning visualization](https://cdn.freecodecamp.org/curriculum/lecture-transcripts/how-do-singly-linked-lists-work-and-how-do-they-differ-from-doubly-linked-list-6.png)

To remove a node from the middle of the linked list, you need to update the reference of the previous node to connect it to the next node in the sequence, forming a sort of "bridge" between them, as you can see in this diagram.

![singly linked list remove from middle visualization](https://cdn.freecodecamp.org/curriculum/lecture-transcripts/how-do-singly-linked-lists-work-and-how-do-they-differ-from-doubly-linked-list-7.png)

That will remove the node that you want to remove, in this case node B, from the sequence of connections, so it won't be reached the next time you traverse it.

To remove a node from the end of the linked list, you need to remove the connection of the previous node and make this node the new tail node. Now the linked list will end at the new tail node.

This operation has a linear time complexity `O(n)`, because first you have to reach the end of the linked list.

![singly linked list remove from end visualization](https://cdn.freecodecamp.org/curriculum/lecture-transcripts/how-do-singly-linked-lists-work-and-how-do-they-differ-from-doubly-linked-list-8.png)

The deletion operation has a constant space complexity `O(1)`, because no additional memory is required to delete a node.

Doubly Linked Lists
-------------------

Now that you know more about singly linked lists, let's talk about doubly linked lists.

In a **doubly linked list**, each node stores two references: a reference to the next node and a reference to the previous node in the sequence.

This means that doubly linked lists can be traversed in both directions.

![doubly linked list structure visualization](https://cdn.freecodecamp.org/curriculum/lecture-transcripts/how-do-singly-linked-lists-work-and-how-do-they-differ-from-doubly-linked-list-9.webp)

In this type of linked list, it's also common to keep a reference to the tail node in the linked list itself to start the traversal from the end if necessary.

That sounds great, right? They're more flexible than singly linked lists.

However, doubly linked lists do require more memory than singly linked lists because each node stores **two** references instead of one.

This is something that you should keep in mind when you're choosing the right data structure for your project.

There **is** a tradeoff.

The insertion and deletion operations work exactly the same. The only difference is that now you will need to update two references per node and keep track of the reference to the tail node to insert elements at the end of the doubly linked list very efficiently and start the traversal process from the back, if necessary.

Singly and doubly linked lists are essential data structures in computer science used for storing and manipulating elements in a sequential order. Understanding their differences is essential for choosing the right one for your specific application.

---

# How Do Stacks and Queues Work?

Stacks and queues are data structures commonly used in computer science.

They're linear data structures that follow specific rules for adding and removing elements.

Stacks
------

Let's start with **Stacks**.

A **stack** is a Last-in, First-out (LIFO) data structure.

This means that the last element that was added to the stack is the first one to be removed.

Stacks have two ends, which we know as top and bottom.

Elements are added and removed from the top of the stack.

You can think of a stack as a pile of dishes, where you can only place dishes at the top of the pile and take dishes from the top of the pile.

![stack data structure visualization](https://cdn.freecodecamp.org/curriculum/lecture-transcripts/how-do-stacks-and-queues-work-1.png)

These operations of adding and removing elements have special names in this context.

Adding an element to a stack is known as a "push" operation. We say that we "push" an element onto the stack when we add it to the top of the stack.

![stack push operation visualization](https://cdn.freecodecamp.org/curriculum/lecture-transcripts/how-do-stacks-and-queues-work-2.png)

Removing an element from a stack is known as a "pop" operation. We say that we "pop" an element from the stack when we remove it from the top of the stack.

![stack pop operation visualization](https://cdn.freecodecamp.org/curriculum/lecture-transcripts/how-do-stacks-and-queues-work-3.png)

You can see that we don't really perform any operations at the bottom of the stack but we keep it there as a reference.

The time complexity of the push and pop operations is typically `O(1)`, a constant time complexity.

When you push an element onto the stack, the element is simply added to the top.

When you pop an element from the stack, the element at the top is removed.

Therefore, the time it takes to perform these operations remains constant regardless of the size of the stack.

The space complexity of the push and pop operations is usually constant `O(1)`. This means that the amount of memory required to perform these operations remains constant regardless of the size of the stack.

Queues
------

Now that you know more about stacks, let's learn about **Queues**.

A queue is a First-in First-out (FIFO) linear data structure. This means that the first element added to the queue is the first one to be removed.

Queues have two ends: front and back.

![queue data structure visualization](https://cdn.freecodecamp.org/curriculum/lecture-transcripts/how-do-stacks-and-queues-work-4.webp)

Elements are added to the back of the queue and they are removed from the front of the queue.

You can think of a queue as a line of people waiting to pay for their groceries at the supermarket. The first person in line is the first one to go to the cash register while new people join the line at the end.

The operations of adding and removing elements have special names in the context of a queue.

Adding an element to the back of a queue is known as an "enqueue" operation.

In an enqueue operation, the new element is added to the end of the queue, becoming the end of the line.

![queue enqueue operation visualization](https://cdn.freecodecamp.org/curriculum/lecture-transcripts/how-do-stacks-and-queues-work-5.png)

Removing an element from the front of the queue is known as a "dequeue" operation.

In the dequeue operation, the element at the front of the queue is removed, and the next element in line becomes the new front.

![queue dequeue operation visualization](https://cdn.freecodecamp.org/curriculum/lecture-transcripts/how-do-stacks-and-queues-work-6.png)

The time complexity of the enqueue and dequeue operations is `O(1)`, constant time. The time it takes to perform these operations remains constant, regardless of the size of the queue.

The space complexity of the enqueue and dequeue operations is usually constant `O(1)`. This means that the amount of memory required to perform these operations remains constant regardless of the size of the queue.

Stacks and queues are data structures used in computer science for organizing and managing elements. Understanding them is essential for building efficient algorithms in various programming applications.

---

# How Do Maps, Hash Maps and Sets Work?

In this lesson, we'll go over maps, hash maps, and sets. But before we do that, let's define Abstract Data Types.

An Abstract Data Type (ADT) is a conceptual representation of a data type, including what operations can be performed on the data and the properties of that data.

Abstract Data Types are like blueprints that describe **what** operations can be performed, not **how** they are performed. They separate the interface from the actual implementation of the operations.

A **map** is an ADT that manages collections of key-value pairs and their operations in a very specific and efficient way.

In a map, every value is associated with a specific key.

One of the key characteristics of maps is that every key must be unique. This uniqueness allows for direct lookups, which makes the process of retrieving information much more efficient.

Only keys must be unique, values can be repeated.

The map Abstract Data Type also defines important operations, such as inserting key-value pairs, getting the value associated with a key, updating the value associated with a key, removing a key-value pair, and checking if a key exists in the map.

It doesn't actually specify how these operations should be performed, it just lists them as part of the available operations of the data type.

A **hash map**, also known as a hash table, is a concrete implementation of the map Abstract Data Type.

Hash maps use a technique called "hashing" to perform common operations very efficiently.

Hashing essentially works by generating a hash value for each element using a hash function.

The hash value is generated based on the key of the key-value pair and it's used to calculate an index in an underlying array, the actual data structure where the key-value pairs are stored.

But you might be asking yourself: What happens if two keys result in the same index?

Hash maps solve these collisions with clever strategies.

One option is to use the "chaining" strategy, where each array index points to a linked list (another data structure), where all the elements with the same index are stored.

Another strategy is to use "open addressing", which involves searching for the next available index in the array based on a predefined search sequence.

The average case time complexity of hash maps is "Constant Time" `O(1)` for inserting, retrieving, and deleting key-value pairs.

The worst case time complexity of these operations is Linear Time `O(n)`, which occurs when there are many hash collisions, so the collision resolution strategy has to be applied multiple times.

The space complexity of inserting into a hash map is constant `O(1)` on the average case, a constant amount of memory to store the new pair. However, in the worst case, it can have linear space complexity `O(n)` due to a resizing operation of the underlying array. In general, removing an element has a constant space complexity `O(1)`.

This turns the hash table into something similar to a linear data structure where `n` elements have to be scanned to find the target key. However, this is relatively rare if the hash map is implemented properly.

Python's **dictionaries** are implemented as hash maps behind the scenes.

To create a Python dictionary, you just need to write the key-value pairs within curly brackets and separate them with a comma. Each key should be separated from its corresponding value with a colon.

```python
my_dictionary = {
  'A': 1,
  'B': 2, 
  'C': 3
}
```

In this code, `'A'` is the key and `1` is the value:

```python
'A': 1
```

Alternatively, you can use `dict()`:

```python
my_dictionary = dict(A=1, B=2, C=3)
```

You can get the value through its corresponding key:

```python
my_dictionary['A']  # 1
```

You can also update the value associated with a key:

```python
my_dictionary['A'] = 4
```

And you can remove a key-value pair:

```python
del my_dictionary['A']
```

You can also check if a key is in the dictionary (or not):

```python
'C' in my_dictionary
```

And you can call these methods to get the keys, values, and items of the dictionary, respectively.

```python
my_dictionary.keys()
my_dictionary.values()
my_dictionary.items()
```

Great. Now that you know more about maps and hash maps, let's talk about sets.

**Sets** are unordered collections of unique elements.

Let's break this concept down into its key components:

* Sets are unordered. The elements of a set are not stored in any specific order, so you cannot access them through indices.
* Sets only contain unique elements. If you try to add the same value twice, only one copy of the value will be kept.

They are analogous to sets in mathematics and they implement the same set operations, like intersection, union, and difference.

One of the main advantages of sets is that they guarantee that the elements will be unique (no duplicates). This is why they are often used to remove duplicates from lists and other data structures.

They are also dynamic. They can adjust to the number of elements that are currently stored. This makes them quite powerful.

The average case time complexity of adding, removing, getting the length of the set, and checking if an element is in the set is "Constant Time" `O(1)`, which is very efficient.

Since sets are implemented as hash tables, the worst case time complexity of adding, removing, and checking membership is "Linear Time" `O(n)`. This may occur when there are multiple hash collisions, transforming the hash table into something similar to a linear data structure, where `n` scans are required to find the key.

In terms of space complexity, in the average case, inserting an element would have constant complexity `O(1)`, with a new unique element requiring a constant amount of memory. However, in the worst case, there could be a resizing operation of the underlying array, which could take linear space complexity `O(n)`. In general, removing an element would take constant space complexity `O(1)`.

Python has a built-in `set` data structure that you use to work with sets in your programs.

Behind the scenes, Python sets are implemented using a hash table where only the keys are stored, without any associated values.

Sets can only store objects of immutable data types because their hash values always remain the same. In contrast, the hash values of mutable objects can change when they are mutated. That's why they cannot be part of sets. If the hash value of an object stored in the set changes, the program would not be able to find it anymore.

To define a set in Python, you just need to surround the elements with curly brackets and separate them with commas:

```python
numbers = {1, 2, 3, 4}
```

To create an empty set, you can call `set()`:

```python
numbers = set()
```

Note that if you use empty curly brackets, this will automatically create a Python dictionary, not a set, so you must call the `set()` function to create an empty set.

You can add an element to a set with the `.add()` method:

```python
numbers.add(5)
```

You can also remove elements from the set with the `.remove()` method:

```python
numbers.remove(5)
```

This will throw a `KeyError` if the element is not found. But if you don't want to throw an error in that case, you can use the `.discard()` method instead.

The `.pop()` method returns an arbitrary element from the set, while the `.clear()` method removes all elements from the set.

You can test if an element is in a set with the `in` operator:

```python
5 in numbers
```

Python also support set operations, including union, difference, symmetric difference, and intersection, which you can perform with these methods:

```python
set_a = {1, 2, 3, 4}
set_b = {2, 3, 4, 5, 6}

set_a.union(set_b)
set_a.intersection(set_b)
set_a.symmetric_difference(set_b)
set_a.difference(set_b)
```

Or with their equivalent operators:

```python
set_a | set_b
set_a & set_b
set_a ^ set_b
set_a - set_b
```

The average case time complexity for adding, removing, and testing membership is "Constant Time" `O(1)`.

The worst case time complexity for these operations is "Linear Time" `O(n)` because of the hash map's worst case collision scenario.

You can also check if a set is a subset or superset of another one:

```python
set_a.issubset(set_b)
set_a.issuperset(set_b)
```

In general, you should use sets when you need to store a collection of unique items and frequently check for the presence of an item.

Maps, hash maps, and sets are powerful data structures designed for efficient data organization and retrieval. Each one of them has its own unique characteristics and use cases. As a developer, you will need to choose the best one for your project.

---

## Module Review Component

# Data Structures Review

Algorithms and Big O Notation
-----------------------------

* **Algorithms**: A set of unambiguous instructions for solving a problem or carrying out a task. Algorithms must finish in a finite number of steps and each step must be precise and unambiguous.
* **Big O Notation**: Describes the worst-case performance, or growth rate, of an algorithm as the input size increases. It focuses on how resource usage grows with input size, ignoring constant factors and lower-order terms.

### Common Time Complexities

* **O(1) - Constant Time**: Algorithm takes the same amount of time regardless of input size.

```python
def check_even_or_odd(number):
    if number % 2 == 0:
        return 'Even'
    else:
        return 'Odd'
```

* **O(log n) - Logarithmic Time**: Time increases slowly as input grows. Common in algorithms that repeatedly reduce problem size by a fraction (like Binary Search).
* **O(n) - Linear Time**: Running time increases proportionally to input size.

```python
for grade in grades:
    print(grade)
```

* **O(n log n) - Log-Linear Time**: Common time complexity of efficient sorting algorithms like Merge Sort and Quick Sort.
* **O(n²) - Quadratic Time**: Running time increases quadratically. Often seen in nested loops.

```python
for i in range(n):
    for j in range(n):
        print("Hello, World!")
```

### Space Complexity

* **O(1) - Constant Space**: Algorithm uses same amount of memory regardless of input size.
* **O(n) - Linear Space**: Memory usage grows proportionally with input size.
* **O(n²) - Quadratic Space**: Memory usage grows quadratically with input size.

Problem-Solving Techniques
--------------------------

* **Understanding the Problem**: Read the problem statement multiple times. Identify the input, expected output, and how to transform input to output.
* **Pseudocode**: High-level description of algorithm logic that is language-independent. Uses common written language mixed with programming constructs like `IF`, `ELSE`, `FOR`, `WHILE`.

```python
GET original_string
SET reversed_string = ""
FOR EACH character IN original_string:
  ADD character TO THE BEGINNING OF reversed_string
DISPLAY reversed_string
```

* **Edge Cases**: Specific, valid inputs that occur at the boundaries of what an algorithm should handle. Always consider and test edge cases.

Arrays
------

* **Static Arrays**: Have a fixed size determined at initialization. Elements stored in adjacent memory locations. Size cannot be changed during program execution.
* **Dynamic Arrays**: Can grow or shrink automatically during program execution. Handle resizing through automatic copying to larger arrays when needed.

### Python Lists (Dynamic Arrays)

```python
numbers = [3, 4, 5, 6]

# Access elements
numbers[0]  # 3

# Update elements
numbers[2] = 16

# Add elements
numbers.append(7)
numbers.insert(3, 15)  # Insert at specific index

# Remove elements
numbers.pop(2)  # Remove at specific index
numbers.pop()   # Remove last element
```

### Time Complexities for Dynamic Arrays

* **Access**: O(1)
* **Insert at end**: O(1) average, O(n) when resizing needed
* **Insert in middle**: O(n)
* **Delete**: O(n) for middle, O(1) for end

Stacks
------

* **Stacks**: Last-In, First-Out (LIFO) data structure. Elements added and removed from the top only.
* **Push Operation**: Adding an element to the top of the stack. Time complexity: O(1).
* **Pop Operation**: Removing an element from the top of the stack. Time complexity: O(1).

```python
# Using Python list as stack
stack = []

# Push operations
stack.append(1)
stack.append(2)
stack.append(3)

# Pop operations
top_element = stack.pop()  # Returns 3
```

Queues
------

* **Queues**: First-In, First-Out (FIFO) data structure. Elements added to the back and removed from the front.
* **Enqueue Operation**: Adding an element to the back of the queue. Time complexity: O(1).
* **Dequeue Operation**: Removing an element from the front of the queue. Time complexity: O(1).

```python
from collections import deque

# Using deque for efficient queue operations
queue = deque()

# Enqueue operations
queue.append(1)
queue.append(2)
queue.append(3)

# Dequeue operations
first_element = queue.popleft()  # Returns 1
```

Linked Lists
------------

* **Linked Lists**: Linear data structure where each node contains data and a reference to the next node. Nodes are connected like a chain.

### Singly Linked Lists

* **Structure**: Each node has data and one reference to the next node.
* **Traversal**: Can only move forward from head to tail.
* **Head Node**: First node in the list, usually the only directly accessible node.
* **Tail Node**: Last node in the list, points to `None`.

### Operations and Time Complexities

* **Insert at beginning**: O(1)
* **Insert at end**: O(n) - must traverse to end
* **Insert in middle**: O(n) - must traverse to position
* **Delete from beginning**: O(1)
* **Delete from end**: O(n) - must traverse to find previous node
* **Delete from middle**: O(n) - must traverse to find node

### Doubly Linked Lists

* **Structure**: Each node has data and two references: next node and previous node.
* **Traversal**: Can move in both directions.
* **Memory**: Requires more memory than singly linked lists due to extra reference.

Hash Maps and Sets
------------------

### Maps and Hash Maps

* **Map (Abstract Data Type)**: Manages collections of key-value pairs. Every key must be unique, but values can be repeated.
* **Hash Map**: Concrete implementation of map ADT using hashing technique. Uses hash function to generate hash values for keys, which determine storage location in underlying array.

### Python Dictionaries (Hash Maps)

```python
# Creating dictionaries
my_dictionary = {
    "A": 1,
    "B": 2, 
    "C": 3
}

# Alternative creation
my_dictionary = dict(A=1, B=2, C=3)

# Access and modify
value = my_dictionary["A"]  # 1
my_dictionary["A"] = 4      # Update value
del my_dictionary["A"]      # Remove key-value pair

# Check membership
"C" in my_dictionary

# Get keys, values, items
my_dictionary.keys()
my_dictionary.values()
my_dictionary.items()
```

### Time Complexities for Hash Maps

* **Average case**: O(1) for insert, get, delete
* **Worst case**: O(n) when many hash collisions occur

### Sets

* **Sets**: Unordered collections of unique elements. No duplicates allowed, no specific order maintained.
* **Immutable Elements Only**: Sets can only contain immutable data types (numbers, strings, tuples) because hash values must remain constant.

```python
# Creating sets
numbers = {1, 2, 3, 4}
empty_set = set()  # Must use set(), not {}

# Add and remove elements
numbers.add(5)
numbers.remove(4)      # Raises KeyError if not found
numbers.discard(4)     # No error if not found

# Set operations
set_a = {1, 2, 3, 4}
set_b = {2, 3, 4, 5, 6}

# Union, intersection, difference, symmetric difference
set_a.union(set_b)                    # or set_a | set_b
set_a.intersection(set_b)             # or set_a & set_b
set_a.difference(set_b)               # or set_a - set_b
set_a.symmetric_difference(set_b)     # or set_a ^ set_b

# Subset and superset checks
set_a.issubset(set_b)
set_a.issuperset(set_b)
set_a.isdisjoint(set_b)

# Membership testing
5 in numbers
```

### Time Complexities for Sets

* **Average case**: O(1) for add, remove, membership testing
* **Worst case**: O(n) due to hash collisions

Hash Collisions
---------------

* **Hash Collision**: Occurs when two different keys produce the same hash value.
* **Collision Resolution Strategies**:

  + **Chaining**: Each array index points to a linked list storing all elements with same hash value
  + **Open Addressing**: Search for next available index using predefined sequence

When to Use Each Data Structure
-------------------------------

* **Lists**: When you need ordered, indexed access and don't know size in advance
* **Stacks**: For LIFO operations (undo functionality, expression evaluation, backtracking)
* **Queues**: For FIFO operations (task scheduling, breadth-first search)
* **Linked Lists**: When frequent insertion/deletion at beginning, unknown size, no random access needed
* **Hash Maps**: For fast key-value lookups, counting occurrences, caching
* **Sets**: For uniqueness checking, mathematical set operations, removing duplicates

---

# Module 12: Searching and Sorting Algorithms

# What Is Binary Search and How Does It Differ From Linear Search?

Searching through a list of items is a common occurrence in computer science. There are two key algorithms you should know about when it comes to searching: linear search and binary search.

Linear search starts at the beginning of a list and iterates through each item until it finds the target value it is looking for.

If the target value is found, the index where it's located in the list is returned. If the target value isn't found, `-1` is returned. We return `-1` because it's not a valid index in most programming languages.

Here is what the code looks like for linear search:

```python
def linear_search(arr, target):
    for i in range(len(arr)):
        if arr[i] == target:
            return i
    return -1
```

If the list we'll search through is `[13, 4, 7, 9, 10]` and the target value is `9`, the function would return `3` because `9` is at index `3`.

If we changed the target value to `5`, the function would return `-1` because `5` is not in the list.

While this is a relatively straightforward algorithm, it is not the most efficient. If you have a large list of items, linear search can take a long time to find the target value.

The time complexity of linear search is `O(n)` because the time it takes to search through the list grows linearly with the size of the list.

The space complexity of linear search is `O(1)` because it doesn't require any additional space to search through the list.

Binary search is a more efficient algorithm for searching through a large list of items. The condition here is that the list must be sorted in ascending order.

Binary search works by dividing the list in half and checking if the target value is in the middle of the list. If the target value is in the middle of the list, the index of the target value is returned. Otherwise, the algorithm checks if the target value is in the left or right half of the list.

It continues to divide the remaining parts of the list into halves until the target value is found. If the target value is not in the list, it returns `-1`

Here is what the code looks like for binary search:

```python
def binary_search(arr, target):
    low = 0
    high = len(arr) - 1

    while low <= high:
        mid = (low + high) // 2  

        if arr[mid] == target:
            return mid
        elif arr[mid] < target:
            low = mid + 1
        else:
            high = mid - 1

    return -1
```

We start by identifying a `low` and `high` index. This represents the range of the list we are searching through.

We then check the condition of `low` being less than or equal to `high`. If `low` is greater than `high`, we have searched through the entire list and the target value is not found. In that case we stop the search and return `-1`.

If the `low` index is less than or equal to the `high` index, we calculate the middle index of the list, `mid`. We then check if the target value is at the middle index. If it is, we return the middle index.

Otherwise, we check if the value at the midpoint is less than the target. If it is, we update the low index to be the middle index plus one. This means we will search the right half of the list.

Lastly, if none of the other conditions are `True`, we update the `high` index to be the middle index minus one. This means we will search the left half of the list.

We continue to repeat this process until we find the target or determine that the target is not in the list.

The time complexity of binary search is `O(log n)` because the time it takes to search through the list grows logarithmically with the size of the list.

The space complexity of binary search is `O(1)` because it doesn't require any additional space to search through the list.

Binary search and linear search can be used for a variety of problems you will encounter in computer science. It is important to understand the differences between the two algorithms and when to use each one.

---

# What Is Divide and Conquer, and How Does Merge Sort Work?

The divide and conquer paradigm in computer science is a technique for recursively breaking down problems into smaller sub-problems. One of the key aspects of this technique is recursion, which happens when a function calls itself repeatedly until a base case is reached. In this lesson, we will take a look at the merge sort algorithm to better understand how the divide and conquer technique works.

Let's say we had this list of numbers:

```python
42 37 53 17
```

The goal is to sort that list from smallest to largest using the merge sort algorithm. The first step is to divide that list in half:

```python
42 37 | 53 17
```

Then we need to look at the left side of the list:

```python
42 37
```

We take that sub list and divide in half again until each sub list has only one item in it:

```python
42 | 37
```

A list with only one item in it is sorted by default. Next we need to merge each of those one element sub lists into a sorted list:

```python
37 42
```

Then we follow the same process for the right side of the original list:

```python
# right side of original list
53 17

# divide the list in half
53 | 17

# merge the lists in sorted order
17 53
```

Now that both halves of the original list are sorted, we merge those two halves together and sort the elements:

```python
17 37 42 53
```

Here is what the algorithm looks like in code:

```python
def merge_sort(arr):
    if len(arr) <= 1:
        return arr

    mid = len(arr) // 2
    left = merge_sort(arr[:mid])
    right = merge_sort(arr[mid:])

    sorted_list = []
    i = 0
    j = 0

    while i < len(left) and j < len(right):
        if left[i] <= right[j]:
            sorted_list.append(left[i])
            i += 1
        else:
            sorted_list.append(right[j])
            j += 1

    sorted_list.extend(left[i:])
    sorted_list.extend(right[j:])

    return sorted_list
```

The time complexity for merge sort would be `O(n log n)` because the list is continuously divided in half (`log n`) and then merged together (`O(n)`). Unlike other sorting algorithms like bubble sort, merge sort is not sorted in place and has a space complexity of `O(n)`.

---

## Module Review Component

# Searching and Sorting Algorithms Review

Searching Algorithms
--------------------

Searching algorithms let you search for a target within a certain list of items.

In computer science, there are two searching algorithms you should know about. They are **linear search** and **binary search** algorithms. It is important to understand the differences between the two algorithms and when to use each one.

### Linear Search

* Linear search iterates through a list of items, checking each item from the beginning until the target item is found.
* If the target item is found, the index where it is located in the list is returned.
* If the target is not found, it returns `-1`, which means **invalid index** in most programming languages.
* Because linear search checks each item until it finds the target, it is not efficient for a large list of items.
* The time complexity of linear search is `O(n)` because the time it takes to search through the list grows linearly with the size of the list.
* The space complexity of linear search is `O(1)` because it doesn't require any additional space to search through the list.

### Binary Search

* Binary search works by dividing a list of items in half, and checking if the target value is in the middle of the list.
* The condition for binary search to work is that the items in the list must be sorted, either in ascending or descending order.
* Binary search is a more efficient algorithm for searching through a large list of items because it divides the list of items in half and ignores any half where the target is not found.
* If the target item is found in the middle of the list, the index of the target item is returned.
* If the item is not found, the algorithm checks if the target item is in the left or right half of the list.
* It continues to divide the remaining parts of the list into halves until the target item is found.
* If the target item is finally not found in the list, it returns `-1`
* The time complexity of binary search is `O(log n)` because the time it takes to search through the list grows logarithmically with the size of the list.
* The space complexity of binary search is `O(1)` because it doesn't require any additional space to search through the list.

### How Linear Search Differs from Binary Search

* Binary search is more suitable for a large list of items compared to linear search.
* The time complexity of linear search is `O(n)` because the time it takes to search through the list grows linearly with the size of the list.
* The time complexity of binary search is `O(log n)` because the time it takes to search through the list grows logarithmically with the size of the list.

Sorting Algorithms and Divide-and-Conquer
-----------------------------------------

In computer science, divide-and-conquer is a technique used to break down a problem into smaller sub-problems so they are easier to solve. Recursion is the technique often employed in divide-and-conquer, and divide-and-conquer is a powerful strategy used to implement many efficient sorting algorithms like merge sort.

### Merge Sort

* Merge sort is a sorting algorithm that follows the divide-and-conquer approach.
* It works by recursively dividing a list into smaller sub-lists until each sub-list contains only one element.
* It then repeatedly merges the sub-lists back together in a sorted order.
* The time complexity for merge sort is `O(n log n)` because the list is continuously divided in half `(log n)` and then merged together `(O(n))`.
* The space complexity of merge sort is `O(n)` because it is not an in-place sorting algorithm.

---

# Module 13: Non-Linear Data Structures (Trees and Graphs)

# What Are Trees and Tries and How Do They Work?

Trees are very important in the world of computer science.

A **tree** is a specific type of graph.

For a graph to be classified as a tree, it must:

* Have no loops or cycles (paths where the start and end nodes are the same).
* Be connected (every node can be reached from every other node).

Trees are non-linear data structures that organize nodes in a hierarchy, where nodes may have children, siblings, and parent nodes.

The root node is the very top of a tree. It's the only node in the tree without a parent node. This is the node where you will start traversing the entire data structure, usually with algorithms like breadth-first search (BFS) or depth-first search (DFS).

This is a graphical example of a tree:

![A tree diagram showing a hierarchical structure with node A at the root, nodes B and C as children of A, and nodes D and E as children of C. Node B is a leaf node.](https://cdn.freecodecamp.org/curriculum/lecture-transcripts/what-are-trees-and-tries-and-how-do-they-work-1.png)

Since nodes are organized in a hierarchy, they have relationships between them.

A **parent node** is a node that is immediately connected to other nodes below it. In the diagram, node A is the parent node of nodes B and C.

A **child node** is a node that is immediately connected to a node above it. In the diagram, node D and E are the child nodes of node C.

Nodes D and E are also classified as **leaves**. A leaf is a node that has no child nodes. You can think of them as the end of the "branches" of the tree.

Tree nodes also have important properties:

* **Depth**: the length of the path from the root to that node. For example, in the diagram, node D has depth 2 because if you start at the root, you have to go through two edges to reach it.
* **Height**: the length of the path from that node down to a leaf. For example, node C has a height of 1 because it's one level above the leaf nodes.
* **Degree:** the number of child nodes each node has. In the diagram, node B has degree 0 because it's a leaf node, so it has no child nodes. Node C has degree 2 because it has two child nodes.

Trees also have a **height**. The height of a tree is the height of its root node.

There are many different types of trees, including Binary Trees, Binary Search Trees, AVL trees, Red-Black Trees, and B-Trees.

Binary Trees and Binary Search Trees
------------------------------------

These are two of the most commonly used types of trees.

A **binary tree** is a type of tree in which each node can have at most two child nodes, a left child node and a right child node. Yes, this means that the example that you have seen so far is a binary tree!

![The same binary tree example highlighting that it's a binary tree, with each node having at most two children.](https://cdn.freecodecamp.org/curriculum/lecture-transcripts/what-are-trees-and-tries-and-how-do-they-work-1.png)

A **binary search tree** is a more specific version of a binary tree, with a very particular ordering property.

To understand it, first you need to understand subtrees. A **subtree** is a section of a tree that is a tree itself.

In our tree example, nodes C, D, and E form a tree by themselves, so they are considered a subtree.

![A diagram highlighting a subtree within the main tree, showing nodes C, D, and E forming their own tree structure.](https://cdn.freecodecamp.org/curriculum/lecture-transcripts/what-are-trees-and-tries-and-how-do-they-work-3.png)

The ordering property of binary search trees (BST) establishes that for every node, all values in its left subtree are less than the node's value, and all values in its right subtree are greater than the node's value.

The left and right subtrees must also be binary search trees themselves.

This ordering makes search, insertion, and deletion operations very efficient if the tree is balanced.

A balanced tree is a tree in which the heights of the left and right subtrees of any node are very similar to make sure that operations remain efficient.

Tries
-----

Now that you know more about trees and binary search trees, let's dive into tries.

**Tries** are tree data structures used to store a set of strings.

Tries are also known as **prefix trees** because they are very efficient for operations that require finding strings based on their prefixes.

Each node in the trie represents a single character of a string.

The root node does not represent any particular character, so you can think of it as representing an empty string.

As you traverse the trie down from the root, the path to a node defines a specific prefix. To find a word, you follow that prefix until you reach the node with the word you are looking for.

Nodes that represent complete words are assigned end-of-word markers.

This is an example of a trie with the words "top", "tea" and "ten".

Notice how the words "tea" and "ten" share the same prefix "te", so the data structure follows the same path until the last character, which is marked as an end-of-word character. In this diagram, this is represented with a red border around the node:

![A trie data structure showing the words 'top', 'tea', and 'ten'. The root node branches to 't', which then branches to 'o' (leading to 'top') and 'e' (leading to 'tea' and 'ten'). End-of-word nodes are marked with red borders.](https://cdn.freecodecamp.org/curriculum/lecture-transcripts/what-are-trees-and-tries-and-how-do-they-work-4.png)

The worst-case time complexity for the search operation is O(L), where L is the length of the string that you are looking for.

Insertion is also efficient. This operation only requires creating new nodes for the characters that don't exist in the trie yet.

The great advantage of this data structure is that when multiple strings share the same prefix, their paths overlap, so the prefix itself is only stored once.

This efficiency makes tries perfect for implementing features like autocomplete and spell checkers.

However, tries are not efficient for all sets of strings. They can be inefficient if the set of strings has many unique characters. This would require storing many unique characters as individual nodes. These nodes would have to be traversed to find the words, which would not be optimal.

Now that you are familiar with the different types of trees and what they are used for, you can start using them in real-world scenarios. Knowing how to choose the right one is a valuable skill to have when you need to tackle challenges in your daily work.

---

# How Do Priority Queues and Heaps Work?

A **priority queue** is an abstract data type (ADT) that works similarly to a queue or stack, but with one key difference.

As you may already know, standard queues follow a FIFO (First-in, First-out) approach, where the first element added to the queue is the first one to be removed from the queue.

Stacks follow a LIFO (Last-in, First-out) approach, where the last element added to the stack is the first one to be removed from the stack.

Queues and stacks only consider the order of insertion of the elements.

However, priority queues take the "priority" of the elements into account. The priority is used to determine which element should be removed next.

Usually, the element with the highest priority is removed first, but some implementations may also choose to remove the element with the lowest priority first. This will depend on the requirements of your program.

Priority queues are very helpful for practical applications like finding the shortest path between two locations, scheduling tasks in operating systems, simulating traffic, compressing data, and managing networks.

In practice, priority queues are commonly implemented using a heap data structure.

A **heap** is a tree data structure with a very specific property called the **heap property**. This property determines the relationship between each node and its children, based on the type of heap.

There are two primary types of heaps:

* Max-heap
* Min-heap

In a **max-heap**, the value of each node is greater than or equal to the value of its children.

In this example, you can see a tree structure with the nodes 8, 7, 5, 2, and 1. Note that node 7 is greater than node 2 and node 1, following the heap property. This is true for all the other nodes as well.

![A max-heap tree structure showing nodes with values 8 at the root, 7 and 5 as children of 8, and 2 and 1 as children of 7, demonstrating that each parent node is greater than its children.](https://cdn.freecodecamp.org/curriculum/lecture-transcripts/how-do-priority-queues-and-heaps-work-1.png)

In contrast, in a **min-heap**, the value of each node is less than or equal to the value of its children.

In this example, we have nodes with values 4, 7, 9, 12, and 15. For example, node 7 is less than node 12 and node 15, following the heap property. This is also true for all the other nodes.

![A min-heap tree structure showing nodes with values 4 at the root, 7 and 9 as children of 4, and 12 and 15 as children of 7, demonstrating that each parent node is less than its children.](https://cdn.freecodecamp.org/curriculum/lecture-transcripts/how-do-priority-queues-and-heaps-work-2.png)

The heap property is key because it ensures that the maximum (or minimum) element (depending on the type of heap) always stays at the top, which makes it very easy to remove.

In practice, heaps are typically implemented as arrays to access parent and child nodes efficiently.

Using arrays simplifies the logic for accessing these values or "nodes" because behind the scenes, if the heap maintains the structure of a complete binary tree, the array implementation only requires simple mathematical operations based on their indices to find where the elements are located in memory.

Python has a `heapq` built-in module that you can use to work with an implementation of a min-heap.

It works by operating directly on Python lists, following specific steps that work with the elements as if the list was a heap, preserving the heap property.

To use this module, you just need to import it:

```python
import heapq
```

Then, you need to define an empty list. This will be the underlying data structure for the heap:

```python
my_heap = []
```

To add elements to the heap, you would call `heappush()`, passing the name of the heap and the element that you want to add as arguments. This will automatically add the element to the list where it should be, to preserve the heap property:

```python
heapq.heappush(my_heap, 9)
```

To get the element with the highest priority (in this case, the smallest value), you would call `heappop()`:

```python
heapq.heappop(my_heap)
```

`heappushpop()` combines both operations into one call.

This is more efficient than calling them in a sequence separately, especially when the heap is large, since it only performs one "heapify" operation to reorder the list as a heap:

```python
heapq.heappushpop(my_heap, 15)
```

If you already have a list and you want to transform it into a heap, you could call `heapify()`, passing the list as argument:

```python
heapq.heapify(my_heap)
```

But currently, we are sorting the elements by their values, right?

What if we want to sort them by their "priority" instead?

You could do this by storing tuples with this structure: `(priority, element)`.

Since tuples are compared element by element from left to right, the priorities will be compared first, and the decisions will be made based on them.

Please note that, in this case, lower values will represent higher priorities. This means that a tuple with priority of 1 will have a **higher** priority than a tuple with priority of 3:

```python
my_heap = []

heapq.heappush(my_heap, (3, "A"))
heapq.heappush(my_heap, (2, "B"))
heapq.heappush(my_heap, (1, "C"))
```

If you need elements with the same priority to be removed in the order that they were inserted, you could consider including a unique counter as the second element of your tuple to break the tie, like this `(priority, counter, element)`.

Now let's talk about the efficiency of heaps.

The average and worst case time complexities for inserting and extracting the minimum or maximum value from a heap (depending on the type of heap) are logarithmic, `O(log n)`, because the number of swaps required is usually proportional to the height of the heap, which is log(n).

The average and worst case time complexity for the "peek" operation is constant time, O(1). Peeking involves getting the minimum or maximum value (depending on the type of heap) without removing it.

The "heapify" operation, where the heap is built from an unsorted list, has linear time complexity, O(n), in the average and worst cases.

Similarly, both searching for and deleting an arbitrary element have linear average and worst case time complexities of O(n), since they potentially require traversing the entire heap.

And how much space do they require?

The space complexity of the heap is linear, O(n), where `n` is the number of elements it contains. It only needs to store the elements and a small additional overhead for the list object itself.

Priority queues and heaps are very important in computer science. They let you quickly find and use the most important elements from a list. This efficiency is crucial for many computer programs that perform critical real-world tasks, such as finding the fastest route on a map.

---

# What Are Graphs in Computer Science?

Graphs are data structures used to represent the connections or relationships between objects or entities. They're often used to model networks.

The types of networks that you can model with a graph include social networks, transportation networks, communications networks, and even recommendation systems.

For example, graphs can represent connections between users on a social media platform, or connections between cities on a road network.

They're very versatile.

A graph is often represented as a collection of points or circles connected by lines.

These circles and lines represent the two main components of a graph: nodes and edges.

![A simple graph showing five nodes labeled A, B, C, D, and E connected by edges. Node A connects to B, B connects to A, C, and D, C connects to B and D, D connects to B, C, and E, and E connects to D.](https://cdn.freecodecamp.org/curriculum/lecture-transcripts/what-are-graphs-in-computer-science-1.png)

**Nodes**, also known as vertices, represent the objects or entities that are part of the network modeled by the graph. They could be users, products, stations, cities, or any other entities in the model.

In this example, nodes are represented as circles and labeled with the letters A, B, C, D, and E to distinguish them visually.

**Edges** are the connections between the nodes. If two nodes are connected by an edge, that means that they're somehow connected in the network.

In this example, there are five edges connecting the different pairs of nodes. Node A is connected to node B. node B is connected to nodes A, C, and D and so on.

The specific meaning of the connection will depend on the context. It may be physical, like a real road that connects two cities, or it could be more abstract, like the connection between two users on a social media platform.

If two nodes are directly connected by an edge, like nodes A and B in this example, they're known as **adjacent nodes**.

![The same graph with nodes A and B highlighted to illustrate adjacent nodes - two nodes that are directly connected by an edge.](https://cdn.freecodecamp.org/curriculum/lecture-transcripts/what-are-graphs-in-computer-science-2.png)

Types of Graphs
---------------

There are different types of graphs with different characteristics and applications. Let's go over some of them.

### Undirected Graphs

**Undirected graphs** are graphs where the edges don't have a specific direction. This type of edge is usually represented with a straight line between the nodes.

![An example of an undirected graph where all edges are represented as straight lines without arrows, demonstrating that connections work in both directions between nodes.](https://cdn.freecodecamp.org/curriculum/lecture-transcripts/what-are-graphs-in-computer-science-1.png)

This means that, if there's an edge connecting nodes A and B, the connection works in both directions: from node A to node B and from node B to node A.

Depending on the network that is being modeled by the graph, this connection can have different meanings.

For example, if you're modeling connections between users of a social media platform, this means that user A is connected to user B and user B is connected to user A. The connection is bidirectional.

### Directed Graphs

In contrast, **directed graphs** are graphs where the edges do have a specific direction.

If there is a connection from node A to node B, that doesn't necessarily imply that there is a connection from node B to node A.

The edges of a directed graph are often represented as straight lines that end with an arrow to indicate the direction.

Here's an example. In this graph, you can go from node A to node B but not from node B to node A because of the direction of the edge.

![A directed graph example showing the same nodes as before but with arrows indicating specific one-way connections: from A to B, B to C, C to D, D to B, and D to E, demonstrating unidirectional edges.](https://cdn.freecodecamp.org/curriculum/lecture-transcripts/what-are-graphs-in-computer-science-4.png)

For example, if you are modeling a road network, this would be helpful to model one-way streets or roads. You can go from city A to city B through that road, but not from city B to city A. You'll need to take a different route.

If there is a two-way connection between the nodes of a directed graph, you can represent this with two directed edges between them.

Here you can see an example. You can go from node B to node D and from node D to node B because there are two edges connecting them, but each edge has a direction.

![A directed graph showing bidirectional connection between nodes B and D with two arrows, one pointing from B to D and another from D to B.](https://cdn.freecodecamp.org/curriculum/lecture-transcripts/what-are-graphs-in-computer-science-5.png)

Vertex Labeled Graphs
---------------------

A **vertex labeled graph** is a graph in which each node is associated with a label or identifier in addition to its data. These labels are used to identify the nodes, represent them visually, and store additional information about them.

For example, in a transportation network graph, nodes could be cities and their labels could be their names, coordinates, or any other characteristic that would be helpful for the purposes of the model.

Cyclic Graphs
-------------

**Cyclic graphs** are directed graphs with at least one cycle.

A **cycle** is a path that you can follow through the edges of a graph that will take you back to the initial node where you started.

In this example, we have a directed graph. If you look more closely, you'll notice that it has a cycle. If we start at node B, go to node C, and then to node D, we can go back to node B again through the directed edges.

This is a cycle, so this is a cyclic graph.

![A directed graph showing a cycle where you can start at node B, go to node C, then to node D, and back to node B, forming a complete cycle.](https://cdn.freecodecamp.org/curriculum/lecture-transcripts/what-are-graphs-in-computer-science-6.png)

Edge Labeled Graphs
-------------------

In **edge labeled graphs**, edges are associated with labels. These labels are usually drawn next to their corresponding edges.

Weighted Graphs
---------------

**Weighted graphs** are a specific type of edge labeled graph in which the labels on the edges represent values that can be compared and used to perform arithmetic operations.

Some edges have a higher weight, while others have a lower weight. These weights represent the "cost" of the edge.

For example, they may represent the distance between two cities or the time it takes to get from one city to the next.

This is an example of a weighted graph. We write each weight next to its corresponding edge. The "cost" of going from node B to node D is 3, and since this is an undirected graph, that's the same cost of going from node D back to node B.

![A weighted graph showing nodes connected by edges with numerical weights labeled next to each edge, such as weight 3 between nodes B and D.](https://cdn.freecodecamp.org/curriculum/lecture-transcripts/what-are-graphs-in-computer-science-7.png)

Directed Acyclic Graph
----------------------

Another very common type of graph in computer science is the **directed acyclic graph**, which is a directed graph with no cycles.

Here's an example. It's a directed graph because each edge has a direction.

It's acyclic because it doesn't have any cycles. Why? Notice that, if you start at a specific node, you cannot go back to it because of the direction of the edges.

![A directed acyclic graph (DAG) with connections from A to B, B to C, B to D, C to D, and D to E, demonstrating how the directional flow prevents any cycles from forming.](https://cdn.freecodecamp.org/curriculum/lecture-transcripts/what-are-graphs-in-computer-science-8.png)

Disconnected Graph
------------------

And the last type of graph that we'll cover in this lesson is the **disconnected graph**.

A disconnected graph is a graph with two or more groups of nodes that are not connected by any edges.

A real-world example would be a social media network, where you have two or more groups of people who don't know each other and who have no friends in common.

This is an example. The first component has the nodes A, B, and C. The second component has the nodes D and E. These components don't have any edges between them, so this is a disconnected graph.

![A disconnected graph showing two separate components: the first component has nodes A, B, and C connected in sequence (A connects to B, B connects to C), and the second component has nodes D and E connected to each other, with no connections between the two components.](https://cdn.freecodecamp.org/curriculum/lecture-transcripts/what-are-graphs-in-computer-science-9.png)

You can implement graphs in a variety of ways, including sets, functions, and arrays. You'll learn more about this in the coming lessons.

Understanding graphs and the characteristics of the different types of graphs is essential for solving a wide range of problems in computer science and other fields.

---

# How Do Matrices and Adjacency Lists Work?

Graphs are very powerful data structures made by a set of nodes, also known as vertices, and edges that connect them.

There are two common ways to implement graphs in your code:

* Adjacency matrices
* Adjacency lists

Let's look more into these, and go over their advantages and limitations.

Adjacency Matrices
------------------

We'll start with adjacency matrices.

An adjacency matrix is a two-dimensional list in which the rows and columns represent the graph's vertices.

The values in the matrix represent the edges or connections between the nodes.

For example, if you have a matrix stored in a variable named `matrix`, the value stored at `matrix[i][j]`, where `i` is the row and `j` is the column, represents the edge or connection between node `i` and node `j`.

The values may have different meanings depending on whether the graph is weighted or unweighted:

* If the graph is unweighted, a value of `1` means that there is an edge connecting these nodes, while a value of `0` means there is no edge between them.
* If the graph is weighted, the value would represent the weight of the edge that connects the nodes.

One of the great advantages of using an adjacency matrix is that checking if there is an edge between two nodes takes constant time `O(1)`. This is because the program only needs to find that particular value in the 2D list.

However, this efficiency in finding the edges comes with a tradeoff. Adjacency matrices have a large quadratic space requirement `O(V²)`, where `V` is the number of nodes in the graph.

This is inefficient for sparse graphs, which are graphs that only have a few edges. Why? Because if the graph is sparse, you will be storing many 0s in the matrix to represent the lack of edges between the nodes, and these 0s will still take space in memory.

Adjacency matrices are also inefficient for finding a node's neighbors because the program has to iterate over the entire row or column to find the 0s and 1s that represent the edges. In the worst case, this process can take O(V) time, where V is the number of nodes in the graph.

Let's see an example of an adjacency matrix for this particular graph:

![A graph with four nodes labeled A, B, C, and D. Node A connects to B, C, and D. Node B connects to A and D. Node C connects to A. Node D connects to A and B.](https://cdn.freecodecamp.org/curriculum/lecture-transcripts/how-do-matrices-and-adjacency-lists-work-1.png)

In the adjacency matrix:

* Each row represents a node. The first row represents node A, the second row represents node B, and so on.
* Each column represents a node too.
* Each value in the matrix represents whether there is an edge between each pair of nodes. A value of 0 means there isn't an edge connecting these nodes, while a value of 1 means there is an edge.

The values in the diagonal represent whether or not each node has a self-loop, an edge that connects the node to itself. In our example, they are all 0s because the graph doesn't have any self-loops.

This is a visual representation of the adjacency matrix to show you how the rows and columns represent the corresponding nodes.

For example, the first row is `[0, 1, 1, 1]` because node A has edges connecting it to nodes B, C, and D:

```python
#      A  B  C  D
# A   [0, 1, 1, 1],
# B   [1, 0, 0, 1],
# C   [1, 0, 0, 0],
# D   [1, 1, 0, 0]
```

And this is the same adjacency matrix, but implemented in Python code:

```python
adjacency_matrix = [
    [0, 1, 1, 1],  # The neighbors of A are B, C, and D
    [1, 0, 0, 1],  # The neighbors of B are A and D
    [1, 0, 0, 0],  # The only neighbor of C is A
    [1, 1, 0, 0]   # The neighbors of D are A and B
]
```

Adjacency Lists
---------------

Another common way to represent graphs is by using adjacency lists.

An adjacency list is an array or dictionary that stores all the neighbors of each node.

There are two ways to implement adjacency lists:

* As an array, where each index represents a node and the list stored at that index contains its neighbors.
* As a dictionary, where each key represents a node and the value associated to that key (a list) contains its neighbors.

Adjacency lists are more efficient than adjacency matrices in terms of space requirements. They have a `O(V + E)` space complexity, where `V` is the number of vertices (nodes) and `E` is the number of edges.

It's also efficient for finding all neighbor nodes, since this operation only requires accessing the list associated to the node.

However, there is also a tradeoff.

Adjacency lists are less efficient than adjacency matrices for determining if there is an edge between two nodes.

The search process can take `O(V)` time in the worst-case, since it may have to search through a very long list of neighbors if the node is connected to all the other nodes in the graph.

Here is an example of an adjacency list for this graph:

![A graph with four nodes labeled A, B, C, and D. Node A connects to B, C, and D. Node B connects to A and D. Node C connects to A. Node D connects to A and B. It's the same image as before.](https://cdn.freecodecamp.org/curriculum/lecture-transcripts/how-do-matrices-and-adjacency-lists-work-1.png)

This adjacency list is implemented as a dictionary. Every key in the dictionary represents a node, and the value associated to that key is a list with all the neighbors of the corresponding node:

```python
adjacency_list = {
    'A': ['B', 'C', 'D'],
    'B': ['A', 'D'],
    'C': ['A'],
    'D': ['A', 'B']
}
```

Alternatively, we could implement it as a 2D list, where each index represents a node. For example, index 0 represents node A, index 1 represents node B, and so on:

```python
adjacency_list = [
    ['B', 'C', 'D'],  # Neighbors of A (index 0)
    ['A', 'D'],       # Neighbors of B (index 1)
    ['A'],            # Neighbors of C (index 2)
    ['A', 'B']        # Neighbors of D (index 3)
]
```

Notice that even if this 2D list may look similar to the adjacency matrix, they are quite different.

* The adjacency matrix stores 0s, 1s, or other values that represent the edges or weights of the edges in the graph.
* The adjacency list stores the actual list of all the neighbors of each node.

This is a very important difference that you should be familiar with.

Both adjacency matrices and adjacency lists are very important for implementing graphs. Choosing between them depends on the graph's size and how you need to use the data. Adjacency matrices are helpful for dense graphs with many edges, while adjacency lists are usually the preferred choice for real-world scenarios, where sparse graphs are more common.

---

# How Do Depth First and Breadth First Search Work?

As you start working with data structures and algorithms, you'll soon realize that one of the common operations that you'll need to perform is visiting each node.

This process is known as "traversing" the data structure.

Traversals are used to do something with every single node in the data structure, like printing their values, finding a specific value, or performing certain operations on the nodes.

By systematically visiting each node, you make sure that the process won't skip any nodes.

But how do you determine the order in which you should traverse the data structure? Where should the process start, and how should the next node be selected?

Without a clear way to traverse the data structure, going through it would be like walking through a maze without a specific path to follow.

That's where algorithms like breadth-first search (BFS) and depth-first search (DFS) become really important. They are commonly used to traverse graphs and for finding a path between two nodes.

When they are used to traverse a data structure, they define the order in which the nodes should be visited to make sure that none of them is skipped.

Let's start with breadth-first search (BFS).

Breadth-First Search (BFS)
--------------------------

**Breadth-first search (BFS)** is an algorithm that visits all neighboring nodes before moving to the next level in the graph.

It can be used to find the shortest path between two nodes in an unweighted graph because it analyzes all the nodes at each level, so it finds the path with fewest edges first.

This algorithm is commonly implemented using a queue data structure to keep track of the nodes that have been visited. Queues follow the FIFO (first in, first out) method, where the first node that was added to the queue is the first one to be removed.

The algorithm works like this:

* You start at a specific node.
* That node is marked as visited and added to the queue.
* While the queue is not empty, the current node is removed from the queue (dequeued). Then, for each one of its neighbors, if the neighbor has not been visited, it is marked as visited and added to the queue.

One important consideration is that, since breadth-first search (BFS) requires storing a queue in memory, and this queue may have a large number of nodes, the space requirements of this algorithm can be considerable. This is especially true for graphs with a large number of nodes on the same level.

Let's see an example of BFS applied to a specific type of graph called a tree.

You will learn more about trees in an upcoming lesson, but they are essentially graphs with no cycles, where nodes are organized in a hierarchy. Cycles are paths that start and end at the same node.

Let's apply the breadth-first search (BFS) algorithm to this tree:

![A tree diagram showing nodes A through G arranged in a hierarchy. Node A is at the root, with children B and C. Node B has children D and E, and node C has children F and G.](https://cdn.freecodecamp.org/curriculum/lecture-transcripts/how-do-depth-first-and-breadth-first-search-work-1.png)

**Step 1:**

We start at the root of the tree, node A. We add A to the queue and immediately mark it as visited.

* **Queue:** `[A]`
* **Visited:** `{A}`

**Step 2:**

We dequeue node A. We add its unvisited children (node B and then node C), to the queue and mark them as visited.

* **Queue:** `[B, C]`
* **Visited:** `{A, B, C}`

The order in which nodes at the same level are added to the queue is defined by the implementation of the data structure and the order in which the edges (connections) are stored in the graph representation.

If the implementation is consistent, the specific order in which the nodes at the same level are traversed will not affect the correctness of the algorithm. It will still visit every node level by level.

**Step 3:**

We dequeue node B. We add its unvisited children, (node D and then node E), to the queue and mark them as visited.

* **Queue:** `[C, D, E]`
* **Visited:** `{A, B, C, D, E}`

**Step 4:**

We dequeue node C. We add its unvisited children, (node F and then node G), to the queue and mark them as visited.

* **Queue:** `[D, E, F, G]`
* **Visited:** `{A, B, C, D, E, F, G}`

**Step 5:**

We dequeue node D. This node does not have any unvisited children, so nothing changes in the visited set.

* **Queue:** `[E, F, G]`
* **Visited:** `{A, B, C, D, E, F, G}`

**Step 6:**

We dequeue node E. This node does not have any unvisited children, so nothing changes in the visited set.

* **Queue:** `[F, G]`
* **Visited:** `{A, B, C, D, E, F, G}`

**Step 7:**

We dequeue F. This node does not have any unvisited children, so nothing changes in the visited set.

* **Queue:** `[G]`
* **Visited:** `{A, B, C, D, E, F, G}`

**Step 8:**

We dequeue G. This node does not have any unvisited children, so nothing changes in the visited set.

* **Queue:** `[]`
* **Visited:** `{A, B, C, D, E, F, G}`

When the queue is empty, the traversal is complete.

The nodes were traversed in this order:

**A → B → C → D → E → F → G**

![The same tree diagram with arrows showing the BFS traversal order: A to B to C to D to E to F to G, demonstrating level-by-level visitation.](https://cdn.freecodecamp.org/curriculum/lecture-transcripts/how-do-depth-first-and-breadth-first-search-work-2.png)

Notice how the algorithm visits the nodes per level.

We start at node A, then move to the next level to visit nodes B and C, then to the next level to nodes D, E, F, and G. That is the core principle of breadth-first search (BFS).

Depth-First Search (DFS)
------------------------

While breadth-first search (BFS) first visits all the neighboring nodes at the same level, **depth-first search (DFS)** follows each branch as deep as possible before it backtracks.

You can imagine this algorithm as exploring a maze by choosing a specific path and following it until you reach a dead end or the exit. If you reach a dead end, you go back and choose a different path.

Depth-first search (DFS) is commonly used to solve puzzles with a single solution, detecting cycles in a graph, and finding connected graph components.

This algorithm can be implemented using recursion or a stack data structure to keep track of the visited nodes.

Stacks follow the LIFO (last in, first out) method, where the last node that was added to the stack is the first one to be removed from the stack.

The algorithm works like this:

* Start at a specific node.
* That node is marked as visited and added to the stack.
* While the stack is not empty, the current node is popped (removed). This is when we "visit" or process it (for example, by printing its value). Then, all of its unvisited neighbors are marked as visited and added to the stack.

One of the limitations of this algorithm is that it's not always guaranteed to find the shortest path between two nodes in an unweighted graph.

Let's see an example of Depth-First Search (DFS) applied to our tree example.

![The same tree diagram as before, showing nodes A through G in their hierarchical structure, ready for DFS demonstration.](https://cdn.freecodecamp.org/curriculum/lecture-transcripts/how-do-depth-first-and-breadth-first-search-work-3.png)

**Step 1:**

We start at the root node A. We mark it as visited and add it to the stack.

* **Stack:** `[A]`
* **Visited:** `{A}`

**Step 2:**

We pop node A from the stack.

Then, we add its unvisited children, node B and node C, to the stack. We'll add them in reverse order, `C` then `B`, so that `B` is on top (LIFO) and will be processed next. We also mark them as visited.

* **Stack:** `[C, B]`
* **Visited:** `{A, B, C}`

**Step 3:**

We pop node B from the stack.

Then, we add its unvisited children, node D and node E, to the stack in reverse order (`E` then `D`). We also mark them as visited.

* **Stack:** `[C, E, D]`
* **Visited:** `{A, B, C, D, E}`

**Step 4:**

We pop node D from the stack. This node has no children to add to the stack.

* **Stack:** `[C, E]`
* **Visited:** `{A, B, C, D, E}`

**Step 5:**

We pop node E from the stack. This node has no children to add to the stack.

* **Stack:** `[C]`
* **Visited:** `{A, B, C, D, E}`

**Step 6:**

We pop node C.

Then, we add its children, node F and node G, to the stack in reverse order (node G then node F) and we mark them as visited.

* **Stack:** `[G, F]`
* **Visited:** `{A, B, C, D, E, F, G}`

**Step 7:**

We pop node F from the stack. This node has no children to add to the stack.

* **Stack:** `[G]`
* **Visited:** `{A, B, C, D, E, F, G}`

**Step 8:**

We pop node G. This node has no children to add to the stack.

* **Stack:** `[]`
* **Visited:** `{A, B, C, D, E, F, G}`

When the stack is empty, the traversal is completed and all nodes have been visited.

The algorithm visited the nodes in this order:

**A → B → D → E → C → F → G**

![The tree diagram with numbers showing the DFS traversal order: A(1), B(2), D(3), E(4), C(5), F(6), G(7), demonstrating depth-first exploration of branches.](https://cdn.freecodecamp.org/curriculum/lecture-transcripts/how-do-depth-first-and-breadth-first-search-work-4.png)

Notice how we start at node A, and then move all the way down the tree to node B, and nodes D and E, before we move up again to node C and then nodes F and G. This is the core principle of depth-first search (DFS), traversing full paths before backtracking and finding other paths.

In this case, we solved this example using a stack. Alternatively, depth-first search (DFS) can be implemented using recursion, where the function processes the current node and then calls itself for each of its unvisited neighbors. The function call stack implicitly manages the LIFO (last-in, first-out) order.

Both breadth-first search (BFS) and depth-first search (DFS) are essential algorithms for traversing graphs and trees. Breadth-first search (BFS) explores nodes level by level, which is perfect for finding the shortest path in an unweighted graph. On the other hand, depth-first search (DFS) follows one branch as deep as possible before backtracking, which is perfect for solving mazes and detecting cycles. Understanding their pros and cons is helpful for choosing the right one for a particular problem.

---

## Module Review Component

# Graphs and Trees Review

Graphs Overview
---------------

A graph is a set of nodes (vertices) connected by edges (connections). Each node can connect to multiple other nodes, forming a network. The different types of graphs include:

* Directed: edges have a direction (from one node to another), often represented with straight lines and arrows.
* Undirected: edges have no direction, represented with simple lines.
* Vertex: each node is associated to a label or identifier.
* Cyclic: contains cycles (a path that starts and ends at the same node).
* Acyclic (DAG): does not contain cycles.
* Edge labeled: each edge has a label usually drawn next to corresponding edge.
* Weighted: edges have weights (values) associated with them, that can be used to perform arithmetic operations.
* Disconnected: contains two or more nodes that are not connected by any edges.

Graphs are used in various applications such as maps, networks, recommendation systems, dependency resolution.

Graph Traversals
----------------

This involves visiting all the nodes in a graph. The two main algorithms are:

* **Breadth-First Search (BFS)**

  + Uses a queue.
  + Explores level by level.
  + Finds shortest path in unweighted graphs.
* **Depth-First Search (DFS)**

  + Uses a stack (or recursion).
  + Explores a branch fully before backtracking.
  + Useful for cycle detection and path finding.

Graph Representations
---------------------

Graphs can be represented in two main ways:

* **Adjacency List**

  + Each node has a list of its neighbors.
  + Space efficient for sparse graphs.
  + Easy to iterate over neighbors.
* **Adjacency Matrix**

  + A 2D array where rows and columns represent nodes.
  + Space intensive for large graphs.
  + Fast to check if an edge exists between two nodes.

Trees
-----

A tree is a special type of graph that is acyclic and connected. Key properties include:

* They have no loops or cycles (paths where the start and end nodes are the same).
* They must be connected (every node can be reached from every other node).

### Common types of trees

The most common types of trees are:

* Binary Trees

  + Each node has at most two children, a left and a right child.
* Binary Search Trees (BST)

  + A binary tree in which every left child is less than its parent, and every right child is greater than its parent.

Tries
-----

Also known as prefix trees, they are used to store sets of strings, where each node represents a character.

Shared prefixes are stored only once, making them efficient for tasks like autocomplete and spell checking.

Search and insertion operations have a time complexity of O(L), where L is the length of the string.

Priority Queues
---------------

A priority queue is an abstract data type where each element has a priority.

Queues and stacks consider only the order of insertion, while priority queues consider the priority of elements.

Standard queues follow FIFO (First In First Out) and stacks follow LIFO (Last In First Out). However, in a priority queue, elements with higher priority are served before those with lower priority, regardless of their insertion order.

Heaps
-----

It's a specialized tree-based data structure with a very specific property called the heap property.

The heap property determines the relationship between parent and child nodes. There are two types of heaps:

* Max-Heap

  + The value of each parent node is greater than or equal to the values of its children.
  + The largest element is at the root.
* Min-Heap

  + The value of each parent node is less than or equal to the values of its children.
  + The smallest element is at the root.

### Python `heapq` module example

```python
import heapq

# Create empty heap
my_heap = []

# Insert elements
heapq.heappush(my_heap, 9)
heapq.heappush(my_heap, 3)
heapq.heappush(my_heap, 5)
print(my_heap) # [3, 9, 5]

# Remove smallest element
print(heapq.heappop(my_heap))  # 3
print(my_heap) # [5, 9]

# Push + Pop in one step
print(heapq.heappushpop(my_heap, 7)) # 5
print(my_heap) # [7, 9]

# Transform list into heap
nums = [5, 7, 3, 1]
heapq.heapify(nums)
```

### Using Priorities

```python
my_heap = []
heapq.heappush(my_heap, (3, "A"))
heapq.heappush(my_heap, (2, "B"))
heapq.heappush(my_heap, (1, "C"))

# Removes lowest number = highest priority
print(heapq.heappop(my_heap))  # (1, "C")
```

---

# Module 14: Dynamic Programming

# What Is Dynamic Programming and What Are Some Common Algorithms?

Dynamic programming is an algorithmic technique that solves complex problems by breaking them down into simpler subproblems and storing the results to avoid redundant calculations. This approach transforms problems that would normally take exponential time into ones that can be solved in polynomial time.

Core Principles of Dynamic Programming
--------------------------------------

Dynamic programming works when two key conditions are present in a problem.

* **Overlapping Subproblems**: The same smaller problems appear multiple times when solving the larger problem. Instead of recalculating these subproblems repeatedly, we store their solutions.
* **Optimal Substructure**: The optimal solution to the problem contains optimal solutions to its subproblems. This means we can build up the best solution by combining the best solutions to smaller parts.

Let's examine these concepts using the classic "climbing stairs" problem.

The Problem with Naive Recursion
--------------------------------

Consider the climbing stairs problem: you're climbing a staircase with `n` steps and can climb either 1 or 2 steps at a time. How many distinct ways can you reach the top?

```python
def climb_stairs_recursive(n):
    """Recursive approach"""
    if n <= 2:
        return n  # Base cases: 1 way for 1 step, 2 ways for 2 steps
    # To reach step n, we can come from step (n-1) or step (n-2)
    return climb_stairs_recursive(n-1) + climb_stairs_recursive(n-2)
```

This implementation has exponential time complexity because of massive redundant calculations. When calculating `climb_stairs(5)`, here's what happens:

* `climb_stairs(5)` calls `climb_stairs(4)` and `climb_stairs(3)`
* `climb_stairs(4)` calls `climb_stairs(3)` and `climb_stairs(2)`
* Now `climb_stairs(3)` is calculated **twice**
* `climb_stairs(3)` calls `climb_stairs(2)` and `climb_stairs(1)`
* `climb_stairs(2)` gets calculated **3 times total**

For just `n=5`, we make 9 function calls when we only need 5 unique calculations. As `n` grows, this redundancy explodes exponentially - `climb_stairs(30)` would require a few million function calls. The time complexity becomes `O(2^n)`, making it inefficient and impractical for larger values of `n`.

Dynamic Programming Solutions
-----------------------------

Dynamic programming eliminates this redundant computation through two main approaches:

### Memoization (Top-Down Approach)

Memoization stores the results of expensive function calls and returns the cached result when the same inputs occur again:

```python
def climb_stairs_memo(n, memo={}):
    """Dynamic programming with memoization"""
    # Check if we've already calculated this value
    if n in memo:
        return memo[n]  # Return cached result - O(1) lookup!
    
    # Base cases
    if n <= 2:
        return n
    
    # Calculate once and store in memo for future use
    memo[n] = climb_stairs_memo(n-1, memo) + climb_stairs_memo(n-2, memo)
    return memo[n]
```

Memoization is so much more efficient because each unique value from `1` to `n` is calculated exactly once. When we need `climb_stairs(3)` again, instead of recalculating it (which would trigger more recursive calls), we simply look it up in our memo dictionary in `O(1)` time.

Let's trace through the execution of `climb_stairs(5)` with the top-down approach to see how memoization eliminates redundant work:

```python
Call: climb_stairs_memo(5)
  memo = {} (empty)
  
  Call: climb_stairs_memo(4) 
    memo = {} (empty)
    
    Call: climb_stairs_memo(3)
      memo = {} (empty)
      
      Call: climb_stairs_memo(2) → returns 2 (base case)
      Call: climb_stairs_memo(1) → returns 1 (base case)
      
      Result: 2 + 1 = 3
      memo = {3: 3} (stored!)
    
    Call: climb_stairs_memo(2) → returns 2 (base case)
    
    Result: 3 + 2 = 5
    memo = {3: 3, 4: 5} (stored!)
  
  Call: climb_stairs_memo(3) → returns 3 (FROM MEMO - no recursion!)
  
  Result: 5 + 3 = 8
  memo = {3: 3, 4: 5, 5: 8}
```

**Efficiency comparison**

* **Naive recursive**: Makes 9 function calls with repeated calculations
* **Memoization**: Makes only 5 unique calculations, then reuses stored results
* **Time complexity**: Reduced from `O(2^n)` to `O(n)` since we make only `n` unique calculations
* **Space complexity**: `O(n)` for the memo storage and call stack
* **Real impact**: `climb_stairs(30)` drops from millions of function calls to about 30 unique subproblem calculations

### Tabulation (Bottom-Up Approach)

Tabulation builds the solution from the ground up, filling a table with solutions to subproblems:

```python
def climb_stairs_tabulation(n):
    """Dynamic programming with tabulation"""
    if n <= 2:
        return n
    
    # Create array to store results for all steps from 0 to n
    dp = [0] * (n + 1)
    dp[1] = 1  # 1 way to reach step 1
    dp[2] = 2  # 2 ways to reach step 2
    
    # Build up the solution iteratively
    for i in range(3, n + 1):
        # Ways to reach step i = ways to reach (i-1) + ways to reach (i-2)
        dp[i] = dp[i-1] + dp[i-2]
    
    return dp[n]
```

Tabulation eliminates recursion entirely by building the solution iteratively from the smallest subproblems up to the target.

Let's see the bottom-up approach in action to see how we build the solution systematically. Here's the iterative construction for `climb_stairs(5)`:

```python
Initial state:
dp = [0, 1, 2, 0, 0, 0]
     [0, 1, 2, 3, 4, 5] ← indices (step numbers)

Step by step construction:

i = 3:
  dp[3] = dp[2] + dp[1] = 2 + 1 = 3
  dp = [0, 1, 2, 3, 0, 0]
  
i = 4:
  dp[4] = dp[3] + dp[2] = 3 + 2 = 5
  dp = [0, 1, 2, 3, 5, 0]
  
i = 5:
  dp[5] = dp[4] + dp[3] = 5 + 3 = 8
  dp = [0, 1, 2, 3, 5, 8]

Final result: dp[5] = 8
```

**Key advantages of tabulation**

* **No recursion overhead**: Unlike memoization, there's no recursive call stack.
* **Predictable execution**: We calculate values in a predetermined order (1, 2, 3, 4, 5...).
* **Cache-friendly**: Sequential array access optimizes memory usage.
* **Easy to optimize**: Can reduce space complexity to `O(1)` since we only need the last two values.

```python
def climb_stairs_optimized(n):
    if n <= 2:
        return n
    
    prev2, prev1 = 1, 2  # Only store last two values
    for i in range(3, n + 1):
        current = prev1 + prev2
        prev2, prev1 = prev1, current
    return prev1
```

**Efficiency comparison**

* **Naive recursive**: 9 function calls for `n=5`, exponential growth.
* **Tabulation**: 3 simple additions for `n=5`, linear growth.
* **Time complexity**: `O(n)` instead of `O(2^n)`.
* **Space complexity**: `O(n)` for the array, or `O(1)` with optimization.
* **Predictable performance**: No risk of stack overflow for large inputs.

Both approaches reduce the time complexity from exponential `O(2^n)` to linear `O(n)`, a dramatic improvement that makes the difference between solving the problem in milliseconds versus waiting years for larger inputs.

Real-World Applications
-----------------------

Dynamic programming has widespread applications in computer science and beyond:

* **Route Optimization**: GPS systems use dynamic programming algorithms to find shortest paths between locations.
* **Text Processing**: Spell checkers and autocomplete features often rely on dynamic programming to calculate edit distances between words.
* **Financial Modeling**: Investment strategies and portfolio optimization frequently employ dynamic programming techniques.
* **Resource Allocation**: The knapsack problem and its variants appear in scheduling, budgeting, and resource management.

Practical Example: Coin Change Problem
--------------------------------------

The coin change problem is a classic coding challenge that, when solved using dynamic programming, demonstrates both of DP's key principles: optimal substructure and overlapping subproblems.

The coin change problem asks, "What's the minimum number of coins needed to make a target amount?"

Here's one solution using dynamic programming:

```python
def min_coins(amount, coins):
    """Find minimum number of coins needed to make the given amount"""
    # Initialize dp array with "infinity" - represents impossible to make
    dp = [float('inf')] * (amount + 1)
    dp[0] = 0  # Base case: 0 coins needed for amount 0
    
    # For each amount from 1 to target amount
    for i in range(1, amount + 1):
        # Try each coin denomination
        for coin in coins:
            if coin <= i:  # Can only use coin if it doesn't exceed current amount
                # Update minimum: current minimum vs (coins for remaining amount + 1)
                dp[i] = min(dp[i], dp[i - coin] + 1)
    
    # Return result if possible, -1 if impossible
    return dp[amount] if dp[amount] != float('inf') else -1

# Example usage:
# coins = [1, 3, 4], amount = 6
# dp[6] = min(dp[5]+1, dp[3]+1, dp[2]+1) = min(3+1, 1+1, 2+1) = 2
# Result: 2 coins (3 + 3)
```

And here's how the dynamic programming coin change algorithm works step by step for `coins = [1, 3, 4]`, `amount = 6`:

```python
Initial state:
dp = [0, ∞, ∞, ∞, ∞, ∞, ∞]
     [0, 1, 2, 3, 4, 5, 6] ← amounts

Building up the solution:

For amount = 1:
  Try coin 1: dp[1] = min(∞, dp[0] + 1) = min(∞, 0 + 1) = 1
  dp = [0, 1, ∞, ∞, ∞, ∞, ∞]

For amount = 2:
  Try coin 1: dp[2] = min(∞, dp[1] + 1) = min(∞, 1 + 1) = 2
  dp = [0, 1, 2, ∞, ∞, ∞, ∞]

For amount = 3:
  Try coin 1: dp[3] = min(∞, dp[2] + 1) = min(∞, 2 + 1) = 3
  Try coin 3: dp[3] = min(3, dp[0] + 1) = min(3, 0 + 1) = 1
  dp = [0, 1, 2, 1, ∞, ∞, ∞]

For amount = 4:
  Try coin 1: dp[4] = min(∞, dp[3] + 1) = min(∞, 1 + 1) = 2
  Try coin 3: dp[4] = min(2, dp[1] + 1) = min(2, 1 + 1) = 2
  Try coin 4: dp[4] = min(2, dp[0] + 1) = min(2, 0 + 1) = 1
  dp = [0, 1, 2, 1, 1, ∞, ∞]

For amount = 5:
  Try coin 1: dp[5] = min(∞, dp[4] + 1) = min(∞, 1 + 1) = 2
  Try coin 3: dp[5] = min(2, dp[2] + 1) = min(2, 2 + 1) = 2
  Try coin 4: dp[5] = min(2, dp[1] + 1) = min(2, 1 + 1) = 2
  dp = [0, 1, 2, 1, 1, 2, ∞]

For amount = 6:
  Try coin 1: dp[6] = min(∞, dp[5] + 1) = min(∞, 2 + 1) = 3
  Try coin 3: dp[6] = min(3, dp[3] + 1) = min(3, 1 + 1) = 2
  Try coin 4: dp[6] = min(2, dp[2] + 1) = min(2, 2 + 1) = 2
  dp = [0, 1, 2, 1, 1, 2, 2]

Final result: dp[6] = 2 (achieved with coins 3 + 3)
```

This solution demonstrates both key principles of dynamic programming. It has overlapping subproblems because finding the minimum coins for amount 6 requires knowing the solutions for amounts 5, 3, and 2. These same subproblems appear when calculating other amounts. It has optimal substructure because the optimal solution for any amount incorporates optimal solutions for smaller amounts. If we know the minimum coins for amount 3 is 1, then one way to make amount 6 is to use that solution plus one more coin of value 3.

Without DP, we'd need to try every possible combination of coins - an exponential number of possibilities. With DP, we build up the solution systematically:

* **Time complexity**: `O(amount × number of coins)` instead of exponential.
* **Space complexity**: `O(amount)` for the `dp` array.
* **No redundant work**: Each subproblem (finding minimum coins for each amount) is solved exactly once.
* **Reusable results**: Once we know the minimum coins for amount 3, we use this knowledge for all larger amounts that can benefit from it.

When to Use Dynamic Programming
-------------------------------

Dynamic programming is effective when:

* The problem can be broken down into overlapping subproblems.
* The problem exhibits optimal substructure.
* A naive recursive solution would involve repeated calculations.
* You need to optimize for time complexity at the cost of space complexity.

Common dynamic programming patterns include optimization problems (finding minimum/maximum values), counting problems (number of ways to achieve something), and decision problems that can be broken down into smaller decisions.

Dynamic programming transforms complex problems into manageable ones by systematically storing and reusing solutions to subproblems. Understanding this technique opens the door to solving a wide range of computational challenges efficiently.

---

## Module Review Component

# Dynamic Programming Review

Introduction to Dynamic Programming
-----------------------------------

* **Definition**: Dynamic programming is an algorithmic technique that solves complex problems by breaking them down into simpler subproblems and storing the results to avoid redundant calculations.
* **Overlapping Subproblems**: The same smaller problems appear multiple times when solving the larger problem. Instead of recalculating these subproblems repeatedly, we store their solutions.
* **Optimal Substructure**: The optimal solution to the problem contains optimal solutions to its subproblems. This means we can build up the best solution by combining the best solutions to smaller parts.

Dynamic Programming Solutions
-----------------------------

* **Memoization (Top-Down Approach)**: Memoization stores the results of expensive function calls and returns the cached result when the same inputs occur again.

```python
def climb_stairs_memo(n, memo={}):
    """Dynamic programming with memoization"""
    # Check if we've already calculated this value
    if n in memo:
        return memo[n]  # Return cached result - O(1) lookup!
    
    # Base cases
    if n <= 2:
        return n
    
    # Calculate once and store in memo for future use
    memo[n] = climb_stairs_memo(n-1, memo) + climb_stairs_memo(n-2, memo)
    return memo[n]
```

* **Tabulation (Bottom-Up Approach)**: Tabulation builds the solution from the ground up, filling a table with solutions to subproblems.

```python
def climb_stairs_tabulation(n):
    """Dynamic programming with tabulation"""
    if n <= 2:
        return n
    
    # Create array to store results for all steps from 0 to n
    dp = [0] * (n + 1)
    dp[1] = 1  # 1 way to reach step 1
    dp[2] = 2  # 2 ways to reach step 2
    
    # Build up the solution iteratively
    for i in range(3, n + 1):
        # Ways to reach step i = ways to reach (i-1) + ways to reach (i-2)
        dp[i] = dp[i-1] + dp[i-2]
    
    return dp[n]
```

Real-World Applications Using Dynamic Programming
-------------------------------------------------

* **Route Optimization**: GPS systems use dynamic programming algorithms to find shortest paths between locations.
* **Text Processing**: Spell checkers and autocomplete features often rely on dynamic programming to calculate edit distances between words.
* **Financial Modeling**: Investment strategies and portfolio optimization frequently employ dynamic programming techniques.
* **Resource Allocation**: The knapsack problem and its variants appear in scheduling, budgeting, and resource management.

When to Use Dynamic Programming
-------------------------------

You should consider using dynamic programming in the following scenarios:

* The problem can be broken down into overlapping subproblems.
* The problem exhibits optimal substructure.
* A naive recursive solution would involve repeated calculations.
* You need to optimize for time complexity at the cost of space complexity.

---

# Course Final Mega Review

# Python Review

What is Python?
---------------

* **Introduction**: Python is a general-purpose programming language known for its simplicity and ease of use. Python is used in many fields like data science and machine learning, web development, scripting and automation, embedded systems and IoT, and much more.
* **Common Use Cases**: Python is used in data science, machine learning, web development, cybersecurity, automation and microcomputers like the Raspberry Pi and MicroPython-compatible boards.

Python in Your Local Environment
--------------------------------

* **Installation**: The best way to install Python on Windows, Mac, and Linux is to download the installer from the official Python website (`https://www.python.org/`).
* **Terminal**: A text-based interface that lets you interact with your computer by typing commands. Each operating system comes with a default terminal app. On macOS, you can use the Terminal app. On Windows, you can use Command Prompt or PowerShell. On Linux, each desktop environment has its own default terminal app, like GNOME Terminal or Konsole.
* **IDE**: IDE stands for Integrated Development Environment and it has features including a code editor, testing tools, a terminal and more.
* **Popular Code Editors and IDEs for Python**: VS Code, PyCharm, and Spyder
* **Running Code Locally**: To run Python code, you have a few options. The first option is to click on the run button in VS Code which looks like a play button located in the upper right hand corner. That will open a terminal and run your Python script there.

Another option is to open a terminal and manually run the program. Here is an example to run a program called `main.py`:

```python
python main.py
```

You must run this command from the folder where `main.py` is saved. For example, if `main.py` is inside a folder called `python-projects`, first use the following in the terminal:

```python
cd python-projects
```

Then run:

```python
python main.py
```

Using the Python Interactive Shell
----------------------------------

* **Definition**: An interactive shell is a program that lets you type commands one at a time and see the results. Open up a terminal app and type in `python` and press `Enter`. This will start a Python interactive shell. The `>>>` symbol means Python is waiting for you to type a command. Try printing `"Hello, world!"` to the terminal:

```python
print("Hello, world!")
```

You should see the text appear like this:

```python
>>> print("Hello, world!")
Hello, world!
```

After the text is printed, Python goes back to the following:

```python
>>>
```

This means you can type in another command.

* **Read, Evaluate, Print, Loop cycle (REPL)**: Whenever you type in commands, the interpreter will read the input, evaluate it, print the result and loop back to show the `>>>` so you can type more commands.

Variables
---------

* **Declaring Variables**: To declare a variable, you start with the variable name followed by the assignment operator (`=`) and then the value. This can be a number, string, boolean, etc. Here are some examples:

```python
name = 'John Doe'
age = 25
```

* **Naming Conventions for Variables**: Here are the naming conventions you should use for variables:

  + Variable names can only start with a letter or an underscore (\_), not a number.
  + Variable names can only contain alphanumeric characters (a-z, A-Z, 0-9) and underscores (\_).
  + Variable names are case-sensitive — `age`, `Age`, and `AGE` are all considered unique.
  + Variable names cannot be one of Python’s reserved keywords such as `if`, `class`, or `def`.
  + Variable names with multiple words are separated by underscores. E.g., `snake_case`.

Comments
--------

* **Single Line Comments**: These types of comments should be used for short notes you wish to leave in your code.

```python
# This is a single line comment
```

* **Multi-line Strings**: These types of strings can be used to leave larger notes or to comment out sections of code.

```python
"""
This is a multi-line string.
Here is some code commented out.

name = 'John Doe'
age = 25
"""
```

* **`print()` Function**: To print data to the console, you can use the `print()` function like this:

```python
print('Hello world!') # Hello world!
```

Common Data Types in Python
---------------------------

* **Introduction**: Python is a dynamically-typed language like JavaScript, meaning you don't need to explicitly declare types for variables. The language knows what the type of a variable is based on what you assign to the variable.
* **Integer**: A whole number without decimals:

```python
my_integer_var = 10
print('Integer:', my_integer_var) # Integer: 10
```

* **Float**: A number with decimals:

```python
my_float_var = 4.50
print('Float:', my_float_var) # Float: 4.5
```

* **String**: A sequence of characters wrapped in quotes:

```python
my_string_var = 'hello'
print('String:', my_string_var) # String: hello
```

* **Boolean**: A value representing either `True` or `False`:

```python
my_boolean_var = True
print('Boolean:', my_boolean_var) # Boolean: True
```

* **Set**: An unordered collection of unique elements:

```python
my_set_var = {7, 5, 8}
print('Set:', my_set_var) # Set: {7, 5, 8}
```

* **Dictionary**: A collection of key-value pairs, enclosed in curly braces:

```python
my_dictionary_var = {"name": "Alice", "age": 25}
print('Dictionary:', my_dictionary_var) # Dictionary: {'name': 'Alice', 'age': 25}
```

* **Tuple**: An immutable ordered collection, enclosed in parentheses:

```python
my_tuple_var = (7, 5, 8)
print('Tuple:', my_tuple_var) # Tuple: (7, 5, 8)
```

* **Range**: A sequence of numbers, often used in loops:

```python
my_range_var = range(5)
print(my_range_var) # range(0, 5)
```

* **List**: An ordered collection of elements that supports different data types:

```python
my_list = [22, 'Hello world', 3.14, True]
print(my_list) # [22, 'Hello world', 3.14, True]
```

* **None**: A special value that represents the absence of a value:

```python
my_none_var = None
print('None:', my_none_var) # None: None
```

Immutable and Mutable Types
---------------------------

* **Immutable Types**: These types cannot change once declared, although you can point their variables at something new, which is called reassignment. They include integer, float, complex, boolean, string, tuple, range, and `None`.
* **Mutable Types**: These types can change once declared. You can add, remove, or update their items. They include collection types such as list, set, and dictionary.
* **`type()` Function**: To see the type for a variable, you can use the `type()` function like this:

```python
greeting = 'Hello there!'
age = 21

print(type(greeting)) # <class 'str'>
print(type(age)) # <class 'int'>
```

* **`isinstance()` Function**: This is used to check if a variable matches a specific data type:

```python
greeting = 'Hello world'
name = 'John Doe'

print(isinstance(greeting, str)) # True
print(isinstance(name, int)) # False
```

Working with Strings
--------------------

* **Definition**: As you recall from JavaScript, strings are immutable which means you cannot change them after they have been created. In Python, you can use either single or double quotes. It is recommended to choose a rule and stick with it:

```python
developer = 'Jessica'
city = "Los Angeles"
```

* **Accessing Characters from Strings**: You can access characters from strings by using bracket notation like this:

```python
my_str = 'Hello world'

print(my_str[0])  # H
print(my_str[6])  # w

print(my_str[-1])  # d
print(my_str[-2]) # l
```

* **Escaping Strings**: You can use a backslash (`\`) if your string contains quotes like this:

```python
msg = 'It\'s a sunny day'
quote = "She said, \"Hello!\""
```

* **String Concatenation**: To concatenate strings, you can use the `+` operator like this:

```python
developer = 'Jessica'
print('My name is ' + developer + '.') # My name is Jessica.
```

Another way to concatenate strings is by using the `+=` operator. This is used to perform concatenation and assignment in the same step like this:

```python
greeting = 'My name is '
developer = 'Jessica.'

greeting += developer
print(greeting) # My name is Jessica.
```

* **`f-strings`**: This is short for formatted string literals. It allows you to handle interpolation and also do some concatenation with a compact and readable syntax:

```python
developer = 'Jessica'
greeting = f'My name is {developer}.'
print(greeting) # My name is Jessica.
```

* **String Slicing**: This is when you can extract portions of a string. Here is the basic syntax:

```python
str[start:stop:step]
```

The start position represents the index where the extraction should begin. The stop position is where the slice should end. This position is non-inclusive. The step position represents the interval to increment for the slicing. Here are some examples:

```python
message = 'Python is fun!'

print(message[0:6])  # Python
print(message[7:])  # is fun!
print(message[::2])  # Pto sfn
```

* **Getting the Length of a String**: The `len()` function is used to return the number of the characters in the string:

```python
developer = 'Jessica'

print(len(developer)) # 7
```

Working with the `in` operator
------------------------------

* **`in` Operator**: This returns a boolean that specifies whether the character or characters exist in the string or not:

```python
my_str = 'Hello world'

print('Hello' in my_str)  # True
print('hey' in my_str)    # False
print('hi' in my_str)    # False
print('e' in my_str)  # True
print('f' in my_str)  # False
```

Common String Methods
---------------------

* **`upper()`**: This string method returns a new string with all characters converted to uppercase:

```python
developer = 'Jessica'

print(developer.upper()) # JESSICA
```

* **`lower()`**: This string method returns a new string with all characters converted to lowercase:

```python
developer = 'Jessica'

print(developer.lower()) # jessica
```

* **`strip()`**: This string method returns a copy of the string with specified leading and trailing characters removed (if no argument is passed to the method, it removes leading and trailing whitespace).

```python
greeting = '  hello world  '

trimmed_my_str = greeting.strip()
print(trimmed_my_str)  # 'hello world'
```

* **`replace()`**: This returns a new string with all occurrences of the old string replaced by a new one.

```python
greeting = 'hello world'

replaced_my_str = greeting.replace('hello', 'hi')
print(replaced_my_str)  # 'hi world'
```

* **`split()`**: This is used to split a string into a list using a specified separator. A separator is a string specifying where the split should happen.

```python
dashed_name = 'example-dashed-name'

split_words = dashed_name.split('-')
print(split_words)  # ['example', 'dashed', 'name']
```

* **`join()`**: This is used to join elements of an iterable into a string with a separator. An iterable is a collection of elements that can be looped over like a list, string or a tuple.

```python
example_list = ['example', 'dashed', 'name']

joined_str = ' '.join(example_list)
print(joined_str)  # example dashed name
```

* **`startswith(prefix)`**: This string method returns a boolean indicating if a string starts with the specified prefix:

```python
developer = 'Naomi'

result = developer.startswith('N')
print(result)  # True
```

* **`endswith(suffix)`**: This string method returns a boolean indicating if a string ends with the specified suffix:

```python
developer = 'Naomi'

result = developer.endswith('N')
print(result)  # False
```

* **`find()`**: This string method returns the index for the first occurrence of a substring. If one is not found, then `-1` is returned:

```python
developer = 'Naomi'

result = developer.find('N')
print(result)  # 0

city = 'Los Angeles'
print(city.find('New')) # -1
```

* **`count(substring)`**: This string method counts how many times a substring appears in a string:

```python
city = 'Los Angeles'
print(city.count('e')) # 2
```

* **`capitalize()`**: This string method returns a new string with the first character capitalized and the other characters lowercased:

```python
dessert = 'chocolate cake'
print(dessert.capitalize()) # Chocolate cake
```

* **`isupper()`**: This string method returns `True` if all letters in the string are uppercase and `False` if otherwise:

```python
dessert = 'chocolate cake'
print(dessert.isupper()) # False
```

* **`islower()`**: This string method returns `True` if all letters in the string are lowercase and `False` if otherwise:

```python
dessert = 'chocolate cake'
print(dessert.islower()) # True
```

* **`title()`**: This string method returns a new string with the first letter of each word capitalized:

```python
city = 'los angeles'
print(city.title()) # Los Angeles
```

* **`maketrans()`**: This string method is used to create a table of 1 to 1 character mappings for translation. It is often used with the `translate()` method which applies that table to a string and return the translated result.

```python
trans_table = str.maketrans('abc', '123')
print(trans_table) # {97: 49, 98: 50, 99: 51}

result = 'abcabc'.translate(trans_table)
print(result)  # 123123
```

Common Operations used with Integers and Floats
-----------------------------------------------

* **Basic Math Operations**: In Python, you can do basic math operations with integers and floats including addition, subtraction, multiplication and division:

```python
int_1 = 56
int_2 = 12
float_1 = 5.4
float_2 = 12.0

# Addition

print('Integer Addition:', int_1 + int_2) # Integer Addition: 68
print('Float Addition:', float_1 + float_2) # Float Addition: 17.4

# Subtraction

print('Int Subtraction:', int_1 - int_2) # Int Subtraction: 44
print('Float Subtraction:',  float_2 - float_1) # Float Subtraction: 6.6

# Multiplication

print('Int Multiplication:', int_1 * int_2) # Int Multiplication: 672
print('Float Multiplication:', float_2 * float_1) # Float Multiplication: 64.80000000000001

# Division

print('Division:', int_1 / int_2) # Division: 4.666666666666667
print('Float Division:', float_2 / float_1) # Float Division: 2.222222222222222
```

When you add a float and an integer, the result will be converted to a float like this:

```python
int_1 = 56
float_1 = 5.4

print(int_1 + float_1) # 61.4
```

* **Modulo Operator (`%`)**: This returns the remainder when a number is divided by another number:

```python
int_1 = 56
int_2 = 12

print(int_1 % int_2) # 8
```

* **Floor Division (`//`)**: This operator is used to divide two numbers and round down the result to the nearest whole number:

```python
int_1 = 56
int_2 = 12

print(int_1 // int_2) # 4
```

* **Exponentiation Operator (`**`)**: This operator is used to raise a number to the power of another:

```python
int_1 = 4
int_2 = 2

print(int_1 ** int_2) # 16
```

* **`float()` Function**: You can use this function to convert an integer to a float.

```python
num = 4

print(float(num)) # 4.0
```

* **`int()` Function**: You can use this function to convert a float to an integer.

```python
num = 4.0

print(int(num)) # 4
```

* **`round()` Function**: This is used to round a number to the nearest whole integer:

```python
num_1 = 3.4
num_2 = 7.7

print(round(num_1)) # 3
print(round(num_2)) # 8
```

* **`abs()` Function**: This is used to return the absolute value of a number:

```python
num = -13

print(abs(num)) # 13
```

* **`pow()` Function**: This is used to raise a number to the power of another:

```python
result = pow(2, 3) 
print(result)  # 8
```

Augmented Assignments
---------------------

* **Definition**: Augmented assignment combines a binary operation with an assignment in one step. It takes a variable, applies an operation to it with another value, and stores the result back into the same variable.

```python
# Addition assignment 
my_var = 10
my_var += 5

print(my_var) # 15

# Subtraction assignment
count = 14
count -= 3

print(count) # 11

# Multiplication assignment 
product = 65
product *= 7

print(product) # 455

# Division assignment 
price = 100
price /= 4

print(price) # 25.0

# Floor Division assignment 
total_pages = 23
total_pages //= 5

print(total_pages) # 4

# Modulo assignment 
bits = 35
bits %= 2

print(bits) # 1

# Exponentiation assignment 
power = 2
power **= 3

print(power) # 8
```

There are other augmented assignment operators too, like those for bitwise operators. They include `&=`, `^=`, `>>=`, and `<<=`.

Working with Functions
----------------------

* **Definition**: Functions are reusable pieces of code that take inputs (arguments) and return an output. To call a function, you need to reference the function name followed by a set of parenthesis:

```python
# Defining a function

def get_sum(num_1, num_2):
    return num_1 + num_2

result = get_sum(3, 4) # function call
print(result) # 7
```

If a function does not explicitly return a value, then the default return value is `None`:

```python
def greet():
    print('hello') 

result = greet() # hello
print(result) # None
```

You can also supply default values to parameters like this:

```python
def get_sum(num_1, num_2=2):
    return num_1 + num_2

result = get_sum(3) 
print(result) # 5
```

If you call the function without the correct number of arguments, you will get a `TypeError`:

```python
def calculate_sum(a, b):
    print(a + b)

calculate_sum()

# TypeError: calculate_sum() missing 2 required positional arguments: 'a' and 'b'
```

Common Built-in Functions
-------------------------

* **`input()` Function**: This is used to prompt the user for some input:

```python
name = input('What is your name?') # User types 'Kolade' and presses Enter  
print('Hello', name) # Hello Kolade
```

* **`int()` Function**: This is used to convert a number, boolean, or a numeric string into an integer:

```python
print(int(3.14)) # 3
print(int('42')) # 42
print(int(True)) # 1
print(int(False)) # 0
```

Scope in Python
---------------

* **Local Scope**: This is when a variable declared inside a function or class can only be accessed within that function or class.

```python
def my_func():
    num = 10
    print(num)
```

* **Enclosing Scope**: This is when a function that's nested inside another function can access the variables of the function it's nested within.

```python
def outer_func():
    msg = 'Hello there!'
    
    def inner_func():
        print(msg)
    inner_func()

print(outer_func()) # Hello there!
```

* **Global Scope**: This refers to variables that are declared outside any functions or classes which can be accessed from anywhere in the program.

```python
tax = 0.70 

def get_total(subtotal):
    total = subtotal + (subtotal * tax)
    return total

print(get_total(100))  # 170.0
```

* **Built-in Scope**: Reserved names in Python for predefined functions, modules, keywords, and objects.

```python
print(str(45)) # '45'
print(type(3.14)) # <class 'float'>
print(isinstance(3, str)) # False
```

Comparison Operators
--------------------

* **Equal (`==`)**: Checks if two values are equal:

```python
print(3 == 4) # False
```

* **Not equal (`!=`)**: Checks if two values are not equal:

```python
print(3 != 4) # True
```

* **Strictly greater than (`>`)**: Checks if one value is greater than another:

```python
print(3 > 4) # False
```

* **Strictly less than (`<`)**: Checks if one value is less than another:

```python
print(3 < 4) # True
```

* **Greater than or equal(`>=`)**: Checks if one value is greater than or equal to another:

```python
print(3 >= 4) # False
```

* **Less than or equal(`<=`)**: Checks if one value is less than or equal to another:

```python
print(3 <= 4) # True
```

Working with `if`, `elif` and `else` Statements
-----------------------------------------------

* **`if` Statements**: These are conditions used to determine if something is true or not. If the condition evaluates to `True`, then that block of code will run.

```python
age = 18

if age >= 18:
    print('You are an adult') # You are an adult
```

* **`elif` Clause**: These are conditions that come after an `if` statement. If the `elif` condition evaluates to `True`, then that block of code will run.

```python
age = 16

if age >= 18:
    print('You are an adult')
elif age >= 13:
    print('You are a teenager')  # You are a teenager
```

* **`else` Clause**: This will run if no other conditions evaluate to `True`.

```python
age = 12

if age >= 18:
    print('You are an adult')
elif age >= 13:
    print('You are a teenager')
else:
    print('You are a child')  # You are a child
```

You can also use nested `if` statements like this:

```python
is_citizen = True
age = 25

if is_citizen:
    if age >= 18:
        print('You are eligible to vote') # You are eligible to vote
else:
    print('You are not eligible to vote')
```

Truthy and Falsy Values
-----------------------

* **Definition**: In Python, every value has an inherent boolean value, or a built-in sense of whether it should be treated as `True` or `False` in a logical context. Many values are considered truthy, that is, they evaluate to `True` in a logical context. Others are falsy, meaning they evaluate to `False`. Here are some examples of falsy values:

```python
None
False
Integer 0
Float 0.0
Empty strings ''
```

Other values like non-zero numbers, and non-empty strings are truthy.

Working with the `bool()` Function
----------------------------------

* **Definition**: If you want to check whether a value is truthy or falsy, you can use the built-in `bool()` function. It explicitly converts a value to its boolean equivalent and returns `True` for truthy values and `False` for falsy values. Here are a few examples:

```python
print(bool(False)) # False
print(bool(0))  # False
print(bool('')) # False

print(bool(True)) # True
print(bool(1)) # True
print(bool('Hello')) # True
```

Boolean Operators and Short-circuiting
--------------------------------------

* **Definition**: These are special operators that allow you to combine multiple expressions to create more complex decision-making logic in your code. There are three Boolean operators in Python: `and`, `or`, and `not`.
* **`and` Operator**: This operator takes two operands and returns the first operand if it is falsy, otherwise, it returns the second operand. Both operands must be truthy for an expression to result in a truthy value.

```python
is_citizen = True
age = 25

print(is_citizen and age) # 25
```

You can also use the `and` operator in conditionals like this:

```python
is_citizen = True
age = 25

if is_citizen and age >= 18:
    print('You are eligible to vote') # You are eligible to vote
else:
    print('You are not eligible to vote')
```

* **`or` Operator**: This operator returns the first operand if it is truthy, otherwise, it returns the second operand. An `or` expression results in a truthy value if at least one operand is truthy. Here is an example:

```python
age = 19
is_employed = False

print(age or is_employed) # 19
```

Just like with the `and` operator, you can use the `or` operator in conditionals like this:

```python
age = 19
is_student = True

if age < 18 or is_student:
    print('You are eligible for a student discount') # You are eligible for a student discount
else:
    print('You are not eligible for a student discount')
```

* **Short-circuiting**: The `and` and `or` operators are known as short-circuit operators. Short-circuiting means Python checks values from left to right and stops as soon as it determines the final result.
* **`not` Operator**: This operator takes a single operand and inverts its boolean value. It converts truthy values to `False` and falsy values to `True`. Unlike the previous operators we looked at, `not` always returns `True` or `False`. Here are some examples:

```python
print(not '') # True, because empty string is falsy
print(not 'Hello') # False, because non-empty string is truthy
print(not 0) # True, because 0 is falsy
print(not 1) # False, because 1 is truthy
print(not False) # True, because False is falsy
print(not True) # False, because True is truthy
```

Here is an example of the `not` operator in a conditional:

```python
is_admin = False

if not is_admin:
    print('Access denied for non-administrators.') # Access denied for non-administrators.
else:
    print('Welcome, Administrator!')
```

Python Lists
------------

* **Introduction**: In Python, the list data type is an ordered sequence of elements that can be composed of strings, numbers or even other lists. Lists are mutable and zero based indexed.

```python
cities = ['Los Angeles', 'London', 'Tokyo']
```

* **Accessing Elements in a List**: To access an element from the `cities` list, you can reference its index number in the sequence:

```python
cities = ['Los Angeles', 'London', 'Tokyo']
cities[0] # Los Angeles
```

* **Accessing Elements Using Negative Indexing**: To access the last element of any list, you can use `-1` as the index number:

```python
cities = ['Los Angeles', 'London', 'Tokyo']
cities[-1] # Tokyo
```

* Negative indexing is used to access elements starting from the end of the list instead of the beginning at index `0`.
* **Creating Lists Using the `list()` constructor**: Lists can also be created using the `list()` constructor. The `list()` constructor is used to convert an iterable into a list:

```python
developer = 'Jessica'

print(list(developer)) 
# Result: ['J', 'e', 's', 's', 'i', 'c', 'a']
```

* **Finding the Length of a List**: You can use the `len()` function to get the length of a list:

```python
numbers = [1, 2, 3, 4, 5]
len(numbers) # 5
```

* **List Mutability**: Lists are mutable, meaning you can update any element in the list as long as you pass in a valid index number. To update lists at a particular index, you can assign a new value to that index:

```python
programming_languages = ['Python', 'Java', 'C++', 'Rust']
programming_languages[0] = 'JavaScript'
print(programming_languages) # ['JavaScript', 'Java', 'C++', 'Rust']
```

* **Index Out of Range Error**: If you pass in an index (either positive or negative) that is out of bounds for the list, then you will receive an `IndexError`:

```python
programming_languages = ['Python', 'Java', 'C++', 'Rust']
programming_languages[10] = 'JavaScript'

"""
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
IndexError: list assignment index out of range
"""
```

* **Removing Elements from a List**: Elements can be removed from a list using the `del` keyword:

```python
developer = ['Jane Doe', 23, 'Python Developer']
del developer[1]
print(developer) # ['Jane Doe', 'Python Developer']
```

* **Checking if an Element Exists in a List**: The `in` keyword can be used to check if an element exists in a list:

```python
programming_languages = ['Python', 'Java', 'C++', 'Rust']

'Rust' in programming_languages # True
'JavaScript' in programming_languages # False
```

* **Nesting Lists**: Lists can be nested inside other lists:

```python
developer = ['Alice', 25, ['Python', 'Rust', 'C++']]
```

* To access the nested list, you will need to access it using index `2` since lists are zero-based indexed.

```python
developer = ['Alice', 25, ['Python', 'Rust', 'C++']]
developer[2] # ['Python', 'Rust', 'C++']
```

* To further access the second language from that nested list, you will need to access it using index `1`:

```python
developer = ['Alice', 25, ['Python', 'Rust', 'C++']]
developer[2][1] # Rust
```

* **Unpacking Values from a List:** Unpacking values from a list is a technique used to assign values from a list to new variables. Here is an example to unpack the `developer` list into new variables called `name`, `age` and `job` like this:

```python
developer = ['Alice', 34, 'Rust Developer']
name, age, job = developer
```

* If the number of variables on the left side of the assignment operator doesn't match the total number of items in the list, then you will receive a `ValueError`.
* **Collecting Remaining Items From a List**: To collect any remaining elements from a list, you can use the asterisk (`*`) operator like this:

```python
developer = ['Alice', 34, 'Rust Developer']
name, *rest = developer
```

* **Slicing Lists**: Slicing is the concept of accessing a portion of a list by using the slice operator `:`. To slice a list that starts at index `1` and ends before index `3`, you can use the following syntax:

```python
desserts = ['Cake', 'Cookies', 'Ice Cream', 'Pie']
desserts[1:3] # ['Cookies', 'Ice Cream']
```

* **Step Intervals**: It is also possible to specify a step interval which determines how much to increment between the indices. Here is an example if you want to extract a list of just even numbers using slicing:

```python
numbers = [1, 2, 3, 4, 5, 6]
numbers[1::2] # [2, 4, 6]
```

List Methods
------------

* **append()**: Used to add an item to the end of the list. Here is an example of using the `append()` method to add the number `6` to this `numbers` list:

```python
numbers = [1, 2, 3, 4, 5]
numbers.append(6)
print(numbers) # [1, 2, 3, 4, 5, 6]
```

* **Appending lists**: The `append()` method can also be used to add one list at the end of another:

```python
numbers = [1, 2, 3, 4, 5]
even_numbers = [6, 8, 10]

numbers.append(even_numbers)
print(numbers) # [1, 2, 3, 4, 5, [6, 8, 10]]
```

* **extend()**: Used to add multiple items to the end of a list. Here is an example of adding the numbers `6`, `8`, and `10` to the end of the `numbers` list:

```python
numbers = [1, 2, 3, 4, 5]
even_numbers = [6, 8, 10]

numbers.extend(even_numbers)
print(numbers) # [1, 2, 3, 4, 5, 6, 8, 10]
```

* **insert()**: Used to insert an item at a specific index in the list. Here is an example of using the `insert()` method:

```python
numbers = [1, 2, 3, 4, 5]
numbers.insert(2, 2.5)

print(numbers) # [1, 2, 2.5, 3, 4, 5]
```

* **remove():** Used to remove an item from the list. The `remove()` method will only remove the first occurrence of an item in the list:

```python
numbers = [1, 2, 3, 4, 5, 5, 5]
numbers.remove(5)

print(numbers) # [1, 2, 3, 4, 5, 5]
```

* **pop()**: Used to remove a specific item from the list and return it:

```python
numbers = [1, 2, 3, 4, 5]
numbers.pop(1) # The number 2 is returned
```

* If you don't specify an element for the `pop` method, then the last element is removed.

```python
numbers = [1, 2, 3, 4, 5]
numbers.pop() # The number 5 is returned
```

* **clear()**: Used to remove all items from the list:

```python
numbers = [1, 2, 3, 4, 5]
numbers.clear()

print(numbers) # []
```

* **sort()**: The `sort()` method is used to sort the elements in place. Here is an example of sorting a random list of `numbers` in place:

```python
numbers = [19, 2, 35, 1, 67, 41]
numbers.sort()

print(numbers) # [1, 2, 19, 35, 41, 67]
```

* **sorted()**: A built-in function that returns a new sorted list instead of modifying the original list:

```python
numbers = [19, 2, 35, 1, 67, 41]
sorted_numbers = sorted(numbers)

print(sorted_numbers) # [1, 2, 19, 35, 41, 67]
print(numbers) # [19, 2, 35, 1, 67, 41]
```

* **reverse()**: Used to reverse the order of the elements in a list:

```python
numbers = [6, 5, 4, 3, 2, 1]
numbers.reverse()

print(numbers) # [1, 2, 3, 4, 5, 6]
```

* **index()**: Used to find the first index where an element can be found in a list:

```python
programming_languages = ['Rust', 'Java', 'Python', 'C++']
programming_languages.index('Java') # 1
```

* If the element cannot be found using the `index()` method, then the result will be a `ValueError`.

Tuples in Python
----------------

* **Definition**: A tuple is a Python data type used to create an ordered sequence of values. Tuples can contain a mixed set of data types:

```python
developer = ('Alice', 34, 'Rust Developer')
```

* Tuples are immutable, meaning the elements in the tuple cannot be changed once created. If you try to update one of the items in the tuple, you will get a `TypeError`:

```python
programming_languages = ('Python', 'Java', 'C++', 'Rust')
programming_languages[0] = 'JavaScript'

"""
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: "tuple" object does not support item assignment
"""
```

* **Accessing Elements from a Tuple**: To access an element from a tuple, use bracket notation and the index number:

```python
developer = ('Alice', 34, 'Rust Developer')
developer[1] # 34
```

* Negative indexing can be used to access elements starting from the end of the tuple:

```python
numbers = (1, 2, 3, 4, 5)
numbers[-2] # 4
```

* If you try to pass in an index number that exceeds or equals the length of the tuple, then you will receive an `IndexError`:

```python
numbers = (1, 2, 3, 4, 5)
numbers[7]

"""
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
IndexError: tuple index out of range
"""
```

* A tuple can also be created using the `tuple()` constructor. Within the constructor, you can pass in different iterables like strings, lists and even other tuples.

```python
developer = 'Jessica'

print(tuple(developer)) 
# Result: ('J', 'e', 's', 's', 'i', 'c', 'a')
```

* **Verifying Items in a Tuple**: To check if an item is in a tuple, you can use the `in` keyword like this:

```python
programming_languages = ('Python', 'Java', 'C++', 'Rust')

'Rust' in programming_languages # True
'JavaScript' in programming_languages # False
```

* **Unpacking Tuples**: Items can be unpacked from a tuple like this:

```python
developer = ('Alice', 34, 'Rust Developer')
name, age, job = developer
```

* If you need to collect any remaining elements from a tuple, you can use the asterisk (`*`) operator like this:

```python
developer = ('Alice', 34, 'Rust Developer')
name, *rest = developer
```

* **Slicing Tuples**: Slicing can be used to extract a portion of a tuple. For example, the items `pie` and `cookies` can be sliced into a separate tuple:

```python
desserts = ('cake', 'pie', 'cookies', 'ice cream')
desserts[1:3] # ('pie', 'cookies')
```

* **Removing Items from Tuples**: Removing an item from a tuple will raise a `TypeError` as tuples are immutable:

```python
developer = ('Jane Doe', 23, 'Python Developer')
del developer[1]

"""
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: "tuple" object doesn't support item deletion
"""
```

* **When to use a Tuple vs a List?**: If you need a dynamic collection of elements where you can add, remove and update elements, then you should use a list. If you know that you are working with a fixed and immutable collection of data, then you should use a tuple.

Common Tuple Methods
--------------------

* **`count()`**: Used to determine how many times an item appears in a tuple. For example, you can check how many times the language `'Rust'` appears in the tuple:

```python
programming_languages = ('Rust', 'Java', 'Python', 'C++', 'Rust')
programming_languages.count('Rust') # 2
```

* If the specified item in the `count()` method is not present at all in the tuple, then the return value will be `0`:

```python
programming_languages = ('Rust', 'Java', 'Python', 'C++', 'Rust')
programming_languages.count('JavaScript') # 0
```

* If no arguments are passed to the `count()` method, then Python will return a `TypeError`.
* **index()**: Used to find the index where a particular item is present in the tuple. Here is an example of using the `index()` method to find the index for the language `'Java'`:

```python
programming_languages = ('Rust', 'Java', 'Python', 'C++', 'Rust')
programming_languages.index('Java') # 1
```

* If the specified item cannot be found, then Python will return a `ValueError`.
* You can pass an optional start index to the `index()` method to specify where to start searching for the item in the tuple:

```python
programming_languages = ('Rust', 'Java', 'Python', 'C++', 'Rust', 'Python')
programming_languages.index('Python', 3) # 5
```

* You can also pass in an optional end index to the `index()` method to specify where to stop searching for the item in the tuple:

```python
programming_languages = ('Rust', 'Java', 'Python', 'C++', 'Rust', 'Python', 'JavaScript', 'Python')
programming_languages.index('Python', 2, 5) # 2
```

* **`sorted()`**: Used to sort the elements in any iterable and return a new sorted list. Here is an example of creating a new list of numbers using the `sorted()` function:

```python
numbers = (13, 2, 78, 3, 45, 67, 18, 7)
sorted(numbers) # [2, 3, 7, 13, 18, 45, 67, 78]
```

* **Modifying Sorting Behavior**: You can customize the sorting behavior for an iterable using the optional `reverse` and `key` arguments. Here is an example of using the `key` argument to sort items in a tuple by length:

```python
programming_languages = ('Rust', 'Java', 'Python', 'C++', 'Rust', 'Python')
sorted(programming_languages, key=len)

# Result
# ['C++', 'Rust', 'Java', 'Rust', 'Python', 'Python']
```

* You can create a new list of values in reverse order, using the `reverse` argument like this:

```python
programming_languages = ('Rust', 'Java', 'Python', 'C++', 'Rust', 'Python')

print(sorted(programming_languages, reverse=True))

# Result
# ['Rust', 'Rust', 'Python', 'Python', 'Java', 'C++']
```

Loops in Python
---------------

* **Definition**: Loops are used to repeat a block of code for a set number of times.
* **`for` loop**: Used to iterate over a sequence (like a list, tuple or string) and execute a block of code for each item in that sequence. Here is an example of using a `for` loop to iterate through a list and print each language to the console:

```python
programming_languages = ['Rust', 'Java', 'Python', 'C++']

for language in programming_languages:
    print(language)

"""
Result 

Rust
Java
Python
C++
"""
```

* Here is an example of using a `for` loop to loop through the string `code` and print out each character:

```python
for char in 'code':
    print(char)

"""
Result 

c
o
d
e
"""
```

* `for` loops can be nested. Here is an example of using a nested `for` loop:

```python
categories = ['Fruit', 'Vegetable']
foods = ['Apple', 'Carrot', 'Banana']

for category in categories:
    for food in foods:
        print(category, food)

"""
Result

Fruit Apple
Fruit Carrot
Fruit Banana
Vegetable Apple
Vegetable Carrot
Vegetable Banana
"""
```

* **`while` loop**: Repeats a block of code until the condition is `False`. Here is an example of using a `while` loop for a guessing game:

```python
secret_number = 3
guess = 0

while guess != secret_number:
    guess = int(input('Guess the number (1-5): '))
    if guess != secret_number:
        print('Wrong! Try again.')

print('You got it!')

"""
Result

Guess the number (1-5): 2
Wrong! Try again.
Guess the number (1-5): 1
Wrong! Try again.
Guess the number (1-5): 3
You got it!
"""
```

* **`break` and `continue` statements**: Used in loops to modify the execution of a loop.
* The `break` statement is used to exit the loop immediately when a certain condition is met. Here is an example of using the `break` statement for a list of `developer_names`:

```python
developer_names = ['Jess', 'Naomi', 'Tom']

for developer in developer_names:
    if developer == 'Naomi':
        break
    print(developer)
```

* The `continue` statement is used to skip that current iteration and move onto the next iteration of the loop. Here is an example to use the `continue` statement instead of a `break` statement:

```python
developer_names = ['Jess', 'Naomi', 'Tom']

for developer in developer_names:
    if developer == 'Naomi':
        continue
    print(developer)
```

* Both `for` and `while` loops can be combined with an `else` clause, which is executed only when the loop was not terminated by a `break`:

```python
words = ['sky', 'apple', 'rhythm', 'fly', 'orange']

for word in words:
    for letter in word:
        if letter.lower() in 'aeiou':
            print(f"'{word}' contains the vowel '{letter}'")
            break
    else:
        print(f"'{word}' has no vowels")
```

Ranges and Their Use in Loops
-----------------------------

* **The `range()` function**: Used to generate a sequence of integers.

```python
range(start, stop, step)
```

* The required `stop` argument is an integer (non-inclusive) that represents the end point for the sequence of numbers being generated. Here is an example of using the `range()` function:

```python
for num in range(3):
    print(num)
```

* If a `start` argument is not specified, then the default will be `0`. By default the sequence of integers will increment by `1`. You can use the optional `step` argument to change the default increment value. Here is an example of generating a sequence of even integers from 2 up to but not including 11 (i.e., includes 10)

```python
for num in range(2, 11, 2):
    print(num)
```

* If you don't provide any arguments to the `range()` function, then you will get a `TypeError`.
* The `range()` function only accepts integers for arguments and not floats. Using floats will also result in a `TypeError`:

```python
ERROR!
Traceback (most recent call last):
  File "<main.py>", line 1, in <module>
TypeError: 'float' object cannot be interpreted as an integer
```

* You can use a negative integer for the `step` argument to generate a sequence of integers in decrementing order:

```python
for num in range(40, 0, -10):
    print(num)
```

* The `range()` function can also be used to create a list of integers by using it with the `list` constructor. The `list` constructor is used to convert an iterable into a list. Here is an example of generating a list of even integers between 2 and 10 inclusive:

```python
numbers = list(range(2, 11, 2))
print(numbers) # [2, 4, 6, 8, 10]
```

`enumerate()` and `zip()` functions in Python
---------------------------------------------

* **`enumerate()`**: used to iterate over a sequence and keep track of the index for each item in that sequence. The `enumerate()` function takes an iterable as an argument and returns an `enumerate` object that consist of the index and value of each item in the iterable.

```python
languages = ['Spanish', 'English', 'Russian', 'Chinese']

for index, language in enumerate(languages):
    print(f'Index {index} and language {language}')

# Result
# Index 0 and language Spanish
# Index 1 and language English
# Index 2 and language Russian
# Index 3 and language Chinese
```

* The `enumerate()` function can also be used outside of a `for` loop:

```python
languages = ['Spanish', 'English', 'Russian', 'Chinese']

print(list(enumerate(languages)))
# [(0, 'Spanish'), (1, 'English'), (2, 'Russian'), (3, 'Chinese')]
```

* The `enumerate()` function also accepts an optional `start` argument that specifies the starting value for the count. If this argument is omitted, then the count will begin at `0`.
* **`zip()`** : Used to iterate over multiple iterables in parallel. Here's an example using the `zip()` function to iterate over `developers` and `ids`:

```python
developers = ['Naomi', 'Dario', 'Jessica', 'Tom']
ids = [1, 2, 3, 4]

for name, id in zip(developers, ids):
    print(f'Name: {name}')
    print(f'ID: {id}')


"""
Result

Name: Naomi
ID: 1
Name: Dario
ID: 2
Name: Jessica
ID: 3
Name: Tom
ID: 4
"""
```

List Comprehensions in Python
-----------------------------

* **Definition**: List comprehension allows you to create a new list in a single line by combining the loop and the condition directly within square brackets. This makes the code shorter and often easier to read.

```python
even_numbers = [num for num in range(21) if num % 2 == 0]
print(even_numbers)
```

Iterable Functions
------------------

* **`filter()`**: Used to filter elements from an iterable based on a condition. It returns an iterator that contains only the elements that satisfy the condition. Here is an example of creating a new list of just words longer than four characters:

```python
words = ['tree', 'sky', 'mountain', 'river', 'cloud', 'sun']

def is_long_word(word):
    return len(word) > 4

long_words = list(filter(is_long_word, words))
print(long_words) # ['mountain', 'river', 'cloud']
```

* **`map()`**: Used to apply a function to each item in an iterable and return a new iterable with the results. Here is an example of using the `map()` function to convert a list of celsius temperatures to fahrenheit:

```python
celsius = [0, 10, 20, 30, 40]

def to_fahrenheit(temp):
    return (temp * 9/5) + 32

fahrenheit = list(map(to_fahrenheit, celsius))
print(fahrenheit) # [32.0, 50.0, 68.0, 86.0, 104.0]
```

* **`sum()`**: Used to get the sum from an iterable like a list or tuple. Here is an example of using the `sum()` function:

```python
numbers = [5, 10, 15, 20]
total = sum(numbers)
print(total) # Result: 50
```

* You can also pass in an optional `start` argument which sets the initial value for the summation. Here is an updated example using the `start` argument as a positional argument:

```python
numbers = [5, 10, 15, 20]
total = sum(numbers, 10) # positional argument
print(total) # 60
```

* You can also choose to use the `start` argument as a keyword argument like this instead:

```python
numbers = [5, 10, 15, 20]
total = sum(numbers, start=10) # keyword argument
print(total) # 60
```

Lambda Functions
----------------

* **Definition**: A lambda function in Python is a concise way to create a function without a name (an anonymous function).
* Lambda functions are often used as an argument to another function. Here is an example of a lambda function:

```python
numbers = [1, 2, 3, 4, 5]

even_numbers = list(filter(lambda x: x % 2 == 0, numbers))
print(even_numbers)  # [2, 4]
```

* Best practices for using lambda functions include not assigning them to a variable, keeping them simple and readable, and using them for short, one-off functions.

Dictionaries
------------

* **Dictionaries**: Dictionaries are built-in data structures that store collections of key-value pairs. Keys need to be immutable data types. This is the general syntax of a Python dictionary:

```python
dictionary = {
    key1: value1,
    key2: value2
}
```

* **`dict()` Constructor**: The `dict()` constructor is an alternative way to build the dictionary. You pass a list of tuples as an argument to the `dict()` constructor. These tuples contain the key as the first element and the value as the second element.

```python
pizza = dict([('name', 'Margherita Pizza'), ('price', 8.9), ('calories_per_slice', 250), ('toppings', ['mozzarella', 'basil'])])
```

* **Bracket Notation**: To access the value of a key-value pair, you can use the syntax known as bracket notation.

```python
dictionary[key]
```

Common Dictionary Methods
-------------------------

* **`get()` Method**: The `get()` method retrieves the value associated with a key. It's similar to the bracket notation, but it lets you set a default value, preventing errors if the key doesn't exist.

```python
dictionary.get(key, default)
```

* **`keys()` and `values()` Methods**: The `keys()` and `values()` methods return a view object with all the keys and values in the dictionary, respectively. A view object is a way to see the content of a dictionary without creating a separate copy of the data.

```python
pizza = {
    'name': 'Margherita Pizza',
    'price': 8.9,
    'calories_per_slice': 250
}

pizza.keys()
# dict_keys(['name', 'price', 'calories_per_slice'])

pizza.values()
# dict_values(['Margherita Pizza', 8.9, 250])
```

* **`items()` Method**: The `items()` method returns a view object with all the key-value pairs in the dictionary, including both the keys and the values.

```python
pizza.items()
# dict_items([('name', 'Margherita Pizza'), ('price', 8.9), ('calories_per_slice', 250)])
```

* **`clear()` Method**: The `clear()` method removes all the key-value pairs from the dictionary.

```python
pizza.clear()
```

* **`pop()` Method**: The `pop()` method removes the key-value pair with the key specified as the first argument and returns its value. If the key doesn't exist, it returns the default value specified as the second argument. If the key doesn't exist and the default value is not specified, a `KeyError` is raised.

```python
pizza.pop('price', 10)
pizza.pop('total_price') # KeyError
```

* **`popitem()` Method**: In Python 3.7 and above, the `popitem()` method removes the last inserted item.

```python
pizza.popitem()
```

* **`update()` Method**: The `update()` method updates the key-value pairs with the key-value pairs of another dictionary. If they have keys in common, their values are overwritten. New keys will be added to the dictionary as new key-value pairs.

```python
pizza.update({ 'price': 15, 'total_time': 25 })
```

Looping Over a Dictionary
-------------------------

* **Iterating Over Values**: If you need to iterate over the values in a dictionary, you can write a `for` loop with `values()` to get all the values of a dictionary.

```python
products = {
    'Laptop': 990,
    'Smartphone': 600,
    'Tablet': 250,
    'Headphones': 70,
}

for price in products.values():
    print(price)
```

Output:

```python
990
600
250
70
```

* **Iterating Over Keys**: If you need to iterate over the keys in the `products` dictionary above, you can write `products.keys()` or `products` directly.

```python
for product in products.keys():
    print(product)
    
# Or

for product in products:
    print(product)
```

Output:

```python
Laptop
Smartphone
Tablet
Headphones
```

* **Iterating Over Key-Value Pairs**: If you need to iterate over the keys and their corresponding values simultaneously, you can iterate over `products.items()`. You get individual tuples with the keys and their corresponding values.

```python
for product in products.items():
    print(product)
```

Output:

```python
('Laptop', 990)
('Smartphone', 600)
('Tablet', 250)
('Headphones', 70)
```

To store the key and value in separate loop variables, you need to separate them with a comma. The first variable stores the key, and the second stores the value.

```python
for product, price in products.items():
    print(product, price)
```

Output:

```python
Laptop 990
Smartphone 600
Tablet 250
Headphones 70
```

* **`enumerate()` Function**: If you need to iterate over a dictionary while keeping track of a counter, you can call the `enumerate()` function. The function returns an `enumerate` object, which assigns an integer to each item, like a counter. You can start the counter from any number, but by default, it starts from 0.

Assigning the index and item to separate loop variables is the common way to use `enumerate()`. For example, with `products.items()`, you can get the entire key-value pair in addition to the index:

```python
for index, product in enumerate(products.items()):
    print(index, product)
```

Output:

```python
0 ('Laptop', 990)
1 ('Smartphone', 600)
2 ('Tablet', 250)
3 ('Headphones', 70)
```

To customize the initial value of the count, you can pass a second argument to `enumerate()`. For example, here we are starting the count from 1.

```python
for index, product in enumerate(products.items(), 1):
    print(index, product)
```

Output:

```python
1 ('Laptop', 990)
2 ('Smartphone', 600)
3 ('Tablet', 250)
4 ('Headphones', 70)
```

Sets
----

* **Sets**: Sets are built-in data structures in Python that do not allow duplicate values. Sets are mutable and unordered, which means that their elements are not stored in any specific order, so you cannot use indices or keys to access them. Also, sets can only contain values of immutable data types, like numbers, strings, and tuples.
* **Defining a Set**: To define a set, you need to write its elements within curly brackets and separate them with commas.

```python
my_set = {1, 2, 3, 4, 5}
```

* **Defining an Empty Set**: If you need to define an empty set, you must use the `set()` function. Only writing empty curly braces will automatically create a dictionary.

```python
set() # Set
{}    # Dictionary
```

Common Set Methods
------------------

* **`add()` Method**: You can add an element to a set with the `add()` method, passing the new element as an argument.

```python
my_set.add(6)
```

* **`remove()` and `discard()` Methods**: To remove an element from a set, you can either use the `remove()` method or the `discard()` method, passing the element you want to remove as an argument. The `remove()` method will raise a `KeyError` if the element is not found while the `discard()` method will not.

```python
my_set.remove(4)
my_set.discard(4)
```

* **`clear()` method**: The `clear()` method removes all the elements from the set.

```python
my_set.clear()
```

Mathematical Set Operations
---------------------------

* **`issubset()` and `issuperset()` Methods**: The `issubset()` and the `issuperset()` methods check if a set is a subset or superset of another set, respectively.

```python
my_set = {1, 2, 3, 4, 5}
your_set = {2, 3, 4, 5}

print(your_set.issubset(my_set)) # True
print(my_set.issuperset(your_set)) # True
```

* **`isdisjoint()` Method**: The `isdisjoint()` method checks if two sets are disjoint, if they don't have elements in common.

```python
my_set = {1, 2, 3}
your_set = {4, 5, 6}

print(my_set.isdisjoint(your_set)) # True
```

* **Union Operator (`|`)**: The union operator `|` returns a new set with all the elements from both sets.

```python
my_set = {1, 2, 3}
your_set = {4, 5, 6}

my_set | your_set # {1, 2, 3, 4, 5, 6}
```

* **Intersection Operator (`&`)**: The intersection operator `&` returns a new set with only the elements that the sets have in common.

```python
my_set = {1, 2, 3, 4, 5}
your_set = {2, 3, 4, 6}

my_set & your_set # {2, 3, 4}
```

* **Difference Operator (`-`)**: The difference operator `-` returns a new set with the elements of the first set that are not in the other set.

```python
my_set = {1, 2, 3, 4, 5}
your_set = {2, 3, 4, 6}

my_set - your_set # {1, 5}
```

* **Symmetric Difference Operator (`^`)**: The symmetric difference operator `^` returns a new set with the elements that are either in the first or the second set, but not both.

```python
my_set = {1, 2, 3, 4, 5}
your_set = {2, 3, 4, 6}

my_set ^ your_set # {1, 5, 6}
```

* **`in` Operator**: You can check if an element is in a set or not with the `in` operator.

```python
print(5 in my_set)
```

Python Standard Library
-----------------------

* **Python Standard Library**: A library gives you pre-written and reusable code, like functions, classes, and data structures, that you can reuse in your projects. Python has an extensive standard library with built-in modules that implement standardized solutions for many problems and tasks. Some examples of popular built-in modules are `math`, `random`, `re` (short for "regular expressions"), and `datetime`.

Import Statement
----------------

* **Import Statement**: To access the elements defined in built-in modules, you use an import statement. Import statements are generally written at the top of the file. Import statements work the same for functions, classes, constants, variables, and any other elements defined in the module.
* **Basic Import Statement**: You can use the `import` keyword followed by the name of the module:

```python
import module_name
```

Then, if you need to call a function from that module, you would use dot notation, with the name of the module followed by the name of the function.

```python
module_name.function_name()
```

For example, you would write the following in your code to import the `math` module and get the square root of 36:

```python
import math

math.sqrt(36)
```

* **Importing a Module with a Different Name**: If you need to import the module with a different name (also known as an "alias"), you can use `as` followed by the alias at the end of the import statement. This is often used for long module names or to avoid naming conflicts.

```python
import module_name as module_alias
```

For example, to refer to the `math` module as `m` in your code, you can assign an alias like this:

```python
import math as m
```

Then, you can access the elements of the module using the alias:

```python
m.sqrt(36)
```

* **Importing Specific Elements**: If you don't need everything from a module, you can import specific elements using `from`. In this case, the import statement starts with `from`, followed by the module name, then the `import` keyword, and finally the names of the elements you want to import.

```python
from module_name import name1, name2
```

Then, you can use these names without the module prefix in your Python script. For example:

```python
from math import radians, sin, cos

angle_degrees = 40
angle_radians = radians(angle_degrees)

sine_value = sin(angle_radians)
cos_value = cos(angle_radians)

print(sine_value) # 0.6427876096865393
print(cos_value)  # 0.766044443118978
```

This is helpful, but it can result in naming conflicts if you already have functions or variables with the same name. Keep it in mind when choosing which type of import statement you want to use.

If you need to assign aliases to these names, you can do so as well, using the `as` keyword followed by the alias.

```python
from module_name import name1 as alias1, name2 as alias2
```

* **Import Statement with Asterisk (`*`)**: The asterisk tells Python that you want to import everything in that module, but you want to import it so that you don't need to use the name of the module as a prefix.

```python
from module_name import *
```

For example, if you use this to import the `math` module, you'll be able to call any function defined in that module without specifying the name of the module as a prefix.

```python
from math import *
print(sqrt(36))  # 6.0
```

However, this is generally discouraged because it can lead to namespace collisions and make it harder to know where names come from.

`if __name__ == '__main__'`
---------------------------

* **`__name__` Variable**: `__name__` is a special built-in variable in Python. When a Python file is executed directly, Python sets the value of this variable to the string `"__main__"`. But if the Python file is imported as a module into another Python script, the value of the `__name__` variable is set to the name of that module.

This is why you'll often find this conditional in Python scripts. It contains the code that you only want to run **only** if the Python script is running as the main program.

```python
if __name__ == '__main__': 
    # Code
```

Common Errors in Python
-----------------------

* **SyntaxError**: The error Python raises when your code does not follow its syntax rules. For example, the code `print("Hello there"` will lead to a syntax error with the message, `SyntaxError: '(' was never closed`, because the code is missing a closing parenthesis.
* **NameError**: Python raises a `NameError` when you try to access a variable or function you have not defined. For instance, if you have the line `print(username)` in your code without having a `username` variable defined first, you will get a name error with the message `NameError: name 'username' is not defined`.
* **TypeError**: This is the error Python throws when you perform an operation on two or more incompatible data types. For example, if you try to add a string to a number, you'll get the error `TypeError: can only concatenate str (not "int") to str`.
* **IndexError**: You'll get an `IndexError` if you access an index that does not exist in a list or other sequences like tuple and string. For example, in a `Hello world` string, the index of the last character is `10`. If you go ahead and access a character this way, `greet = "hello world"; print(greet[11])`, you'll get an error with the message `IndexError: string index out of range`.
* **AttributeError**: Python raises this error when you try to use a method or property that does not exist in an object of that type. For example, calling `.append()` on a string like `"hello".append("!")` will lead to an error with the message `AttributeError: 'str' object has no attribute 'append'`.

Good Debugging Techniques in Python
-----------------------------------

* **Using the `print` function**: Inserting `print()` statements around various points in your code while debugging helps you see the values of variables and how your code flows.
* **Using Python's Built-in Debugger (`pdb`)**: Python provides a `pdb` module for debugging. It's a part of the Python's standard library, so it's always available to use. With `pdb`, you can set a trace with the `set_trace()` function so you can start stepping through the code and inspect variables in an interactive way.
* **Leveraging IDE Debugging Tools**: Many integrated development environments (IDEs) and code editors like Pycharm and VS Code offer debugging tools with breakpoints, step execution, variable inspection, and other debugging features.

Exception Handling
------------------

* **`try...except`**: This is used to execute a block of code that might raise an exception. The `try` block is where you anticipate an error might occur, while the `except` block takes a specified exception and runs if that specified error is raised. Here's an example:

  ```
  try:
    print(22 / 0)
  except ZeroDivisionError:
    print('You can\'t divide by zero!')
    # You can't divide by zero!
  ```

  You can also chain multiple `except` blocks so you can handle more types of exceptions:

  ```
  try:
    number = int(input('Enter a number: '))
    print(22 / number)
  except ZeroDivisionError:
    print('You cannot divide by zero!')
    # You cannot divide by zero! prints when you enter 0
  except ValueError:
    print('Please enter a valid number!')
    # Please enter a valid number! prints when you don't enter an integer
  ```
* **`else` and `finally`**: These blocks extend `try...except`. If no exception occurs, the `else` block runs. The `finally` block always runs regardless of errors.

  ```
  try:
    result = 100 / 4
  except ZeroDivisionError:
    print('You cannot divide by zero!') # This will not run
  else:
    print(f'Result is {result}') # Result is 25.0
  finally:
    print('Execution complete!') # Execution complete!
  ```
* **Exception Object**: This lets you access the exception itself for better debugging and printing the direct error message. To access the exception object, you need to use the `as` keyword. Here's an example:

  ```
  try:
      value = int('This will raise an error')
  except ValueError as e:
      print(f'Caught an error: {e}')
      # Caught an error: invalid literal for int() with base 10: 'This will raise an error'
  ```
* **The `raise` Statement**: This allows you to manually raise an exception. You can use it to throw an exception when a certain condition is met. Here's an example:

  ```
  def divide(a, b):
      if b == 0:
          raise ZeroDivisionError('You cannot divide by zero')
      return a / b
  ```

Exception Signaling
-------------------

The `raise` statement is also useful when you create your own custom exceptions, as you can use it to throw an exception with a custom message. Here's an example of that:

```python
class InvalidCredentialsError(Exception):
    def __init__(self, message="Invalid username or password"):
        self.message = message
        super().__init__(self.message)

def login(username, password):
    stored_username = "admin"
    stored_password = "password123"
    
    if username != stored_username or password != stored_password:
        raise InvalidCredentialsError()
    
    return f"Welcome, {username}!"
```

Here's a how you can use the `login` function with the `InvalidCredentialsError` exception:

```python
# failed login attempt
try:
    message = login("user", "wrongpassword")
except InvalidCredentialsError as e:
    print(f"Login failed: {e}")
else:
    print(message)

# successful login attempt
try:
    message = login("admin", "password123")
except InvalidCredentialsError as e:
    # This block is not executed because the login was successful
    print(f"Login failed: {e}")
else:
    # The else block runs if the 'try' block completes without an exception
    print(message)
```

The `raise` statement can also be used with the `from` keyword to chain exceptions, showing the relationship between different errors:

```python
def parse_config(filename):
  try:
      with open(filename, 'r') as file:
          data = file.read()
          return int(data)
  except FileNotFoundError:
      raise ValueError('Configuration file is missing') from None
  except ValueError as e:
      raise ValueError('Invalid configuration format') from e

config = parse_config('config.txt')
```

Python Classes and Objects
--------------------------

* **Class Definition**: A class is a blueprint for creating objects. It defines the behavior an object will have through its attributes and methods. Here is a basic example of a class definition in Python:

```python
class Dog:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def bark(self):
        print(f'{self.name.upper()} says woof woof!')
```

* **Creating Objects**: Objects are instances of a class. They are created by calling the class with the necessary arguments.

```python
dog1 = Dog('Jack', 3)
dog2 = Dog('Thatcher', 5)

dog1.bark()  # JACK says woof woof!
dog2.bark()  # THATCHER says woof woof!
```

* **Calling Methods on Objects**: You can call methods on objects to perform actions or retrieve information.

```python
object_name1.method_name()
object_name2.method_name()
```

* **Difference Between Class and Object**: A class is a reusable template, while an object is a specific instance of that class with actual data.

Attributes
----------

* **Instance Attributes**: Defined in `__init__()` using `self`, and unique to each object.
* **Class Attributes**: Defined directly inside the class and shared by all instances.

```python
class Dog:
    species = 'French Bulldog'  # Class attribute

    def __init__(self, name):
        self.name = name  # Instance attribute

print(Dog.species) # French Bulldog

jack = Dog('Jack')
print(jack.name)     # Jack
print(jack.species)  # French Bulldog
```

Methods
-------

* **Methods**: Functions defined inside a class that operate on the object's attributes.

```python
class Car:
    def __init__(self, color, model):
        self.color = color
        self.model = model

    def describe(self):
        return f'This car is a {self.color} {self.model}'

my_car_1 = Car('red', 'Tesla Model S')
print(my_car_1.describe())  # This car is a red Tesla Model S
```

* **Accessing Methods**: Call methods on objects using the dot notation. Here is an example of calling the `describe` method on two different car objects:

```python
class Car:
    def __init__(self, color, model):
        self.color = color  
        self.model = model  

    def describe(self):
        return f'This car is a {self.color} {self.model}'

my_car_1 = Car('red', 'Tesla Model S')
my_car_2 = Car('green', 'Lamborghini Revuelto')

print(my_car_1.describe()) # Calling method using the dot notation

print(my_car_2.describe()) # Calling method using the dot notation
```

Dunder (Magic) Methods
----------------------

* **Definition**: Special methods that start and end with a double underscore (e.g., `__init__`, `__len__`, `__str__`, `__eq__`). Python uses them internally for built-in operations.

```python
class Book:
    def __init__(self, title, pages):
        self.title = title
        self.pages = pages

    def __len__(self):
        return self.pages

    def __str__(self):
        return f"'{self.title}' has {self.pages} pages"

    def __eq__(self, other):
        return self.pages == other.pages

book1 = Book('Built Wealth Like a Boss', 420)
print(len(book1))        # 420
print(str(book1))        # 'Built Wealth Like a Boss' has 420 pages
```

* **Calling dunder methods indirectly**: You don't need to call dunder methods directly. Instead, Python automatically calls them when certain actions happen. These operations include:

  + **arithmetic operations like addition, subtraction, multiplication, division, and others**. `__add__()` is called for addition, `__sub__()` for subtraction, `__mul__()` for multiplication, and `__truediv__()` for division.
  + **string operations like concatenation, repetition, formatting, and conversion to text**. `__add__()` is called for concatenation, `__mul__()` for repetition, `__format__()` for formatting, `__str__()` and `__repr__()` for text conversion, and so on.
  + **comparison operations like equality, less-than, greater-than, and others**. `__eq__()` is called for equality checks, `__lt__()` for less-than, `__gt__()` for greater-than, and so on.
  + **iteration operations like making an object iterable and advancing through items**. `__iter__()` is called to return an iterator and  `__next__()` to fetch the next item.

Real World Example: Shopping Cart
---------------------------------

* **Cart Class with Dunder Methods**: Allows adding, removing, iterating, and checking contents with built-in behavior.

```python
class Cart:
    def __init__(self):
        self.items = []

    def add(self, item):
        self.items.append(item)

    def remove(self, item):
        if item in self.items:
            self.items.remove(item)
        else:
            print(f'{item} is not in cart')

    def list_items(self):
        return self.items

    def __len__(self):
        return len(self.items)

    def __getitem__(self, index):
        return self.items[index]

    def __contains__(self, item):
        return item in self.items

    def __iter__(self):
        return iter(self.items)

cart = Cart()
cart.add('Laptop')
print(len(cart))        # 1
print('Laptop' in cart) # True
```

What is Object-Oriented Programming?
------------------------------------

* **Object-oriented programming**: A programming style in which developers treat everything in their code like a real-world object. It is popularly called OOP. The four key principles that help you organize and manage code effectively are **encapsulation**, **inheritance**, **polymorphism**, and **abstraction**
* **Classes**: The blueprint for creating objects. Every single object created from a class has attributes that define data and methods that determine the behaviors of the object.

What is Encapsulation?
----------------------

* **Encapsulation**: The bundling of the attributes and methods of an object into a single unit. It lets you hide the internal state of the object behind a simple set of public methods and attributes that act like doors. Behind those doors are private attributes and methods that control how the data changes and who can see it.
* **Example of Encapsulation**: If you want to track a wallet balance, you will allow deposit and withdrawal, but you won't want anyone to tamper with the wallet balance itself:

```python
class Wallet:
   def __init__(self, balance):
       self.__balance = balance # Private attribute

   def deposit(self, amount):
       if amount > 0:
           self.__balance += amount # Add to the balance safely

   def withdraw(self, amount):
       if 0 < amount <= self.__balance:
           self.__balance -= amount # Remove from the balance safely

account = Wallet(500)
print(account.__balance) # AttributeError: 'Wallet' object has no attribute '__balance'
```

* **Difference Between Prefixing Attributes with Single and Double Underscore**: Prefixing attributes and methods with a single underscore means they are meant for internal use. This is a convention, and it doesn't enforce accessing attributes from the outside. Prefixing attributes and methods with a double underscore effectively prevents them from being accessed from outside of their class.

What Are Getters and Setters?
-----------------------------

* **Getters and Setters**: Methods that let you control how the attributes of a class are accessed and modified. You retrieve values with getters and you set values with setters.
* **Properties**: They connect getters and setters, and allow access to data. They run extra logic behind the scenes when you get, set, or delete values.
* **Why Properties Instead of Methods**: Properties are used instead of methods for better readability and cleaner code. They let you access values with dot notation, like regular attributes, without parentheses.
* **Creating a Getter**: To create a getter, you use the `@property` decorator. Here's a getter that gets the radius of a circle:

```python
class Circle:
    def __init__(self, radius):
        self.radius = radius # Calling the setter

    @property
    def radius(self): # A getter to get the radius
        return self._radius
  
    @property
    def area(self):  # A getter to calculate area
        return 3.14 * (self._radius ** 2)

my_circle = Circle(3)

print(my_circle.radius) # 3
print(my_circle.area) # 28.26
```

Using self.radius inside `__init__()` ensures the setter runs during object creation, so invalid radius values are caught immediately.

* **Creating a Setter**: To create the setter that will set the radius, you have to define another method with the same name and use `@<property_name>.setter` above it:

```python
class Circle:
    def __init__(self, radius):
        self.radius = radius # Calling the setter

    @property
    def radius(self):  # A getter to get the radius
        return self._radius

    @radius.setter
    def radius(self, value):  # A setter to set the radius
        if value <= 0:
            raise ValueError('Radius must be positive')
        self._radius = value

my_circle = Circle(3)
print('Initial radius:', my_circle.radius) # Initial radius: 3

my_circle.radius = 8
print('After modifying the radius:', my_circle.radius) # After modifying the radius: 8
```

* **How Python Handles Getters and Setters**: Once you define getters and setters, Python automatically calls them under the hood whenever you use normal attribute syntax this way:

```python
my_circle.radius # This will call the getter
my_circle.radius = 4 # This will call the setter
```

Inside the setter, you should not assign to the property name itself because that will cause a `RecursionError`.

* **Deleter**: After setting and getting a value with setter and getter, you can control how it is deleted with a `deleter`. A deleter runs custom logic when you use the `del` statement on a property. To create a deleter, you use the `@<property_name>.deleter` decorator.

```python
  # Deleter
    @radius.deleter
    def radius(self):
        print("Deleting radius...")
        del self._radius
```

What Is Inheritance and How Does It Promote Code Reuse?
-------------------------------------------------------

* **Inheritance**: The process by which a child class uses the attributes and methods of a parent class. Inheritance promotes code reuse, provides clear hierarchies, and customizes behavior without rewriting everything. To implement inheritance, a child class takes in the name of a parent class:

```python
class Parent:
    # Parent attributes and methods

class Child(Parent):
    # Child inherits, extends, and/or overrides where necessary
```

* **Single and Multiple Inheritance**: When a child class inherits properties and methods from a single parent, as you can see above, the process is called **single inheritance**. When a child class inherits properties and methods from more than one parent, that is **multiple inheritance**. Here's the syntax for that:

```python
class Parent:
    # Attributes and methods for Parent

class Child:
    # Attributes and methods for Child

class GrandChild(Parent, Child):
    # GrandChild inherits from both Parent and Child
    # GrandChild can combine or override behavior from each
```

* **`super()` Function**: A function that lets you **call** a method from a parent class, when a class has a different implementation of that method, or it extends the method, without duplicating code.

What Is Polymorphism and How Does It Promote Code Reuse?
--------------------------------------------------------

* **Polymorphism**: The OOP principle that lets different classes use the same method name, but each class implements it differently when called. Here's the syntax for it:

```python
class A:
   def action(self): ...

class B:
   def action(self): ...

class C:
   def action(self): ...

Class().method()  # Works for A, B, or C
```

* **Inheritance-based polymorphism**: A parent sets up a method, and each child class twists it to their use.

What is Name Mangling and How Does it Work?
-------------------------------------------

* **Name Mangling**: A process in which Python internally renames an attribute prefixed with a double underscore by adding an underscore and the class name as a prefix, turning `__attribute` into `_ClassName__attribute`.
* **The Purpose of Name Mangling**: The main purpose of name mangling is to prevent accidental attribute and method overriding when you use inheritance. Here's a code that makes that more understandable:

```python
class Parent:
    def __init__(self):
        self.__data = 'Parent data'

class Child(Parent):
    def __init__(self):
        super().__init__()
        self.__data = 'Child data'

c = Child()
print(c.__dict__) # {'_Parent__data': 'Parent data', '_Child__data': 'Child data'}
```

What Is Abstraction and How Does It Help Keep Complex Systems Organized?
------------------------------------------------------------------------

* **Abstraction**: A programming concept in which complex implementation details of object or system are hidden and only the essential features are shown. In Python and other programming languages, abstraction simplifies complex systems by increasing reusability.
* **Example of Abstraction**: A good example of abstraction in everyday life is a car letting you just use the wheel, pedals, and shifter without knowing how the engine or brakes work.
* **How Python Implements Abstraction**: Python implements abstraction through the `abc` module. The module provides the `ABC` class (abstract base class) and the `@abstractmethod` decorator. An abstract base class (ABC) defines the common methods and properties subclasses must implement. It can't be instantiated.
* **How Abstract Method is Defined**: An abstract method is defined with `@abstractmethod` and must be overridden in subclasses, even if it has a default implementation. The basic syntax of abstraction looks like this:

```python
from abc import ABC, abstractmethod

# Define an abstract base class
class AbstractClass(ABC):
    @abstractmethod
    def abstract_method(self):
        pass

# Concrete subclass that implements the abstract method
class ConcreteClassOne(AbstractClass):
    def abstract_method(self):
        print('Implementation in ConcreteClassOne')

# Another concrete subclass
class ConcreteClassTwo(AbstractClass):
    def abstract_method(self):
        print('Implementation in ConcreteClassTwo')
```

Algorithms and Big O Notation
-----------------------------

* **Algorithms**: A set of unambiguous instructions for solving a problem or carrying out a task. Algorithms must finish in a finite number of steps and each step must be precise and unambiguous.
* **Big O Notation**: Describes the worst-case performance, or growth rate, of an algorithm as the input size increases. It focuses on how resource usage grows with input size, ignoring constant factors and lower-order terms.

### Common Time Complexities

* **O(1) - Constant Time**: Algorithm takes the same amount of time regardless of input size.

```python
def check_even_or_odd(number):
    if number % 2 == 0:
        return 'Even'
    else:
        return 'Odd'
```

* **O(log n) - Logarithmic Time**: Time increases slowly as input grows. Common in algorithms that repeatedly reduce problem size by a fraction (like Binary Search).
* **O(n) - Linear Time**: Running time increases proportionally to input size.

```python
for grade in grades:
    print(grade)
```

* **O(n log n) - Log-Linear Time**: Common time complexity of efficient sorting algorithms like Merge Sort and Quick Sort.
* **O(n²) - Quadratic Time**: Running time increases quadratically. Often seen in nested loops.

```python
for i in range(n):
    for j in range(n):
        print("Hello, World!")
```

### Space Complexity

* **O(1) - Constant Space**: Algorithm uses same amount of memory regardless of input size.
* **O(n) - Linear Space**: Memory usage grows proportionally with input size.
* **O(n²) - Quadratic Space**: Memory usage grows quadratically with input size.

Problem-Solving Techniques
--------------------------

* **Understanding the Problem**: Read the problem statement multiple times. Identify the input, expected output, and how to transform input to output.
* **Pseudocode**: High-level description of algorithm logic that is language-independent. Uses common written language mixed with programming constructs like `IF`, `ELSE`, `FOR`, `WHILE`.

```python
GET original_string
SET reversed_string = ""
FOR EACH character IN original_string:
  ADD character TO THE BEGINNING OF reversed_string
DISPLAY reversed_string
```

* **Edge Cases**: Specific, valid inputs that occur at the boundaries of what an algorithm should handle. Always consider and test edge cases.

Arrays
------

* **Static Arrays**: Have a fixed size determined at initialization. Elements stored in adjacent memory locations. Size cannot be changed during program execution.
* **Dynamic Arrays**: Can grow or shrink automatically during program execution. Handle resizing through automatic copying to larger arrays when needed.

### Python Lists (Dynamic Arrays)

```python
numbers = [3, 4, 5, 6]

# Access elements
numbers[0]  # 3

# Update elements
numbers[2] = 16

# Add elements
numbers.append(7)
numbers.insert(3, 15)  # Insert at specific index

# Remove elements
numbers.pop(2)  # Remove at specific index
numbers.pop()   # Remove last element
```

### Time Complexities for Dynamic Arrays

* **Access**: O(1)
* **Insert at end**: O(1) average, O(n) when resizing needed
* **Insert in middle**: O(n)
* **Delete**: O(n) for middle, O(1) for end

Stacks
------

* **Stacks**: Last-In, First-Out (LIFO) data structure. Elements added and removed from the top only.
* **Push Operation**: Adding an element to the top of the stack. Time complexity: O(1).
* **Pop Operation**: Removing an element from the top of the stack. Time complexity: O(1).

```python
# Using Python list as stack
stack = []

# Push operations
stack.append(1)
stack.append(2)
stack.append(3)

# Pop operations
top_element = stack.pop()  # Returns 3
```

Queues
------

* **Queues**: First-In, First-Out (FIFO) data structure. Elements added to the back and removed from the front.
* **Enqueue Operation**: Adding an element to the back of the queue. Time complexity: O(1).
* **Dequeue Operation**: Removing an element from the front of the queue. Time complexity: O(1).

```python
from collections import deque

# Using deque for efficient queue operations
queue = deque()

# Enqueue operations
queue.append(1)
queue.append(2)
queue.append(3)

# Dequeue operations
first_element = queue.popleft()  # Returns 1
```

Linked Lists
------------

* **Linked Lists**: Linear data structure where each node contains data and a reference to the next node. Nodes are connected like a chain.

### Singly Linked Lists

* **Structure**: Each node has data and one reference to the next node.
* **Traversal**: Can only move forward from head to tail.
* **Head Node**: First node in the list, usually the only directly accessible node.
* **Tail Node**: Last node in the list, points to `None`.

### Operations and Time Complexities

* **Insert at beginning**: O(1)
* **Insert at end**: O(n) - must traverse to end
* **Insert in middle**: O(n) - must traverse to position
* **Delete from beginning**: O(1)
* **Delete from end**: O(n) - must traverse to find previous node
* **Delete from middle**: O(n) - must traverse to find node

### Doubly Linked Lists

* **Structure**: Each node has data and two references: next node and previous node.
* **Traversal**: Can move in both directions.
* **Memory**: Requires more memory than singly linked lists due to extra reference.

Hash Maps and Sets
------------------

### Maps and Hash Maps

* **Map (Abstract Data Type)**: Manages collections of key-value pairs. Every key must be unique, but values can be repeated.
* **Hash Map**: Concrete implementation of map ADT using hashing technique. Uses hash function to generate hash values for keys, which determine storage location in underlying array.

### Python Dictionaries (Hash Maps)

```python
# Creating dictionaries
my_dictionary = {
    "A": 1,
    "B": 2, 
    "C": 3
}

# Alternative creation
my_dictionary = dict(A=1, B=2, C=3)

# Access and modify
value = my_dictionary["A"]  # 1
my_dictionary["A"] = 4      # Update value
del my_dictionary["A"]      # Remove key-value pair

# Check membership
"C" in my_dictionary

# Get keys, values, items
my_dictionary.keys()
my_dictionary.values()
my_dictionary.items()
```

### Time Complexities for Hash Maps

* **Average case**: O(1) for insert, get, delete
* **Worst case**: O(n) when many hash collisions occur

### Sets

* **Sets**: Unordered collections of unique elements. No duplicates allowed, no specific order maintained.
* **Immutable Elements Only**: Sets can only contain immutable data types (numbers, strings, tuples) because hash values must remain constant.

```python
# Creating sets
numbers = {1, 2, 3, 4}
empty_set = set()  # Must use set(), not {}

# Add and remove elements
numbers.add(5)
numbers.remove(4)      # Raises KeyError if not found
numbers.discard(4)     # No error if not found

# Set operations
set_a = {1, 2, 3, 4}
set_b = {2, 3, 4, 5, 6}

# Union, intersection, difference, symmetric difference
set_a.union(set_b)                    # or set_a | set_b
set_a.intersection(set_b)             # or set_a & set_b
set_a.difference(set_b)               # or set_a - set_b
set_a.symmetric_difference(set_b)     # or set_a ^ set_b

# Subset and superset checks
set_a.issubset(set_b)
set_a.issuperset(set_b)
set_a.isdisjoint(set_b)

# Membership testing
5 in numbers
```

### Time Complexities for Sets

* **Average case**: O(1) for add, remove, membership testing
* **Worst case**: O(n) due to hash collisions

Hash Collisions
---------------

* **Hash Collision**: Occurs when two different keys produce the same hash value.
* **Collision Resolution Strategies**:

  + **Chaining**: Each array index points to a linked list storing all elements with same hash value
  + **Open Addressing**: Search for next available index using predefined sequence

When to Use Each Data Structure
-------------------------------

* **Lists**: When you need ordered, indexed access and don't know size in advance
* **Stacks**: For LIFO operations (undo functionality, expression evaluation, backtracking)
* **Queues**: For FIFO operations (task scheduling, breadth-first search)
* **Linked Lists**: When frequent insertion/deletion at beginning, unknown size, no random access needed
* **Hash Maps**: For fast key-value lookups, counting occurrences, caching
* **Sets**: For uniqueness checking, mathematical set operations, removing duplicates

Searching Algorithms
--------------------

Searching algorithms let you search for a target within a certain list of items.

In computer science, there are two searching algorithms you should know about. They are **linear search** and **binary search** algorithms. It is important to understand the differences between the two algorithms and when to use each one.

### Linear Search

* Linear search iterates through a list of items, checking each item from the beginning until the target item is found.
* If the target item is found, the index where it is located in the list is returned.
* If the target is not found, it returns `-1`, which means **invalid index** in most programming languages.
* Because linear search checks each item until it finds the target, it is not efficient for a large list of items.
* The time complexity of linear search is `O(n)` because the time it takes to search through the list grows linearly with the size of the list.
* The space complexity of linear search is `O(1)` because it doesn't require any additional space to search through the list.

### Binary Search

* Binary search works by dividing a list of items in half, and checking if the target value is in the middle of the list.
* The condition for binary search to work is that the items in the list must be in ascending order.
* Binary search is a more efficient algorithm for searching through a large list of items because it divides the list of items in half and ignores any half where the target is not found.
* If the target item is found in the middle of the list, the index of the target item is returned.
* If the item is not found, the algorithm checks if the target item is in the left or right half of the list.
* It continues to divide the remaining parts of the list into halves until the target item is found.
* If the target item is finally not found in the list, it returns `-1`
* The time complexity of binary search is `O(log n)` because the time it takes to search through the list grows logarithmically with the size of the list.
* The space complexity of binary search is `O(1)` because it doesn't require any additional space to search through the list.

### How Linear Search Differs from Binary Search

* Binary search is more suitable for a large list of items compared to linear search.
* The time complexity of linear search is `O(n)` because the time it takes to search through the list grows linearly with the size of the list.
* The time complexity of binary search is `O(log n)` because the time it takes to search through the list grows logarithmically with the size of the list.

Sorting Algorithms and Divide-and-Conquer
-----------------------------------------

In computer science, divide-and-conquer is a technique used to break down a problem into smaller sub-problems so they are easier to solve. Recursion is the technique often employed in divide-and-conquer, and divide-and-conquer is a powerful strategy used to implement many efficient sorting algorithms like merge sort.

### Merge Sort

* Merge sort is a sorting algorithm that follows the divide-and-conquer approach.
* It works by recursively dividing a list into smaller sub-lists until each sub-list contains only one element.
* It then repeatedly merges the sub-lists back together in a sorted order.
* The time complexity for merge sort is `O(n log n)` because the list is continuously divided in half `(log n)` and then merged together `(O(n))`.
* The space complexity of merge sort is `O(n)` because it is not an in-place sorting algorithm.

Graphs Overview
---------------

A graph is a set of nodes (vertices) connected by edges (connections). Each node can connect to multiple other nodes, forming a network. The different types of graphs include:

* Directed: edges have a direction (from one node to another), often represented with straight lines and arrows.
* Undirected: edges have no direction, represented with simple lines.
* Vertex: each node is associated with a label or identifier.
* Cyclic: contains cycles (a path that starts and ends at the same node).
* Acyclic (DAG): does not contain cycles.
* Edge labeled: each edge has a label usually drawn next to corresponding edge.
* Weighted: edges have weights (values) associated with them, that can be used to perform arithmetic operations.
* Disconnected: contains two or more nodes that are not connected by any edges.

Graphs are used in various applications such as maps, networks, recommendation systems, dependency resolution.

Graph Traversals
----------------

This involves visiting all the nodes in a graph. The two main algorithms are:

* **Breadth-First Search (BFS)**

  + Uses a queue.
  + Explores level by level.
  + Finds shortest path in unweighted graphs.
* **Depth-First Search (DFS)**

  + Uses a stack (or recursion).
  + Explores a branch fully before backtracking.
  + Useful for cycle detection and path finding.

Graph Representations
---------------------

Graphs can be represented in two main ways:

* **Adjacency List**

  + Each node has a list of its neighbors.
  + Space efficient for sparse graphs.
  + Easy to iterate over neighbors.
* **Adjacency Matrix**

  + A 2D array where rows and columns represent nodes.
  + Space intensive for large graphs.
  + Fast to check if an edge exists between two nodes.

Trees
-----

A tree is a special type of graph that is acyclic and connected. Key properties include:

* They have no loops or cycles (paths where the start and end nodes are the same).
* They must be connected (every node can be reached from every other node).

### Common types of trees

The most common types of trees are:

* Binary Trees

  + Each node has at most two children, a left and a right child.
* Binary Search Trees (BST)

  + A binary tree in which every left child is less than its parent, and every right child is greater than its parent.

Tries
-----

Also known as prefix trees, they are used to store sets of strings, where each node represents a character.

Shared prefixes are stored only once, making them efficient for tasks like autocomplete and spell checking.

Search and insertion operations have a time complexity of O(L), where L is the length of the string.

Priority Queues
---------------

A priority queue is an abstract data type where each element has a priority.

Queues and stacks consider only the order of insertion, while priority queues consider the priority of elements.

Standard queues follow FIFO (First In First Out) and stacks follow LIFO (Last In First Out). However, in a priority queue, elements with higher priority are served before those with lower priority, regardless of their insertion order.

Heaps
-----

It's a specialized tree-based data structure with a very specific property called the heap property.

The heap property determines the relationship between parent and child nodes. There are two types of heaps:

* Max-Heap

  + The value of each parent node is greater than or equal to the values of its children.
  + The largest element is at the root.
* Min-Heap

  + The value of each parent node is less than or equal to the values of its children.
  + The smallest element is at the root.

### Python `heapq` module example

```python
import heapq

# Create empty heap
my_heap = []

# Insert elements
heapq.heappush(my_heap, 9)
heapq.heappush(my_heap, 3)
heapq.heappush(my_heap, 5)
print(my_heap) # [3, 9, 5]

# Remove smallest element
print(heapq.heappop(my_heap))  # 3
print(my_heap) # [5, 9]

# Push + Pop in one step
print(heapq.heappushpop(my_heap, 7)) # 5
print(my_heap) # [7, 9]

# Transform list into heap
nums = [5, 7, 3, 1]
heapq.heapify(nums)
```

### Using Priorities

```python
my_heap = []
heapq.heappush(my_heap, (3, "A"))
heapq.heappush(my_heap, (2, "B"))
heapq.heappush(my_heap, (1, "C"))

# Removes lowest number = highest priority
print(heapq.heappop(my_heap))  # (1, "C")
```

Introduction to Dynamic Programming
-----------------------------------

* **Definition**: Dynamic programming is an algorithmic technique that solves complex problems by breaking them down into simpler subproblems and storing the results to avoid redundant calculations.
* **Overlapping Subproblems**: The same smaller problems appear multiple times when solving the larger problem. Instead of recalculating these subproblems repeatedly, we store their solutions.
* **Optimal Substructure**: The optimal solution to the problem contains optimal solutions to its subproblems. This means we can build up the best solution by combining the best solutions to smaller parts.

Dynamic Programming Solutions
-----------------------------

* **Memoization (Top-Down Approach)**: Memoization stores the results of expensive function calls and returns the cached result when the same inputs occur again.

```python
def climb_stairs_memo(n, memo={}):
    """Dynamic programming with memoization"""
    # Check if we've already calculated this value
    if n in memo:
        return memo[n]  # Return cached result - O(1) lookup!
    
    # Base cases
    if n <= 2:
        return n
    
    # Calculate once and store in memo for future use
    memo[n] = climb_stairs_memo(n-1, memo) + climb_stairs_memo(n-2, memo)
    return memo[n]
```

* **Tabulation (Bottom-Up Approach)**: Tabulation builds the solution from the ground up, filling a table with solutions to subproblems.

```python
def climb_stairs_tabulation(n):
    """Dynamic programming with tabulation"""
    if n <= 2:
        return n
    
    # Create array to store results for all steps from 0 to n
    dp = [0] * (n + 1)
    dp[1] = 1  # 1 way to reach step 1
    dp[2] = 2  # 2 ways to reach step 2
    
    # Build up the solution iteratively
    for i in range(3, n + 1):
        # Ways to reach step i = ways to reach (i-1) + ways to reach (i-2)
        dp[i] = dp[i-1] + dp[i-2]
    
    return dp[n]
```

Real-World Applications Using Dynamic Programming
-------------------------------------------------

* **Route Optimization**: GPS systems use dynamic programming algorithms to find shortest paths between locations.
* **Text Processing**: Spell checkers and autocomplete features often rely on dynamic programming to calculate edit distances between words.
* **Financial Modeling**: Investment strategies and portfolio optimization frequently employ dynamic programming techniques.
* **Resource Allocation**: The knapsack problem and its variants appear in scheduling, budgeting, and resource management.

When to Use Dynamic Programming
-------------------------------

You should consider using dynamic programming in the following scenarios:

* The problem can be broken down into overlapping subproblems.
* The problem exhibits optimal substructure.
* A naive recursive solution would involve repeated calculations.
* You need to optimize for time complexity at the cost of space complexity.

---

