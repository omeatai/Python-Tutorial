# Python-Tutorial

Python Tutorial by Ifeanyi Omeata

## Tutorial

---

### [1-PYTHON COURSE - W3SCHOOLS](#)

+INTRODUCTION

<details>
  <summary>1. Python Introduction</summary>

Python is a popular programming language. It was created by Guido van Rossum, and released in 1991.

It is used for:

- web development (server-side),
- software development,
- mathematics,
- system scripting.

What can Python do?

- Python can be used on a server to create web applications.
- Python can be used alongside software to create workflows.
- Python can connect to database systems. It can also read and modify files.
- Python can be used to handle big data and perform complex mathematics.
- Python can be used for rapid prototyping, or for production-ready software development.

```py
print("Hello, World!")
```

```py
# Hello, World!
```

```py
x = "Python is awesome"
print(x)
```

```py
# Python is awesome
```

```py
x = "Python"
y = "is"
z = "awesome"
print(x, y, z)
```

```py
# Python is awesome
```

```py
x = "Python "
y = "is "
z = "awesome"
print(x + y + z)
```

In the print() function, when you try to combine a string and a number with the + operator, Python will give you an error.

```py
# Python is awesome
```

check Python version:

```bs
python --version
python -V
```

Run Python File:

```bs
python index.py
```

Run Python Shell:

```bs
python
```

```bs
Python 3.9.12 (main, Apr  5 2022, 01:53:17)
[Clang 12.0.0 ] :: Anaconda, Inc. on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>> print("Hello")
Hello
>>> exit()
%
```

</details>

<details>
  <summary>2. Python Comments </summary>

- Python has commenting capability for the purpose of in-code documentation.

- Comments start with a #, and Python will render the rest of the line as a comment.

- Comments can be used to explain Python code.

- Comments can be used to make the code more readable.

- Comments can be used to prevent execution when testing code.

- Comments can be placed at the end of a line, and Python will ignore the rest of the line.

- A comment does not have to be text that explains the code, it can also be used to prevent Python from executing code.

- Python does not really have a syntax for multiline comments.

- To add a multiline comment you could insert a # for each line.

- Since Python will ignore string literals that are not assigned to a variable, you can add a multiline string (triple quotes) in your code, and place your comment inside it.

```py
#This is a comment.
print("Hello, World!")
```

```py
print("Hello, World!") #This is a comment
```

```py
#print("Hello, World!")
print("Cheers, Mate!")
```

```py
#This is a comment
#written in
#more than just one line
print("Hello, World!")
```

```py
"""
This is a comment
written in
more than just one line
"""
print("Hello, World!")
```

</details>

<details>
  <summary>3. Python Variables </summary>

- Python has no command for declaring a variable.

- A variable is created the moment you first assign a value to it.

- Variable names are case-sensitive.

- A variable can have a short name (like x and y) or a more descriptive name (age, carname, total\*volume).

Rules for Python variables:

- A variable name must start with a letter or the underscore character
- A variable name cannot start with a number
- A variable name can only contain alpha-numeric characters and underscores (A-z, 0-9, and \* )
- Variable names are case-sensitive (age, Age and AGE are three different variables)

Legal variable names:

```py
myvar = "John"
my_var = "John"
_my_var = "John"
myVar = "John"
MYVAR = "John"
myvar2 = "John"
```

- Camel Case = myVariableName
- Pascal Case = MyVariableName
- Snake Case = my_variable_name

```py
x = 5
y = "John"
print(x)
print(y)
```

```py
# 5
# John
```

```py
x = 4       # x is of type int
x = "Sally" # x is now of type str
print(x)
```

```py
# Sally
```

```py
a = 4
A = "Sally"
#A will not overwrite a
```

Many Values to Multiple Variables-

- Python allows you to assign values to multiple variables in one line:

```py
x, y, z = "Orange", "Banana", "Cherry"
print(x)
print(y)
print(z)
```

```py
# Orange
# Banana
# Cherry
```

One Value to Multiple Variables-

- And you can assign the same value to multiple variables in one line:

```py
x = y = z = "Orange"
print(x)
print(y)
print(z)
```

```py
# Orange
# Orange
# Orange
```

Unpack a Collection-

- If you have a collection of values in a list, tuple etc.
- Python allows you to extract the values into variables. This is called unpacking.

```py
fruits = ["apple", "banana", "cherry"]
x, y, z = fruits
print(x)
print(y)
print(z)
```

```py
# apple
# banana
# cherry
```

</details>

<details>
  <summary>4. Python Type Casting </summary>

