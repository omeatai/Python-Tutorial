# Python-Tutorial

Python Tutorial by Ifeanyi Omeata

## Tutorial

---

### [1-100 Days of Code: The Complete Python Pro Bootcamp for 2023 - ANGELA YU]()

<details>
  <summary>1. Introduction - Print Function </summary>

```py
# input() will get user input in console
# Then print() will print the word "Hello" and the user input
print("Hello + input("What is your name?"))
```

```py
# What is your name? Bob
# Hello Bob
```

```py
#This code prints the number of characters in a user's name.
print(len input ("What is your name?") ) )
```

```py
# What is your name? Bob
# 3
```

```py
name = input("What is your name?")
print(name)
```

```py
# What is your name? Mark
# Mark
```

```py
#1. Create a greeting for your program.
print("Welcome to the band name generator.")
#2. Ask the user for the city that they grew up in.
city = input("Which city did you grow up in?\n")
#3. Ask the user for the name of a pet.
pet = input("What is the name of a pet?\n")
#4. Combine the name of their city and pet and show them their band name.
print("Your band name could be " + city + " " + pet)
#5. Make sure the input cursor shows on a new line, see the example at:
# https://band-name-generator-end.appbrewery.repl.run/
```

```py
# Welcome to the band name generator.
# Which city did you grow up in?
# Bristol
# What is the name of a pet?
# Rabbit
# Your band name could be  Bristol Rabbit
```

</details>

<details>
  <summary>2. Number Manipulation </summary>

Rounding Numbers:

```py
print(round(8 / 3, 2))
```

```py
# 2.67
```

Flooring Numbers:

```py
print(8 // 3)
```

```py
# 2
```

```py
result = 4 / 2
result /= 2
print(result)
```

```py
# 1.0
```

```py
score = 0
score += 1
print(score)

```

```py
# 1
```

</details>

<details>
  <summary>3. Using F Strings </summary>

```py
score = 0
print("your score is " + str(score))
```

```py
score = 0
height = 1.8
isWinning = True
#f-String
print (f"your score is {score}")
```

```py
# your score is 0
```

```py
score = 0
height = 1.8
isWinning = True
#f-String
print(f"your score is {score}, your height is {height}, you are winning is {isWinning}")
```

```py
# your score is 0, your height is 1.8, you are winning is True
```

```py
age = input("What is your current age? ")

rem = (90 - int(age))
d =  rem * 365
w = rem * 52
m = rem * 12

print(f"You have {d} days, {w} weeks, and {m} months left.")
```

```py
# What is your current age? 35
# You have 20075 days, 2860 weeks, and 660 months left.
```

Using the Format function:

```py
format(salesAmount, '.2f')
```

Using the Format Method:

```py
"{:.2f}".format(salesAmount)
```

```py
print("Welcome to the tip calculator!")
bill = float(input("What was the total bill?\n$"))
tip = int(input("How much tip would you like to give? 10, 12, or 15?\n"))
people = int(input("How many people to split the bill?\n"))
bill_with_tip = (tip/100+1) * bill
bill_for_each_person = "{:.2f}".format(bill_with_tip/people)
print(f'Each person should pay: ${bill_for_each_person}.')
```

```py
# Welcome to the tip calculator!
# What was the total bill?
# $150.00
# How much tip would you like to give? 10, 12, or 15?
# 12
# How many people to split the bill?
# 5
# Each person should pay: $33.60.
```

</details>

<details>
  <summary>4. If Else Statements </summary>

```py
print("Welcome to the rollercoaster!")
height = int(input("What is your height in cm? "))

if height > 120:
	print("You can ride the rollercoaster!")
else:
	print("Sorry, you have to grow taller before you can ride.")
```

```py
# Welcome to the rollercoaster!
# What is your height in cm? 180
# You can ride the rollercoaster!
```

```py
number = int(input("Which number do you want to check? "))

if number%2 == 0:
    print('This is an even number.')
else:
    print('This is an odd number.')
```

```py
# Which number do you want to check? 51
# This is an odd number.
```

Nested If/Else:

```py
print("Welcome to the rollercoaster!")
height = int(input("What is your height in cm? "))

if height >= 120:
	print("You can ride the rollercoaster!")
	age = int(input("What is your age? "))
	if age <= 18:
		print("Please pay $7.")
	else:
		print("Please pay $12.")
else:
	print("Sorry, you have to grow taller before you can ride.")
```

```py
# Welcome to the rollercoaster!
# What is your height in cm? 180
# You can ride the rollercoaster!
# What is your age? 19
# Please pay $12.
```

Nested If/Elif/Else:

```py
if condition1:
  do A
elif condition2:
  do B
else:
  do this
```

```py
print("Welcome to the rollercoaster!")
height = int(input("What is your height in cm? "))

if height >= 120:
	print("You can ride the rollercoaster!")
	age = int(input("What is your age? "))

	if age < 12:
		print("Please pay $5.")
	elif age <= 18:
		print("Please pay $7.")
	else:
		print("Please pay $12.")
else:
	print("Sorry, you have to grow taller before you can ride.")
```

```py
# Welcome to the rollercoaster!
# What is your height in cm? 180
# You can ride the rollercoaster!
# What is your age? 11
# Please pay $5.
```

```py
height = float(input("enter your height in m: "))
weight = float(input("enter your weight in kg: "))

bmi = round(weight / height**2)

if bmi < 18.5:
    print(f"Your BMI is {bmi}, you are underweight.")
elif bmi < 25:
    print(f"Your BMI is {bmi}, you have a normal weight.")
elif bmi < 30:
    print(f"Your BMI is {bmi}, you are slightly overweight.")
elif bmi < 35:
    print(f"Your BMI is {bmi}, you are obese.")
else:
    print(f"Your BMI is {bmi}, you are clinically obese.")

```

```py
# enter your height in m: 1.8034
# enter your weight in kg: 120
# Your BMI is 37, you are clinically obese.
```

```py

```

```py

```

</details>

<details>
  <summary>5. sample </summary>

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
  <summary>6. sample </summary>

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
  <summary>7. sample </summary>

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
  <summary>8. sample </summary>

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
  <summary>9. sample </summary>

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
  <summary>10. sample </summary>

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
  <summary>11. sample </summary>

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
  <summary>12. sample </summary>

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
  <summary>13. sample </summary>

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
  <summary>14. sample </summary>

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
  <summary>15. sample </summary>

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
  <summary>16. sample </summary>

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
  <summary>17. sample </summary>

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
  <summary>18. sample </summary>

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
  <summary>19. sample </summary>

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
  <summary>20. sample </summary>

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
  <summary>21. sample </summary>

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
  <summary>22. sample </summary>

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
  <summary>23. sample </summary>

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
  <summary>24. sample </summary>

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
  <summary>25. sample </summary>

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
  <summary>26. sample </summary>

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
  <summary>27. sample </summary>

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
  <summary>28. sample </summary>

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
  <summary>29. sample </summary>

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
  <summary>30. sample </summary>

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
  <summary>31. sample </summary>

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
  <summary>32. sample </summary>

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

<details>
  <summary>51. sample </summary>

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
  <summary>52. sample </summary>

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
  <summary>53. sample </summary>

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
  <summary>54. sample </summary>

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
  <summary>55. sample </summary>

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
  <summary>56. sample </summary>

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
  <summary>57. sample </summary>

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
  <summary>58. sample </summary>

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
  <summary>59. sample </summary>

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
  <summary>60. sample </summary>

```py

```

```py

```

```py

```

```py

```

</details>
