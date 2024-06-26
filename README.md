[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15332366&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.

   Python is a high-level, interpreted programming language

   features:
   Simple Syntax :syntax is straightforward and resembles natural language.
   Cross-Platform:Python is platform-independent
   It is simple and Easy to Learn
   Scalability:suitable for projects of varying scales

   use case scenarios
   Machine Learning and Artificial Intelligence
   server side scripting
   Data Analysis and Visualization
   Web Development
   Scientific Computing.

2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.

   > Go to the Python official website and download the latest version of Python for Windows.
   > Once the download is complete, run the installer executable (.exe file) that you downloaded.
   > Follow the prompts in the Python installer. choose the default options unless you have specific preferences.Click "Install Now" to begin the installation.
   To verify:
   > Open Command Prompt and type python --version to verify that Python is installed correctly.

3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.

   print("hello world")
   The print() function in Python is used to output text to the console
   strings are enclosed in either single quotes ('') or double quotes (" ")

4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.
   Integer (int):
   Represents whole numbers without decimal points.
    ie X=19
   Float (float):
   Represents numbers with decimal points ..
   ie X=2.23

   String (str):
   Represents a sequence of characters enclosed in single quotes ('') or double quotes ("").
   name="plp project"

   Boolean (bool):
   Represents truth values True or False.
   is_plp_fun = True
   
   List (list):
   age= [11, 22, 13, 14, 25]
   Represents an ordered collection of items enclosed in square brackets ([]).


5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.

   Conditional statements in Python are used to execute certain code blocks based on whether a condition is true or false.
   i.e 
   x = 20
   if x > 10:
    print("x is greater than 10")
   else:
    print("x is not greater than 10")

   Loops in Python allow you to iterate over a sequence of data, performing repetitive tasks until a certain condition is met there ae different types of loops ie for loop and while loop do while loop.
   ie 
      numbers = [1, 2, 3, 4, 5]

     for num in numbers:
        print(num)

6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.

   Functions in Python are  blocks of code that perform a specific task.
   Modularity: Functions promote code reuse by encapsulating logic into independent units. This reduces redundancy and makes code easier to maintain and update.

   Abstraction: Functions hide complex implementation details, allowing you to focus on what the function does rather than how it does it. This improves code readability and comprehension.

   Organization: Using functions organizes code into logical blocks, making it easier to navigate and understand the structure of a program.

   Ease of Testing: Functions facilitate unit testing because you can test each function independently to ensure it behaves correctly under different conditions.

   def calculate_sum(a, b):
    
    return a + b

  result = calculate_sum(3, 6)

  print("Sum:", result)



7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.

   Lists:

   Lists are used to store collections of items in a specific order.
   Access: Elements in a list are accessed by their position.
   Example: [1, 2, 3, 4, 5]

   Dictionaries:

   Dictionaries are used to store key-value pairs where each value is accessed by its key.
   Access: Elements in a dictionary are accessed by their keys.
   Example: {'name': 'Kare', 'age': 22, 'city': 'Nairobi'}

8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.

   Exception handling in Python allows you to gracefully manage and respond to errors that occur during program execution. It involves using try, except, and optionally finally blocks to catch and handle exceptions (errors).
   Try Block:
   The try block is used to enclose the code that may raise an exception.
   Except Block:
   The except block is used to handle specific exceptions that are raised within the try block.
   Finally Block (optional):
   The finally block is used to execute cleanup code that should always run, whether an exception occurred or not.

   try:
    x = 10 / 0  # Trying to divide by zero
    print("Division result:", x)  
except ZeroDivisionError:
    print("Error: Division by zero!") 
finally:
    print("Finally block executed.")  
 

9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.

   Modules in Python are like containers that hold Python code
   To import and use a module in Python, you use the 'import' statement followed by the module or package name ie import math
   This brings the entire 'math' module into your script, allowing you to use its functions and constants.

   Packages in Python are folders that contain multiple Python modules. 

10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.

    To read from a file in Python:

    Open the File: Use the open() function with the file path and mode ('r' for reading).
    Read the Content: Use methods like read(), readline(), or readlines() to read the file content.
    Close the File: Always close the file using the close().

   file_path = 'sample.txt'  # Replace with the actual file path
   try:
    
    with open(file_path, 'r') as file:
       
        file_content = file.read()
        print("File Content:")
        print(file_content)
   except FileNotFoundError:
    print(f"Error: The file '{file_path}' does not exist.")
   except IOError:
    print(f"Error: Unable to read the file '{file_path}'.")


    To write file :
    You can use the open() function with 'w' (write) mode. If the file does not exist, it will be created. If it exists, its previous content will be overwritten.

    
lines_to_write = [
    "Hello,",
    "This is an example file.",
    "Demonstrating writing lines to a file in Python."
]

output_file = 'output.txt'  # Replace with the actual file path

try:
    with open(output_file, 'w') as file:
        
        for line in lines_to_write:
            file.write(line + '\n')
    print(f"Successfully wrote lines to '{output_file}'.")
except IOError:
    print(f"Error: Failed to write to the file '{output_file}'.")


# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


Reference from AI Chatbot 