If you want to specify the data type of a variable, this can be done with casting.

```py
x = str(3)    # x will be '3'
y = int(3)    # y will be 3
z = float(3)  # z will be 3.0

print(x)
print(y)
print(z)
```

```py
# 3
# 3
# 3.0
```

```py
x = int(1)   # x will be 1
y = int(2.8) # y will be 2
z = int("3") # z will be 3
```

```py
x = float(1)     # x will be 1.0
y = float(2.8)   # y will be 2.8
z = float("3")   # z will be 3.0
w = float("4.2") # w will be 4.2
```

```py
x = str("s1") # x will be 's1'
y = str(2)    # y will be '2'
z = str(3.0)  # z will be '3.0'
```

</details>

<details>
  <summary>5. Python get Type </summary>

You can get the data type of a variable with the type() function.

```py
x = 5
y = "John"
print(type(x))
print(type(y))
```

```py
# <class 'int'>
# <class 'str'>
```

</details>

<details>
  <summary>6. Python Global Variables </summary>

- Variables that are created outside of a function are known as global variables.

- Global variables can be used by everyone, both inside of functions and outside.

- If you create a variable with the same name inside a function, this variable will be local, and can only be used inside the function.

- The global variable with the same name will remain as it was, global and with the original value.

- Normally, when you create a variable inside a function, that variable is local, and can only be used inside that function.

- To create a global variable inside a function, you can use the global keyword.

- Also, use the global keyword if you want to change a global variable inside a function.

```py
x = "awesome"

def myfunc():
  print("Python is " + x)

myfunc()
```

```py
# Python is awesome
```

```py
x = "awesome"

def myfunc():
  x = "fantastic"
  print("Python is " + x)

myfunc()

print("Python is " + x)
```

```py
# Python is fantastic
# Python is awesome
```

```py
def myfunc():
  global x
  x = "fantastic"

myfunc()

print("Python is " + x)
```

```py
# Python is fantastic
```

```py
x = "awesome"

def myfunc():
  global x
  x = "fantastic"

myfunc()

print("Python is " + x)
```

```py
# Python is fantastic
```

</details>

<details>
  <summary>7. Python DataTypes </summary>

- In programming, data type is an important concept.

- Variables can store data of different types, and different types can do different things.

Python has the following data types built-in by default, in these categories:

```bs
Text Type:	        str
Numeric Types:	        int, float, complex
Sequence Types:	        list, tuple, range
Mapping Type:	        dict
Set Types:	        set, frozenset
Boolean Type:	        bool
Binary Types:	        bytes, bytearray, memoryview
None Type:	        NoneType
```

str:

```bs
x = "Hello World"	str
x = str("Hello World")	str
```

int, float, complex:

```bs
x = 20	        int
x = int(20)	int

x = 20.5	float
x = float(20.5)	float

x = 1j	        complex
x = complex(1j)	complex
```

list, tuple, range:

```bs
x = ["apple", "banana", "cherry"]	    list
x = list(("apple", "banana", "cherry"))	    list

x = ("apple", "banana", "cherry")	    tuple
x = tuple(("apple", "banana", "cherry"))    tuple

x = range(6)	                            range
```

dict:

```bs
x = {"name" : "John", "age" : 36}	dict
x = dict(name="John", age=36)	        dict
```

set, frozenset:

```bs
x = {"apple", "banana", "cherry"}	set
x = set(("apple", "banana", "cherry"))	set

x = frozenset({"apple", "banana", "cherry"})	frozenset
```

bool:

```bs
x = True	bool
x = bool(5)	bool
```

bytes, bytearray, memoryview:

```bs
x = b"Hello"	            bytes
x = bytes(5)	            bytes

x = bytearray(5)	    bytearray

x = memoryview(bytes(5))    memoryview
```

NoneType:

```bs
x = None	NoneType
```

</details>

+NUMBERS

<details>
  <summary>8. Python Numbers </summary>

There are three numeric types in Python:

- int
- float
- complex

Variables of numeric types are created when you assign a value to them.

- Int, or integer, is a whole number, positive or negative, without decimals, of unlimited length.

- Float, or "floating point number" is a number, positive or negative, containing one or more decimals.

- Float can also be scientific numbers with an "e" to indicate the power of 10.

- Complex numbers are written with a "j" as the imaginary part.

- You can convert from one type to another with the int(), float(), and complex() methods.

- You cannot convert complex numbers into another number type.

```py
x = 1    # int
y = 2.8  # float
z = 1j   # complex
print(type(x))
print(type(y))
print(type(z))
```

