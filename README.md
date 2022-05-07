# Want to be a Python developer

![](https://www.snpinfotech.com/assets/images/developments/python_banner.jpg)

Python is a powerful general-purpose programming language used in GIScience, data science, web development, machine learning, game development and so on. Python is simple, easy-to-use, versatile language. That is why it gains huge popularity in the community and the biggest organizations such as Google, NASA and Spotify use Python to power-up their services.

I created this as a short note to explain the things I had explored in the world of Python as much as simple I can. To kick start, you may required

* A computer with Python 3.x installed

* A text editor or IDE (Sublime, VSCode or whatever you preferred)

* Patience and Time

  

## Table of content

- [Basic Syntax](#basic-syntax)
   - [Interpret your code](#interpret-your-code)
   - [Comments](#comments)
   - [Identifiers](#identifiers)
   - [Naming Conventions](#naming-conventions)
   - [Multiple Statements in a Single Line](#multiple-statements-in-a-single-line)
   - [Single statement in Multiple Lines](#single-statement-in-multiple-lines)
   - [Indentation](#Indentation)
   
- [Variables and Data Types](#variables-and-data-types)
   - [Variables](#variables)
   
     - Multiple methods to assign
   
     - Global and Local variables
     - Delete declared variable
   
   - [Data types](#data-types)
   
- Conditionals

- Type Casting

- Lists, Tuples, Sets, Dictionaries

- Exceptions

- Functions

- [Resources](#resources)
   - [Cheat Sheets](#cheat-sheets)



## Basic Syntax
Each line in a Python script is a statement. A statement is an instruction or may be a set of instructions that Python interpreter can execute. Each Python statement ends with a NEWLINE character. 


### Interpret your code

Python code can be write and executed in many ways.

1. By using Command Line

   In Windows, open CMD. In Linux/Mac, open terminal.
   
   ```shell
   python
   >>> print("Hello, World!")
   Hello, World

2. By using Python IDLE

   ```IDL
   >>> print("Hello, World!")
   Hello, World

3. By using a text editor or a IDE
   
   ```python
   print("Hello, World!")
   ```
   
   Write above code in a new file and save as **.py** file and execute.
   
   Note: py is the extension of python script files.

Either way, you can run (interpret) your program. 



### Comments

Comments can be used to explain code you write. It help you and other people who use your code to read the code more easily. Also, comments can be used to prevent execution when testing code. There are multiple ways of writing comments.

- Single line comment

  Generally use hash tag (`#`) to indicate single line comment.
  
  ```python
  name = input("Enter your name") # Take user's name as a input
  print(name)  # Display the name taken above
  # End the program
  ```
  
  
  
- Multi line comment

  Use six single quotes as two groups  (`''' '''`) to indicate a multi-line comment.

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

---

### Naming Conventions

- [ ] Class names should use the Title Case convention. All other identifiers start with a lowercase letter.

  `Class Persion`    `Class NetworkManager` 

- [ ] If it is a function name and contains multiple words, should use underscores to separate the words.

- [ ] Constant variable names should be in uppercase.

  `PI=3.141`    `RATE=3.4` 

- [ ] Starting an identifier with a single leading underscore indicates that the identifier is private.

- [ ] Starting an identifier with two leading underscores indicates a strongly private identifier.

- [ ] Use of one or two underscore characters when naming the instance attributes of a class.

- [ ] Identifier ends with two trailing underscores is a language-defined special name.

- [ ] Two leading and trailing underscores are used in Python itself for a special purpose.

  `__init__`    `__main__`    `__add__`



### Multiple Statements in a Single Line

The semicolon (` ; `) allows Python to execute multiple statements written in a single line of code.

```python
import datetime; now = datetime.datetime.now(); current_time = now.strftime("%H:%M:%S"); print("Current Time =", current_time)
```



### Single statement in Multiple lines

Python uses a newline character (`\n`) to separate statements. It places each statement on one line. However, a long statement can span multiple lines by using the backslash (`\`) character.

```python
a,b,c = True, False, True

if (a == True) \
and (b == False) and \
(c == True):
    print("Continuation of statements")
```



Statements contained within the `[]`, `{}`, or `()` brackets do not need to use the line continuation character.

```python
days = ['Monday', 'Tuesday', 'Wednesday',
        'Thursday', 'Friday']
```



### Indentation

Leading space or tab at the beginning of the line is considered as indentation level of the line. It is used to determine a group of statements which is belongs to a block of code. The number of spaces in the indentation is variable, but all statements within the block must be indented the same amount.

```python
a = 5

if a == 5:
    # This block of code execute when a is equals to 5
    print("a is 5")
else:
    # If it is not, this block of code will execute
    print("a is not 5")
```



There are several rules.

- [ ] Use the colon `:` to start a block.

- [ ] All the lines in a block must use the same indentation, either space or a tab.

- [ ] A block can have inner blocks with next level indentation.

  ```python
  a = 5
  
  if a > 0:
      # This block of code execute when a is greater than 0
      print("a is a positive integer")
      
      if a%2 == 0:
          # This block of code execute whe a can be devide by 2
          print("a is a mulatiple of 2")
  else:
      # If it is not, this block of code will execute
      print("a is not a positive integer")
  ```

- [ ] Do not mix space and tab in the same script.



## Variables and Data types



### Variables

A variable is a labeled location used to store data in the main memory. So variables is a container with a unique name that can holds data in it. To define a variable, you use the following syntax.

```python
variable_name = value
```

Here, `=` symbol is the assignment operator. It assign right hand side value to the left hand side variable. Variable can hold any value or values belongs to a data type.

```python
my_age = 22            # This variable contains an integer
my_name = "Thiwanka"   # This variable contains a string (text)
my_weight_in_kg = 60.5 # This variable contains a deciaml
```

In Python, data holds in a variable can be changed later (redeclare) with in the program. 

```python
temp_var = True
temp_var = "Python"
temp_var = 5
```



#### Multiple methods to assign

```python
a = 1; b = 2; c = 3 # set a to 1, b to 2, and c to 3
a = b = c = 1       # set a, b and c to 1
a, b, c = 1, 2, 3   # set a to 1, b to 2, and c to 3
```



#### Global and Local variables

All the variables declared in python may not be accessible at all locations. It will depend on where these variables  were declared. **Scope of the variable** defines where in the program the  variable will be accessible. The scope can be either Local or Global.

A variable that is declared inside a python function or a module can only be used in that specific function or Python Module is known as a local variable.

```python
def engine_attributes(speed):
    '''This is a Python function named engine_attributes.
    It keeps engine_speed as a local variable'''
    
    engine_speed = speed
    
engine_attributes(150) # call the function by passing 150 as an argument
print(engine_speed) # display engine speed. Syntax error.
```



Above code will be throw a syntax error. because engine_speed declarer inside the engine_attributes function. Which means it can not be access outside of the function. If we want to access that variable outside of the function, we should declare it as a global variable.


```python
def engine_attributes(speed):
    '''This is a Python function named engine_attributes.
    it keeps engine_speed as a local variable'''
    
    global engine_speed # re-declared the variable engine_speed in the function as a global variable
    engine_speed = speed
    
engine_attributes(150) # call the function by passing 150 as an argument
print(engine_speed) # display engine speed
```



#### Delete declared variable

Delete a variable when it is not in use so as to free up space.

```python
abc = 10
del abc # delete variable abc
```





### Data types

Data types are the categorization of data items. Python supports several built-in data types.

- [ ] Scaler Types
  - Integer `int` - Positive or negative whole numbers.
    - Integer -  `10` 
    - Hexadecimal -  `0xfff`
    - Octal - `0o777`
    - Binary - `0b1000001`
  - Floating-point `float` - Any real number with a floating-point representation. Ex: `0.001` `1.0e-3`
  - Boolean `bool` - Values should be `True` `False` or `1` `0`.
  - Null `None` - Represents the null object in Python. Ex: `name = None`
- [ ] Sequence Types
  - Text `string` - Collection of one or more characters put in single, double or triple quotes. Ex: `'thiwaK'` `"thiwaK"` `"""thiwaK"""`
  - List `list` - An ordered collection of one or more data items, not necessarily of the same type. Ex: `names = ['Snow', 'Shelby']` `temp_data = ['fabbc5f=', 55, False, 0.1]`
  - Tuple `tuple` - An ordered collection of one or more data items, not necessarily of the same type. Ex: `names = ('Snow', 'Shelby')` `temp_data = ('fabbc5f=', 55, False, 0.1)`
- [ ] Mapping Types
  - Dictionary `dict` - an unordered collection of data in a `key`:`value` pair form. Ex: `player_score = {'Snow':20, 'Shelby': 50}`



| Class   | Name           | Mutable | Supports                 |
| ------- | -------------- | ------- | ------------------------ |
| int     | Integer        | No      | int (int, hex, bin, oct) |
| float   | Floating point | No      | float                    |
| string  | Text           | No      | string                   |
| bool    | Boolean        | No      | bool                     |
| list    | List           | Yes     | any                      |
| tuple   | Tuple          | Yes     | any                      |
| dict    | Dictionary     | Yes     | any                      |
| complex | Complex        | No      | complex                  |



## Resources

### Cheat Sheets

- [intellipaat.com](#https://intellipaat.com/mediaFiles/2018/11/Python-Basics-Cheat-Sheet-1-1.png)

- [cusy.io](#https://cusy.io/en/assets/images/python-cheat-sheet-2.jpg)

- [cusy.io](#https://cusy.io/en/assets/images/python-cheat-sheet.jpg)
