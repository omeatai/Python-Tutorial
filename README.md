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
  <summary>24. Python Strings - casefold() Method </summary>

- The casefold() method returns a string where all the characters are lower case.

- This method is similar to the lower() method, but the casefold() method is stronger, more aggressive, meaning that it will convert more characters into lower case, and will find more matches when comparing two strings and both are converted using the casefold() method.

```py
txt = "Hello, And Welcome To My World!"

x = txt.casefold()

print(x)
```

```py
# hello, and welcome to my world!
```

</details>

<details>
  <summary>25. Python Strings - center() Method </summary>

- The center() method will center align the string, using a specified character (space is default) as the fill character.

```bs
string.center(length, character)
```

```py
txt = "banana"

x = txt.center(20)

print(x)
```

```py
# "    banana     "
```

```py
txt = "banana"

x = txt.center(20, "O")

print(x)
```

```py
# OOOOOOObananaOOOOOOO
```

</details>

<details>
  <summary>26. Python Strings - count() Method </summary>

- The count() method returns the number of times a specified value appears in the string.

```bs
string.count(value, start, end)
```

```py
txt = "I love apples, apple are my favorite fruit"

x = txt.count("apple")

print(x)
```

```py
# 2
```

```py
txt = "I love apples, apple are my favorite fruit"

x = txt.count("apple", 10, 24)

print(x)
```

```py
# 1
```

</details>

<details>
  <summary>27. Python Strings - encode() Method </summary>

- The encode() method encodes the string, using the specified encoding. If no encoding is specified, UTF-8 will be used.

```bs
string.encode(encoding=encoding, errors=errors)
```

```py
txt = "My name is Ståle"

x = txt.encode()

print(x)
```

```py
# b'My name is St\xc3\xe5le'
```

```py
txt = "My name is Ståle"

print(txt.encode(encoding="ascii",errors="backslashreplace"))
print(txt.encode(encoding="ascii",errors="ignore"))
print(txt.encode(encoding="ascii",errors="namereplace"))
print(txt.encode(encoding="ascii",errors="replace"))
print(txt.encode(encoding="ascii",errors="xmlcharrefreplace"))
```

```py
# b'My name is St\\xe5le'
# b'My name is Stle'
# b'My name is St\\N{LATIN SMALL LETTER A WITH RING ABOVE}le'
# b'My name is St?le'
# b'My name is Ståle'
```

</details>

<details>
  <summary>28. Python Strings - endswith() Method </summary>

- The endswith() method returns True if the string ends with the specified value, otherwise False.

```bs
string.endswith(value, start, end)
```

```py
txt = "Hello, welcome to my world."

x = txt.endswith(".")

print(x)
```

```py
# True
```

```py
txt = "Hello, welcome to my world."

x = txt.endswith("my world.")

print(x)
```

```py
# True
```

```py
txt = "Hello, welcome to my world."

x = txt.endswith("my world.", 5, 11)

print(x)
```

```py
# False
```

</details>

<details>
  <summary>29. Python Strings - expandtabs() Method </summary>

- The expandtabs() method sets the tab size to the specified number of whitespaces.

```bs
string.expandtabs(tabsize)
```

```py
txt = "H\te\tl\tl\to"

x =  txt.expandtabs(2)

print(x)
```

```py
# H e l l o
```

```py
txt = "H\te\tl\tl\to"

print(txt)
print(txt.expandtabs())
print(txt.expandtabs(2))
print(txt.expandtabs(4))
print(txt.expandtabs(10))
```

```py
# H       e       l       l       o
# H       e       l       l       o
# H e l l o
# H   e   l   l   o
# H         e         l         l         o
```

</details>

<details>
  <summary>30. Python Strings - find() Method </summary>

- The find() method finds the first occurrence of the specified value.

- The find() method returns -1 if the value is not found.

- The find() method is almost the same as the index() method, the only difference is that the index() method raises an exception if the value is not found.

```bs
string.find(value, start, end)
```

```py
txt = "Hello, welcome to my world."

x = txt.find("welcome")

print(x)
```

```py
# 7
```

```py
txt = "Hello, welcome to my world."

x = txt.find("e")

print(x)
```

```py
# 1
```

```py
txt = "Hello, welcome to my world."

x = txt.find("e", 5, 10)

print(x)
```

```py
# 8
```

```py
txt = "Hello, welcome to my world."

print(txt.find("q"))
print(txt.index("q"))
```