```py
# <class 'int'>
# <class 'float'>
# <class 'complex'>
```

```py
x = 1
y = 35656222554887711
z = -3255522

print(type(x))
print(type(y))
print(type(z))
```

```py
# <class 'int'>
# <class 'int'>
# <class 'int'>
```

```py
x = 1.10
y = 1.0
z = -35.59
x = 35e3
y = 12E4
z = -87.7e100

print(type(x))
print(type(y))
print(type(z))
```

```py
# <class 'float'>
# <class 'float'>
# <class 'float'>
# <class 'float'>
# <class 'float'>
# <class 'float'>
```

```py
x = 3+5j
y = 5j
z = -5j

print(type(x))
print(type(y))
print(type(z))
```

```py
# <class 'complex'>
# <class 'complex'>
# <class 'complex'>
```

```py
x = 1    # int
y = 2.8  # float
z = 1j   # complex

#convert from int to float:
a = float(x)

#convert from float to int:
b = int(y)

#convert from int to complex:
c = complex(x)

print(a)
print(b)
print(c)

print(type(a))
print(type(b))
print(type(c))
```

```py
1.0
2
(1+0j)
<class 'float'>
<class 'int'>
<class 'complex'>
```

</details>

<details>
  <summary>9. Python Random Number </summary>

Python does not have a random() function to make a random number, but Python has a built-in module called random that can be used to make random numbers.

```py
import random

print(random.randrange(1, 10))
```

```py
# 9
```

</details>

+STRINGS

<details>
  <summary>10. Python Strings </summary>

- Strings in python are surrounded by either single quotation marks, or double quotation marks.

- 'hello' is the same as "hello".

- You can display a string literal with the print() function.

- Assigning a string to a variable is done with the variable name followed by an equal sign and the string.

- You can assign a multiline string to a variable by using three quotes.

- Square brackets can be used to access elements of the string.

```py
print("Hello")
print('Hello')
```

```py
a = "Hello"
print(a)
```

```py
a = """Lorem ipsum dolor sit amet,
consectetur adipiscing elit,
sed do eiusmod tempor incididunt
ut labore et dolore magna aliqua."""
print(a)
```

```py
a = '''Lorem ipsum dolor sit amet,
consectetur adipiscing elit,
sed do eiusmod tempor incididunt
ut labore et dolore magna aliqua.'''
print(a)
```

```py
# Lorem ipsum dolor sit amet,
# consectetur adipiscing elit,
# sed do eiusmod tempor incididunt
# ut labore et dolore magna aliqua.
```

```py
a = "Hello, World!"
print(a[1])
```

```py
# e
```

</details>

<details>
  <summary>11. Python Strings - Looping </summary>

- Since strings are arrays, we can loop through the characters in a string, with a for loop.

```py
for x in "banana":
  print(x)
```

```py
# b
# a
# n
# a
# n
# a
```

</details>

<details>
  <summary>12. Python Strings - Length </summary>

- To get the length of a string, use the len() function.

```py
a = "Hello, World!"
print(len(a))
```

```py
# 13
```

</details>

<details>
  <summary>13. Python Strings - Check in String </summary>

- To check if a certain phrase or character is present in a string, we can use the keyword in.

```py
txt = "The best things in life are free!"
print("free" in txt)
```

```py
# True
```

```py
txt = "The best things in life are free!"
if "free" in txt:
  print("Yes, 'free' is present.")
```

```py
# Yes, 'free' is present.
```

</details>

<details>
  <summary>14. Python Strings - Check not in String </summary>

```py
txt = "The best things in life are free!"
print("expensive" not in txt)
```

```py
# True
```

```py
txt = "The best things in life are free!"
if "expensive" not in txt:
  print("No, 'expensive' is NOT present.")
```

```py
# No, 'expensive' is NOT present.
```

</details>

<details>
  <summary>15. Python Strings - Slicing Strings </summary>

- You can return a range of characters by using the slice syntax.

- Specify the start index and the end index, separated by a colon, to return a part of the string.

- By leaving out the start index, the range will start at the first character.

- By leaving out the end index, the range will go to the end.

- Use negative indexes to start the slice from the end of the string.

```py
b = "Hello, World!"
print(b[2:5])
```

```py
# llo
```

```py
b = "Hello, World!"
print(b[:5])
```

```py
# Hello
```

```py
b = "Hello, World!"
print(b[2:])
```

```py
# llo, World!
```

```py
b = "Hello, World!"
print(b[-5:-2])
```

```py
# orl
```

</details>

<details>
  <summary>16. Python Strings - Upper and Lower Case </summary>

