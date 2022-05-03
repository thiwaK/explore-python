# Become a Python developer

Python is a powerful general-purpose programming language used in GIS, data science, web development, machine learning, game development and so on. Python is simple, easy-to-use, versatile language. That is why it gain huge popularity among community and biggest organizations such as Google, NASA and Spotify use Python to power-up their services.

I created this as short note to explain the things I had explored in the world of Python as much as simple I can. To kick start, you may required

* A computer with Python 3.x installed
* A text editor or IDE (Sublime , VSCode or whatever you preferred)
* Patience and Time

## Table of content

- [ ] [Basic Syntax](#basic-syntax)
   - [Interpret your code](#interpret-your-code)
   - [Comments](#comments)
   - Identifiers
   - Multiple Statements in Single Line
   - Indentation
   - Naming Conventions
   - 
   
- Variables and Data Types
- Conditionals
- Type Casting
- Lists, Tuples, Sets, Dictionaries
- Exceptions
- Functions

### Basic Syntax

#### Interpret your code

Python codes can be write and executed in many ways.

1. By using Command Line

   In Windows, open CMD. In Linux/Mac open terminal.
   > python
   > \>>> print("Hello, World!")
   > Hello, World
   
2. By using Python IDLE

   > \>>> print("Hello, World!")
   >
   > Hello, World

3. By using text editor

   > print("Hello, World!")

   Write above code in a new file and save as **.py** file and execute.
   
   Note: py is the extension of python script files.

Either way, you can run this simple program. 



#### Comments

Comments can be used to explain code you write. It help you and other people who use your code to read the code more easily. Also, comments can be used to prevent execution when testing code. There are multiple ways of writing comments.

- Single line comment

  Use to make single line of comment. Generally use hash tag (#) to indicate single line comment.
  
  ```python
  name = input("Enter your name") # Take user's name as a input
  print(name)  # Display the name taken above
  # End the program
  ```
  
  
  
- Multi line comment

  Use to make multi-lines of comment.

  ```python
  '''This code will,
  	* Display 'Hi'
      * Take user's name as a input 
      * Display the name enterd by user and terminate'''
  
  print("Hi")
  name = input("Enter your name")
  print(name)
  ```