```py
# -1
# Traceback (most recent call last):
#   File "demo_ref_string_find_vs_index.py", line 4 in <module>
#     print(txt.index("q"))
# ValueError: substring not found
```

</details>

<details>
  <summary>31. Python Strings - format() Method </summary>

- The format() method formats the specified value(s) and insert them inside the string's placeholder.

- The placeholder is defined using curly brackets: {}.

- The format() method returns the formatted string.

- The placeholders can be identified using named indexes {price}, numbered indexes {0}, or even empty placeholders {}.

```bs
string.format(value1, value2...)
```

```py
txt = "For only {price:.2f} dollars!"
print(txt.format(price = 49))
```

```py
# For only 49.00 dollars!
```

```py
txt1 = "My name is {fname}, I'm {age}".format(fname = "John", age = 36)
txt2 = "My name is {0}, I'm {1}".format("John",36)
txt3 = "My name is {}, I'm {}".format("John",36)
```

```py
# My name is John, I'm 36
# My name is John, I'm 36
# My name is John, I'm 36
```

</details>

<details>
  <summary>32. Python Strings - index() Method </summary>

- The index() method finds the first occurrence of the specified value.

- The index() method raises an exception if the value is not found.

- The index() method is almost the same as the find() method, the only difference is that the find() method returns -1 if the value is not found.

```bs
string.index(value, start, end)
```

```py
txt = "Hello, welcome to my world."

x = txt.index("welcome")

print(x)
```

```py
# 7
```

```py
txt = "Hello, welcome to my world."

x = txt.index("e")

print(x)
```

```py
# 1
```

```py
txt = "Hello, welcome to my world."

x = txt.index("e", 5, 10)

print(x)
```

```py
# 8
```

```py
txt = "Hello, welcome to my world."

print(txt.find("q"))
print(txt.index("q"))
```

```py
# -1
# Traceback (most recent call last):
#   File "demo_ref_string_find_vs_index.py", line 4 in <module>
#     print(txt.index("q"))
# ValueError: substring not found
```

</details>

<details>
  <summary>33. Python Strings - isalnum() Method </summary>

- The isalnum() method returns True if all the characters are alphanumeric, meaning alphabet letter (a-z) and numbers (0-9).

- Example of characters that are not alphanumeric: (space)!#%&? etc.

```bs
string.isalnum()
```

```py
txt = "Company12"

x = txt.isalnum()

print(x)
```

```py
# True
```

```py
txt = "Company 12"

x = txt.isalnum()

print(x)
```

```py
# False
```

</details>

<details>
  <summary>34. Python Strings - isalpha() Method </summary>

- The isalpha() method returns True if all the characters are alphabet letters (a-z).

- Example of characters that are not alphabet letters: (space)!#%&? etc.

```py
txt = "CompanyX"

x = txt.isalpha()

print(x)

```

```py
# True
```

```py
txt = "Company10"

x = txt.isalpha()

print(x)

```

```py
# False
```

</details>

<details>
  <summary>35. Python Strings - isdecimal() Method </summary>

- The isdecimal() method returns True if all the characters are decimals (0-9).

- This method is used on unicode objects.

```py
a = "\u0030" #unicode for 0
b = "\u0047" #unicode for G

print(a.isdecimal())
print(b.isdecimal())
```

```py
# True
# False
```

</details>

<details>
  <summary>36. Python Strings - isdigit() Method </summary>

- The isdigit() method returns True if all the characters are digits, otherwise False.

- Exponents, like ², are also considered to be a digit.

```py
txt = "50800"

x = txt.isdigit()

print(x)
```

```py
# True
```

```py
a = "\u0030" #unicode for 0
b = "\u00B2" #unicode for ²

print(a.isdigit())
print(b.isdigit())
```

```py
# True
# True
```

</details>

<details>
  <summary>37. Python Strings - isidentifier() Method </summary>

- The isidentifier() method returns True if the string is a valid identifier, otherwise False.

- A string is considered a valid identifier if it only contains alphanumeric letters (a-z) and (0-9), or underscores (\_).

- A valid identifier cannot start with a number, or contain any spaces.

```py
txt = "Demo"

x = txt.isidentifier()

print(x)
```

```py
# True
```

```py
a = "MyFolder"
b = "Demo002"
c = "2bring"
d = "my demo"

print(a.isidentifier())
print(b.isidentifier())
print(c.isidentifier())
print(d.isidentifier())
```

