# https-github.com-Powerlearnproject-se-assignment-6-introduction-to-python-Thandeshnie

Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.

Python is a dynamic, high-level, free open source, and interpreted programming language. It supports object-oriented programming as well as procedural-oriented programming. In Python, we don’t need to declare the type of variable because it is a dynamically typed language.

The key features that makes python to be popular are as follows 
(1) It is easy to learn and read , it has staight forward syntax that makes it easy for beginners to grasp. the code is readable .
(2) Python supports object oriented  programming which include concepts like classes and object encapusation. 
(3) Python has vast community on platform like stackoverflow , providing answers common questions and helping developers troubleshoot issues.
(4) It has GUI programming support modules such as PyQt5 , wxPython and Tk allow developers to create  grafical  user interface GUI for applications 

Python is particularly effective in 
-Web Developmen,  Python is widely used for building web applications, thanks to frameworks like Django and Flask.
-Data Science and Machine Learning ,Python dominates data science and ML due to libraries like NumPy, pandas, and scikit-learn.
-Automation and Scripting , Python’s simplicity makes it ideal for automating repetitive tasks and writing scripts.
-Game Development ,Pygame and other libraries enable game development.


2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.

-Visit the official Python website and navigate to the download page.
-Choose the appropriate version of Python based on your Windows operating system (64-bit or 32-bit) in my case I used 64-bit versin 3.12.4  which is compitable with my windows 11 
-Click the Download button to get the installer.
-Run the downloaded .exe file.
-During installation, make sure to check the box that says “Add Python to PATH.” This ensures that you can run Python from the command prompt.
-Follow the prompts to complete the installation

Verify Python Installation
-Open a new Command Prompt or PowerShell window.
-Type python --version and press Enter.
-If Python is installed correctly, it will display the installed version (e.g., Python 3.12.4).
![alt text](<Screenshot 2024-06-30 023519python.png>)
Set Up a Virtual Environment
-Decide on a directory where you want to create your virtual environment (e.g., your project folder).
-Open the Command Prompt or PowerShell in that directory.
-Run the following command to create a virtual environment named “env”:
(python -m venv env)
-This will create a new folder called “env” containing the isolated Python environment.
-To activate the virtual environment(env\Scripts\activate)


3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.


![alt text](<Screenshot 2024-06-30 024014q3 helloworld.png>)

