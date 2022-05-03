# Become a Python developer

![](https://www.snpinfotech.com/assets/images/developments/python_banner.jpg)

Python is a powerful general-purpose programming language used in GIS, data science, web development, machine learning, game development and so on. Python is simple, easy-to-use, versatile language. That is why it gain huge popularity among community and biggest organizations such as Google, NASA and Spotify use Python to power-up their services.

I created this as short note to explain the things I had explored in the world of Python as much as simple I can. To kick start, you may required

* A computer with Python 3.x installed
* A text editor or IDE (Sublime , VSCode or whatever you preferred)
* Patience and Time

## Table of content

- [Basic Syntax](#basic-syntax)
   - [Interpret your code](#interpret-your-code)
   - [Comments](#comments)
   - [Identifiers](#identifiers)
   - [Naming Conventions](#naming-conventions)
   - Multiple Statements in Single Line
   - Single statement in Multi-lines
   - Indentation
   - 
- Variables and Data Types
- Conditionals
- Type Casting
- Lists, Tuples, Sets, Dictionaries
- Exceptions
- Functions

## Basic Syntax

Each line in a Python script is a statement. A statement is an instruction that Python interpreter can execute. Each Python statement ends with a NEWLINE character. 



### Interpret your code

Python code can be write and executed in many ways.

1. By using Command Line

   In Windows, open CMD. In Linux/Mac open terminal.
   
   > python
   >
   > \>>> print("Hello, World!")
   >
   > Hello, World
---
2. By using Python IDLE

   > \>>> print("Hello, World!")
   >
   > Hello, World
---
3. By using a text editor or a IDE

   > print("Hello, World!")

   Write above code in a new file and save as **.py** file and execute.
   
   Note: py is the extension of python script files.

Either way, you can run this simple program. 



### Comments

Comments can be used to explain code you write. It help you and other people who use your code to read the code more easily. Also, comments can be used to prevent execution when testing code. There are multiple ways of writing comments.

- Single line comment

  Use to make single line of comment. Generally use hash tag (`#`) to indicate single line comment.
  
  ```python
  name = input("Enter your name") # Take user's name as a input
  print(name)  # Display the name taken above
  # End the program
  ```
  
  
  
- Multi line comment

  Use to make multi-lines of comment. Use six single quotes as two groups of three and three (`''' '''`) to indicate multi-line comment.

  ```python
  '''This code will,
      * Display 'Hi'
      * Take user's name as a input 
      * Display the name enterd by user and terminate'''
  
  print("Hi")
  name = input("Enter your name")
  print(name)
  ```



### Identifiers

Identifiers are names that used to identify variables, functions, modules, classes, and other objects in Python. The name of an identifier needs to starts with a letter or underscore (`_`). The following characters can be alphanumeric or underscore. Letters can be uppercase or lowercase.

| NAME | _nAme | n___ |
|----|----|----|
| **__**   | **n4**    | **_4**   |
| **n4__** | **N4me**  | **n_4** |




Identifiers should not contains any other symbols like `@`, `$`, `#`, and so on. Also, we can not start a identifier by a number. In the below table, we can find invalid identifiers.

| 4name | &name | name! |
| ----- | ---- | ---- |



In a computer languages there are some words known as keywords or reserved word.  Keywords are words that cannot be used as an identifier. Here is some of them.

| and      | exec    | not    |
| -------- | ------- | ------ |
| assert   | finally | or     |
| break    | for     | pass   |
| class    | from    |  return |
| continue | global  | raise  |
| def      | if      | lambda |
| del      | import  | try    |
| elif     | in      | while  |
| else     | is      | with   |




You can use following code to find the current keywords.

```python
import keyword

print(keyword.kwlist) 
```



Python identifiers are case-sensitive. For example, the `name`, `NAME` and `Name` are three different identifiers!



Note: **Keep in mind. Your identifiers should be meaningful and short.**



### Naming Conventions

- [ ] Class names start with an uppercase letter. All other identifiers start with a lowercase letter.

- [ ] Starting an identifier with a single leading underscore indicates that the identifier is private.

- [ ] Starting an identifier with two leading underscores indicates a strongly private identifier.

- [ ] Identifier ends with two trailing underscores is a language-defined special name.