```py
# True
# True
# False
# False
```

</details>

<details>
  <summary>38. Python Strings - islower() Method </summary>

- The islower() method returns True if all the characters are in lower case, otherwise False.

- Numbers, symbols and spaces are not checked, only alphabet characters.

```py
txt = "hello world!"

x = txt.islower()

print(x)
```

```py
# True
```

```py
a = "Hello world!"
b = "hello 123"
c = "mynameisPeter"

print(a.islower())
print(b.islower())
print(c.islower())

```

```py
# False
# True
# False
```

</details>

<details>
  <summary>39. Python Strings - isnumeric() Method  </summary>

- The isnumeric() method returns True if all the characters are numeric (0-9), otherwise False.

- Exponents, like ² and ¾ are also considered to be numeric values.

- "-1" and "1.5" are NOT considered numeric values, because all the characters in the string must be numeric, and the - and the . are not.

```py
txt = "565543"

x = txt.isnumeric()

print(x)

```

```py
# True
```

```py
a = "\u0030" #unicode for 0
b = "\u00B2" #unicode for ²
c = "10km2"
d = "-1"
e = "1.5"

print(a.isnumeric())
print(b.isnumeric())
print(c.isnumeric())
print(d.isnumeric())
print(e.isnumeric())

```

```py
# True
# True
# False
# False
# False
```

</details>

<details>
  <summary>40. Python Strings - isprintable() Method </summary>

- The isprintable() method returns True if all the characters are printable, otherwise False.

- Example of none printable character can be carriage return and line feed.

```py
txt = "Hello! Are you #1?"

x = txt.isprintable()

print(x)

```

```py
# True
```

```py
txt = "Hello!\nAre you #1?"

x = txt.isprintable()

print(x)
```

```py
# False
```

</details>

<details>
  <summary>41. Python Strings - isspace() Method  </summary>

The isspace() method returns True if all the characters in a string are whitespaces, otherwise False.

```py
txt = "   "

x = txt.isspace()

print(x)
```

```py
# True
```

```py
txt = "   s   "

x = txt.isspace()

print(x)

```

```py
# False
```

</details>

<details>
  <summary>42. Python Strings - istitle() Method </summary>

- The istitle() method returns True if all words in a text start with a upper case letter, AND the rest of the word are lower case letters, otherwise False.

- Symbols and numbers are ignored.

```py
txt = "Hello, And Welcome To My World!"

x = txt.istitle()

print(x)

```

```py
# True
```

```py
a = "HELLO, AND WELCOME TO MY WORLD"
b = "Hello"
c = "22 Names"
d = "This Is %'!?"

print(a.istitle())
print(b.istitle())
print(c.istitle())
print(d.istitle())

```

```py
# False
# True
# True
# True
```

</details>

<details>
  <summary>43. Python Strings - isupper() Method  </summary>

- The isupper() method returns True if all the characters are in upper case, otherwise False.

- Numbers, symbols and spaces are not checked, only alphabet characters.

```py
txt = "THIS IS NOW!"

x = txt.isupper()

print(x)

```

```py
# True
```

```py
a = "Hello World!"
b = "hello 123"
c = "MY NAME IS PETER"

print(a.isupper())
print(b.isupper())
print(c.isupper())

```

```py
# False
# False
# True
```

</details>

<details>
  <summary>44. Python Strings - join() Method  </summary>

- The join() method takes all items in an iterable and joins them into one string.

- A string must be specified as the separator.

```py
myTuple = ("John", "Peter", "Vicky")

x = "#".join(myTuple)

print(x)
```

```py
# John#Peter#Vicky
```

```py
myDict = {"name": "John", "country": "Norway"}
mySeparator = "TEST"

x = mySeparator.join(myDict)

print(x)

```

```py
# nameTESTcountry
```

</details>

<details>
  <summary>45. Python Strings - ljust() Method </summary>

The ljust() method will left align the string, using a specified character (space is default) as the fill character.

```py
txt = "banana"

x = txt.ljust(20)

print(x, "is my favorite fruit.")
```

```py
# banana              is my favorite fruit.
```

```py
txt = "banana"

x = txt.ljust(20, "O")

print(x)

```

```py
# bananaOOOOOOOOOOOOOO
```

</details>

<details>
  <summary>46. Python Strings - lower() Method </summary>