print() Function
-The print() function is used to display text or other values in the console.
-Inside the parentheses, we provide the string we want to display (in this case, "Hello, World!").
-The string must be enclosed in either single quotes (') or double quotes (").


4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.

(1)Integer (int)
-Represents whole numbers (positive, negative, or zero).
-Example: age = 25
(2)Floating-Point Number (float)
-Represents decimal numbers.
-Example: pi = 3.14
(3) String (str)
-Represents text.
-Enclosed in single (') or double (") quotes.
-Example: name = "Alice"
(4) Boolean (bool)
-Represents either True or False.
-Used for logical operations.
-Example: is_student = True
(5)List (list)
-Ordered collection of items.
-Enclosed in square brackets ([]).
-Example: fruits = ["apple", "banana", "cherry"]
(6)Tuple (tuple)
-Similar to a list but immutable (cannot be modified after creation).
-Enclosed in parentheses (()).
-Example: coordinates = (10, 20)
(7)Dictionary (dict):
-Key-value pairs.
-Enclosed in curly braces ({}).
-Example: person = {"name": "Bob", "age": 30}

![alt text](<Screenshot 2024-06-30 py.png>)


5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.

-Conditional statements allow you to execute different code blocks based on certain conditions.
The most common conditional statement is the if-else statement.

age = 16
if age >= 16:
    print("You are an adult.")
else:
    print("You are not yet an adult.")


-Loops allow you to repeat a block of code multiple times.
Two common types of loops in Python are for loops and while loops.

# Using a for loop to print numbers from 1 to 5
for i in range(1, 6):
    print(i)

# Using a while loop to calculate the sum of numbers from 1 to 10
total = 0
num = 1
while num <= 10:
    total += num
    num += 1
print("Sum of numbers:", total)

-The range(1, 6) generates numbers from 1 to 5 (inclusive).
-It prints each number in the loop.
-In the second loop
-The while loop continues as long as num is less than or equal to 10.

6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.

Python are reusable blocks of code that perform specific tasks. They allow you to organize your code, improve readability, and avoid redundancy


-Modularity functions break down complex tasks into smaller, manageable parts. You can reuse these parts across different parts of your program.
-Abstraction functions hide implementation details. You can use a function without knowing how it works internally.
-Readability well-named functions make your code more readable. They act as building blocks that describe their purpose.

def add_numbers(a, b):
    """Returns the sum of two numbers."""
    return a + b
![alt text](<Screenshot 2024-06-30 030622dsddds.png>)

# Example usage:
result = add_numbers(10, 7)
print("Sum:", result)  # Output: Sum: 17

7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.

-Lists are ordered collections of items.
-Items in a list can be of any data type (e.g., numbers, strings, other lists).
-Lists are defined using square brackets ([]).

# Creating a list of numbers
numbers_list = [1, 2, 3, 4, 5]

# Accessing elements
print("First element:", numbers_list[0])  # Output: 1

# Modifying an element
numbers_list[2] = 10
print("Modified list:", numbers_list)  # Output: [1, 2, 10, 4, 5]

# Adding an element
numbers_list.append(6)
print("Updated list:", numbers_list)  # Output: [1, 2, 10, 4, 5, 6]


-Dictionaries are unordered collections of key-value pairs.
-Each value is associated with a unique key.
-Dictionaries are defined using curly braces ({}).

# Creating a dictionary
student_info = {
    "name": "Thando",
    "age": 26,
    "major": "Computer Science"
}

# Accessing values
print("Name:", student_info["name"])  # Output: Thando

# Modifying a value
student_info["age"] = 26
print("Updated info:", student_info)  # Output: {'name': 'Thando', 'age': 26, 'major': 'Computer Science'}

# Adding a new key-value pair
student_info["gpa"] = 3.8
print("Updated info:", student_info)  # Output: {'name': 'Alice', 'age': 21, 'major': 'Computer Science', 'gpa': 3.8}


8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.

`except`

def divide(a, b):
    try:
        result = a / b
    except ZeroDivisionError:
        print("Error: Cannot divide by zero.")
    else:
        print(f"Result: {result}")
    finally:
        print("Execution completed.")

# Example usage
divide(10, 2)  # Output: Result: 5.0 \n Execution completed.
divide(10, 0)  # Output: Error: Cannot divide by zero. \n Execution completed.

9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.



# Import the entire module
import math

# Import specific functions/classes from a module
from math import sqrt, pi
import math

# Calculate square root
x = 16
sqrt_x = math.sqrt(x)
print(f"Square root of {x} is {sqrt_x:.2f}")

# Calculate area of a circle
radius = 5
area = math.pi * radius**2
print(f"Area of the circle with radius {radius} is {area:.2f}")


Square root of 16 is 4.00
Area of the circle with radius 5 is 78.54

![alt text](image.png)

10. File I/O:  - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.


# Read from a file
try:
    with open("sample.txt", "r") as file:
        content = file.read()
        print("File content:")
        print(content)
except FileNotFoundError:
    print("File not found.")

# Write to a file
data_to_write = ["Hello", "World", "Python", "Files"]
try:
    with open("output.txt", "w") as file:
        for item in data_to_write:
            file.write(item + "\n")  # Add a newline after each item
    print("Data written to output.txt.")
except IOError:
    print("Error writing to file.")


    Referencies 

    https://www.geeksforgeeks.org/python-features/
    https://pythonsden.com/top-15-python-use-cases/
    https://stackoverflow.com/questions/56715476/how-do-i-test-if-python-is-installed-on-windows-10-and-run-an-exe-to-install

# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].