- The upper() method returns the string in upper case.

- The lower() method returns the string in lower case.

```py
a = "Hello, World!"
print(a.upper())
```

```py
# HELLO, WORLD!
```

```py
a = "Hello, World!"
print(a.lower())
```

```py
# hello, world!
```

</details>

<details>
  <summary>17. Python Strings - Strip (Remove) Whitespace</summary>

- Whitespace is the space before and/or after the actual text, and very often you want to remove this space.

- The strip() method removes any whitespace from the beginning or the end

```py
a = " Hello, World! "
print(a.strip()) # returns "Hello, World!"
```

```py
# Hello, World!
```

</details>

<details>
  <summary>18. Python Strings - Replace String </summary>

- The replace() method replaces a string with another string.

```py
a = "Hello, World!"
print(a.replace("H", "J"))
```

```py
# Jello, World!
```

</details>

<details>
  <summary>19. Python Strings - Split String </summary>

- The split() method returns a list where the text between the specified separator becomes the list items.

- The split() method splits the string into substrings if it finds instances of the separator.

```py
a = "Hello, World!"
print(a.split(",")) # returns ['Hello', ' World!']
```

```py
# ['Hello', ' World!']
```

</details>

<details>
  <summary>20. Python Strings - String Concatenation </summary>

- To concatenate, or combine, two strings you can use the + operator.

```py
a = "Hello"
b = "World"
c = a + b
print(c)
```

```py
# HelloWorld
```

```py
a = "Hello"
b = "World"
c = a + " " + b
print(c)
```

```py
# Hello World
```

</details>

<details>
  <summary>21. Python Strings - Format Strings </summary>

- We can combine strings and numbers by using the format() method!

- The format() method takes the passed arguments, formats them, and places them in the string where the placeholders {} are.

- The format() method takes unlimited number of arguments, and are placed into the respective placeholders.

- You can use index numbers {0} to be sure the arguments are placed in the correct placeholders.

```py
age = 36
txt = "My name is John, and I am {}"
print(txt.format(age))
```

```py
# My name is John, and I am 36
```

```py
quantity = 3
itemno = 567
price = 49.95
myorder = "I want {} pieces of item {} for {} dollars."
print(myorder.format(quantity, itemno, price))
```

```py
# I want 3 pieces of item 567 for 49.95 dollars.
```

```py
quantity = 3
itemno = 567
price = 49.95
myorder = "I want to pay {2} dollars for {0} pieces of item {1}."
print(myorder.format(quantity, itemno, price))
```

```py
# I want to pay 49.95 dollars for 3 pieces of item 567
```

</details>

<details>
  <summary>22. Python Strings - Escape Characters </summary>

- To insert characters that are illegal in a string, use an escape character.

- An escape character is a backslash \ followed by the character you want to insert.

- An example of an illegal character is a double quote inside a string that is surrounded by double quotes. To fix this problem, use the escape character \".

```py
txt = "We are the so-called \"Vikings\" from the north."
```

```py
# We are the so-called "Vikings" from the north.
```

```bs
\'	  Single Quote
\\	  Backslash
\n	  New Line
\r	  Carriage Return
\t	  Tab
\b	  Backspace
\f	  Form Feed
\ooo	  Octal value
\xhh	  Hex value
```

</details>

<details>
  <summary>23. Python Strings - capitalize() Method</summary>

- The capitalize() method returns a string where the first character is upper case, and the rest is lower case.

```bs
string.capitalize()
```

```py
txt = "hello, and welcome to my world."

x = txt.capitalize()

print (x)
```

```py
# Hello, and welcome to my world.
```

```py
txt = "python is FUN!"

x = txt.capitalize()

print (x)
```

```py
# Python is fun!
```

```py
txt = "36 is my age."

x = txt.capitalize()

print (x)
```

```py
# 36 is my age
```

</details>

<details>
  <summary>24. Python Strings - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>25. Python Strings - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>26. Python Strings - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>27. Python Strings - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>28. Python Strings -  </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>29. Python Strings - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>30. Python Strings - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>31. Python Strings - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>32. Python Strings - </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>33. sample </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>34. sample </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>35. sample </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>36. sample </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>37. sample </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>38. sample </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>39. sample </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>40. sample </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>41. sample </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>42. sample </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>43. sample </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>44. sample </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>45. sample </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>46. sample </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>47. sample </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>48. sample </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>49. sample </summary>

```py

```

```py

```

```py

```

```py

```

</details>

<details>
  <summary>50. sample </summary>

```py

```

```py

```

```py

```

```py

```

</details>