- The lower() method returns a string where all characters are lower case.

- Symbols and Numbers are ignored.

```py
txt = "Hello my FRIENDS"

x = txt.lower()

print(x)

```

```py
# hello my friends
```

</details>

<details>
  <summary>47. Python Strings - lstrip() Method </summary>

The lstrip() method removes any leading characters (space is the default leading character to remove).

```py
txt = "     banana     "

x = txt.lstrip()

print("of all fruits", x, "is my favorite")
```

```py
# of all fruits banana     is my favorite
```

```py
txt = ",,,,,ssaaww.....banana"

x = txt.lstrip(",.asw")

print(x)

```

```py
# banana
```

</details>

<details>
  <summary>48. Python Strings - maketrans() Method </summary>

- The maketrans() method returns a mapping table that can be used with the translate() method to replace specified characters.

```py
txt = "Hello Sam!"

mytable = txt.maketrans("S", "P")

print(txt.translate(mytable))

```

```py
# Hello Pam!
```

```py
txt = "Hi Sam!"

x = "mSa"
y = "eJo"

mytable = txt.maketrans(x, y)

print(txt.translate(mytable))

```

```py
# Hi Joe!
```

```py
txt = "Good night Sam!"

x = "mSa"
y = "eJo"
z = "odnght"

mytable = txt.maketrans(x, y, z)

print(txt.translate(mytable))
```

```py
# G i Joe!
```

</details>

<details>
  <summary>49. Python Strings - partition() Method </summary>

- The partition() method searches for a specified string, and splits the string into a tuple containing three elements.

- The first element contains the part before the specified string.

- The second element contains the specified string.

- The third element contains the part after the string.

```py
txt = "I could eat bananas all day"

x = txt.partition("bananas")

print(x)

```

```py
# ('I could eat ', 'bananas', ' all day')
```

```py
txt = "I could eat bananas all day"

x = txt.partition("apples")

print(x)

```

```py
# ('I could eat bananas all day', '', '')
```

</details>

<details>
  <summary>50. Python Strings - replace() Method </summary>

The replace() method replaces a specified phrase with another specified phrase.

```py
txt = "I like bananas"

x = txt.replace("bananas", "apples")

print(x)
```

```py
# I like apples
```

```py
txt = "one one was a race horse, two two was one too."

x = txt.replace("one", "three")

print(x)

```

```py
# three three was a race horse, two two was three too."
```

```py
txt = "one one was a race horse, two two was one too."

x = txt.replace("one", "three", 2)

print(x)

```

```py
# three three was a race horse, two two was one too."
```

</details>

<details>
  <summary>51. Python Strings - rfind() Method </summary>

- The rfind() method finds the last occurrence of the specified value.

- The rfind() method returns -1 if the value is not found.

- The rfind() method is almost the same as the rindex() method.

```py
txt = "Mi casa, su casa."

x = txt.rfind("casa")

print(x)

```

```py
# 12
```

```py
txt = "Hello, welcome to my world."

x = txt.rfind("e")

print(x)

```

```py
# 13
```

```py
txt = "Hello, welcome to my world."

x = txt.rfind("e", 5, 10)

print(x)

```

```py
# 8
```

```py
txt = "Hello, welcome to my world."

print(txt.rfind("q"))
print(txt.rindex("q"))
```

```py
# -1
# Traceback (most recent call last):
#   File "demo_ref_string_rfind_vs_rindex.py", line 4 in <module>
#     print(txt.rindex("q"))
# ValueError: substring not found
```

</details>

<details>
  <summary>52. Python Strings - rindex() Method </summary>

- The rindex() method finds the last occurrence of the specified value.

- The rindex() method raises an exception if the value is not found.

- The rindex() method is almost the same as the rfind() method.

```py
txt = "Mi casa, su casa."

x = txt.rindex("casa")

print(x)

```

```py
# 12
```

```py
txt = "Hello, welcome to my world."

x = txt.rindex("e")

print(x)

```

```py
# 13
```

```py
txt = "Hello, welcome to my world."

x = txt.rindex("e", 5, 10)

print(x)
```

```py
# 8
```

```py
txt = "Hello, welcome to my world."

print(txt.rfind("q"))
print(txt.rindex("q"))
```

```py
# -1
# Traceback (most recent call last):
#   File "demo_ref_string_rfind_vs_rindex.py", line 4 in <module>
#     print(txt.rindex("q"))
# ValueError: substring not found
```

</details>

<details>
  <summary>53. Python Strings - rjust() Method  </summary>

The rjust() method will right align the string, using a specified character (space is default) as the fill character.

```py
txt = "banana"

x = txt.rjust(20)

print(x, "is my favorite fruit.")
```

```py
#                  banana is my favorite fruit.
```

```py
txt = "banana"

x = txt.rjust(20, "O")

print(x)

```

```py
# OOOOOOOOOOOOOObanana
```

</details>

<details>
  <summary>54. Python Strings - rpartition() Method </summary>

- The rpartition() method searches for the last occurrence of a specified string, and splits the string into a tuple containing three elements.

- The first element contains the part before the specified string.

- The second element contains the specified string.

- The third element contains the part after the string.

```py
txt = "I could eat bananas all day, bananas are my favorite fruit"

x = txt.rpartition("bananas")

print(x)
```

```py
# ('I could eat bananas all day, ', 'bananas', ' are my favorite fruit')
```

```py
txt = "I could eat bananas all day, bananas are my favorite fruit"

x = txt.rpartition("apples")

print(x)
```

```py
# ('', '', 'I could eat bananas all day, bananas are my favorite fruit')
```

</details>

<details>
  <summary>55. Python Strings - rsplit() Method </summary>

- The rsplit() method splits a string into a list, starting from the right.

- If no "max" is specified, this method will return the same as the split() method.

```py
txt = "apple, banana, cherry"

x = txt.rsplit(", ")

print(x)
```

```py
# ['apple', 'banana', 'cherry']
```

```py
txt = "apple, banana, cherry"

# setting the maxsplit parameter to 1, will return a list with 2 elements!
x = txt.rsplit(", ", 1)

print(x)

# note that the result has only 2 elements "apple, banana" is the first element, and "cherry" is the last.
```

```py
['apple, banana', 'cherry']
```

</details>

<details>
  <summary>56. Python Strings - rstrip() Method </summary>

The rstrip() method removes any trailing characters (characters at the end a string), space is the default trailing character to remove.

```py
txt = "     banana     "

x = txt.rstrip()

print("of all fruits", x, "is my favorite")
```

```py
# of all fruits     banana is my favorite
```

```py
txt = "banana,,,,,ssqqqww....."

x = txt.rstrip(",.qsw")

print(x)

```

```py
# banana
```

</details>

<details>
  <summary>57. Python Strings - split() Method </summary>

```py
txt = "welcome to the jungle"

x = txt.split()

print(x)
```

```py
# ['welcome', 'to', 'the', 'jungle']
```

```py
txt = "hello, my name is Peter, I am 26 years old"

x = txt.split(", ")

print(x)
```

```py
# ['hello', 'my name is Peter', 'I am 26 years old']
```

```py
txt = "apple#banana#cherry#orange"

x = txt.split("#")

print(x)

```

```py
# ['apple', 'banana', 'cherry', 'orange']
```

```py
txt = "apple#banana#cherry#orange"

# setting the maxsplit parameter to 1, will return a list with 2 elements!
x = txt.split("#", 1)

print(x)
```

```py
# ['apple', 'banana#cherry#orange']
```

</details>

<details>
  <summary>58. Python Strings - splitlines() Method </summary>

The splitlines() method splits a string into a list. The splitting is done at line breaks.

```py
txt = "Thank you for the music\nWelcome to the jungle"

x = txt.splitlines()

print(x)

```

```py
# ['Thank you for the music', 'Welcome to the jungle']
```

```py
txt = "Thank you for the music\nWelcome to the jungle"

x = txt.splitlines(True)

print(x)

```

```py
# ['Thank you for the music\n', 'Welcome to the jungle']
```

</details>

<details>
  <summary>59. Python Strings - startswith() Method </summary>

The startswith() method returns True if the string starts with the specified value, otherwise False.

```py
txt = "Hello, welcome to my world."

x = txt.startswith("Hello")

print(x)

```

```py
# True
```

```py
txt = "Hello, welcome to my world."

x = txt.startswith("wel", 7, 20)

print(x)

```

```py
# True
```

</details>

<details>
  <summary>60. Python Strings - strip() Method </summary>

The strip() method removes any leading (spaces at the beginning) and trailing (spaces at the end) characters (space is the default leading character to remove).

```py
txt = "     banana     "

x = txt.strip()

print("of all fruits", x, "is my favorite")

```

```py
# of all fruits banana is my favorite
```

```py
txt = ",,,,,rrttgg.....banana....rrr"

x = txt.strip(",.grt")

print(x)

```

```py
# banana
```

</details>

<details>
  <summary>61. Python Strings - swapcase() Method </summary>

The swapcase() method returns a string where all the upper case letters are lower case and vice versa.

```py
txt = "Hello My Name Is PETER"

x = txt.swapcase()

print(x)

```

```py
# hELLO mY nAME iS peter
```

</details>

<details>
  <summary>62. Python Strings - title() Method </summary>

- The title() method returns a string where the first character in every word is upper case. Like a header, or a title.

- If the word contains a number or a symbol, the first letter after that will be converted to upper case.

```py
txt = "Welcome to my world"

x = txt.title()

print(x)
```

```py
# Welcome To My World
```

```py
txt = "Welcome to my 2nd world"

x = txt.title()

print(x)

```

```py
# Welcome To My 2Nd World
```

</details>

<details>
  <summary>63. Python Strings - translate() Method </summary>

- The translate() method returns a string where some specified characters are replaced with the character described in a dictionary, or in a mapping table.

- Use the maketrans() method to create a mapping table.

- If a character is not specified in the dictionary/table, the character will not be replaced.

- If you use a dictionary, you must use ascii codes instead of characters.

```py
#use a dictionary with ascii codes to replace 83 (S) with 80 (P):
mydict = {83:  80}

txt = "Hello Sam!"

print(txt.translate(mydict))

```

```py
# Hello Pam!
```

```py
txt = "Hello Sam!"

mytable = txt.maketrans("S", "P")

print(txt.translate(mytable))

```

```py
# Hello Pam!
```

```py
txt = "Hi Sam!"

x = "mSa"
y = "eJo"

mytable = txt.maketrans(x, y)

print(txt.translate(mytable))

```

```py
# Hi Joe!
```

```py
txt = "Good night Sam!"

x = "mSa"
y = "eJo"
z = "odnght"

mytable = txt.maketrans(x, y, z)

print(txt.translate(mytable))

```

```py
# G i Joe!
```

```py
txt = "Good night Sam!"

mydict = {109: 101, 83: 74, 97: 111, 111: None, 100: None, 110: None, 103: None, 104: None, 116: None}

print(txt.translate(mydict))

```

```py
# G i Joe!
```

</details>

<details>
  <summary>64. Python Strings - upper() Method </summary>

- The upper() method returns a string where all characters are in upper case.

- Symbols and Numbers are ignored.

```py
txt = "Hello my friends"

x = txt.upper()

print(x)

```

```py
# HELLO MY FRIENDS
```

</details>

<details>
  <summary>65. Python Strings - zfill() Method </summary>

- The zfill() method adds zeros (0) at the beginning of the string, until it reaches the specified length.

- If the value of the len parameter is less than the length of the string, no filling is done.

```py
txt = "50"

x = txt.zfill(10)

print(x)

```

```py
# 0000000050
```

```py
a = "hello"
b = "welcome to the jungle"
c = "10.000"

print(a.zfill(10))
print(b.zfill(10))
print(c.zfill(10))
```

```py
# 00000hello
# welcome to the jungle
# 000010.000
```

</details>

<details>
  <summary>66. sample </summary>

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
  <summary>67. sample </summary>

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
  <summary>68. sample </summary>

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
  <summary>69. sample </summary>

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
  <summary>70. sample </summary>

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
  <summary>71. sample </summary>

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
  <summary>72. sample </summary>

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
  <summary>73. sample </summary>

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
  <summary>74. sample </summary>

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
  <summary>75. sample </summary>

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
  <summary>76. sample </summary>

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
  <summary>77. sample </summary>

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
  <summary>78. sample </summary>

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
  <summary>79. sample </summary>

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
  <summary>80. sample </summary>

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
  <summary>81. sample </summary>

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
  <summary>82. sample </summary>

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
  <summary>83. sample </summary>

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
  <summary>84. sample </summary>

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
  <summary>85. sample </summary>

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
  <summary>86. sample </summary>

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
  <summary>87. sample </summary>

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
  <summary>88. sample </summary>

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
  <summary>89. sample </summary>

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
  <summary>99. sample </summary>

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
  <summary>100. sample </summary>

```py

```

```py

```

```py

```

```py

```

</details>
