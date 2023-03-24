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
year = int(input("Which year do you want to check? "))

if year % 4 == 0:
    if not year % 100 == 0 or year % 100 == 0 and year % 400 == 0:
        print('Leap year.')
    else:
        print('Not leap year.')
else:
    print('Not leap year.')
```

```py
# Which year do you want to check? 2000
# Leap year.
```

Multiple If statements:

```py
print("Welcome to the rollercoaster!")
height = int(input("What is your height in cm? "))
bill = 0

if height >= 120:
	print("You can ride the rollercoaster!")
	age = int(input("What is your age? "))
	if age < 12:
		bill = 5
		print("Child tickets are $5.")
	elif age <= 18:
		bill = 7
		print("Youth tickets are $7.")
	else:
		bill = 12
		print("Adult tickets are $12.")

	wants_photo = input("Do you want a photo taken? Y or N. ")
	if wants_photo == "Y":
		bill += 3
	print(f"Your final bill is ${bill}.")
else:
	print("Sorry, you have to grow taller before you can ride.")
```

```py
# Welcome to the rollercoaster!
# What is your height in cm? 181
# You can ride the rollercoaster!
# What is your age? 22
# Adult tickets are $12.
# Do you want a photo taken? Y or N. Y
# Your final bill is $15.
```

```py
print("Welcome to Python Pizza Deliveries!")
size = input("What size pizza do you want? S, M, or L ")
add_pepperoni = input("Do you want pepperoni? Y or N ")
extra_cheese = input("Do you want extra cheese? Y or N ")

bill = 0
pepperoni_bill = 0

if size == "S":
  bill += 15
elif size == "M":
  bill += 20
  pepperoni_bill = 3
else:
  bill += 25
  pepperoni_bill = 3

if add_pepperoni == "Y":
	if size == "S":
		bill += 2
	else:
		bill += 3

if extra_cheese == "Y":
  bill += 1

print(f"Your final bill is: ${bill}.")
```

```py
# Welcome to Python Pizza Deliveries!
# What size pizza do you want? S, M, or L S
# Do you want pepperoni? Y or N N
# Do you want extra cheese? Y or N Y
# Your final bill is: $16.
```

```py
print("Welcome to the Love Calculator!")
name1 = input("What is your name? \n")
name2 = input("What is their name? \n")

true = "true"
love = "love"
names = (name1 + name2).lower().strip()
true_count = 0
love_count = 0

for i in true:
    true_count += names.count(i)

for j in love:
    love_count += names.count(j)

love_score = int(f"{true_count}{love_count}")

if love_score < 10 or love_score > 90:
    print(f"Your score is {love_score}, you go together like coke and mentos.")
elif love_score >= 40 and love_score =< 50:
    print(f"Your score is {love_score}, you are alright together.")
else:
    print(f"Your score is {love_score}.")
```

```py
# Welcome to the Love Calculator!
# What is your name?
# Kanye West
# What is their name?
# Kim Kardashian
# Your score is 42, you are alright together.
```

```py
print("Welcome to Tresure Island.")
print("Your mission is to find the treasure.")

choice1=input('You\'re at a crossroad, where do you want to go? Type "left" or "right". ').lower()

if choice1 == "left":
	choice2=input('You\'ve come to a lake. There is an island in the middle of the lake. Type "wait" to wait for a boat. Type "swim" to swim across.').lower()
	if choice2 == "wait":
		choice3 = input("You arrive at the island unharmed. There is a house with 3 doors.One red, one yellow and one blue. Which colour do you choose?").lower()
		if choice3 == "red":
			print("It's a room full of fire. Game Over.")
		elif choice3 == "yellow":
			print("You found the treasure! You Win!")
		elif choice3 == "blue":
			print("You enter a room of beasts. Game Over.")
		else:
			print("You chose a door that doesn't exist. Game Over.")
	else:
		print("You got attacked by an angry trout. Game Over.")
else:
	print("You fell into a hole. Game Over.")
```

```py
# Welcome to Tresure Island.
# Your mission is to find the treasure.
# You're at a crossroad, where do you want to go? Type "left" or "right". left
# You've come to a lake. There is an island in the middle of the lake. Type "wait" to wait for a boat. Type "swim" to swim across.wait
# You arrive at the island unharmed. There is a house with 3 doors.One red, one yellow and one blue. Which colour do you choose?yellow
# You found the treasure! You Win!
```

```py
import random

listofnum = [1, 2, 3, 4, 5]
# 1
print(random.choice(listofnum))

# 2
random.shuffle(listofnum)
print(listofnum)
```

```py
# 4
# [2, 1, 4, 5, 3]
```

```py
import random

print("Welcome to Treasure Island.")
print("Your mission is to find the treasure.")

start = 'ON'

choices = ['left', 'right']
random_choice = random.choice(choices)
# print(random_choice)
choice = input(
    "You're at a cross road. Where do you want to go? Type 'left' or 'right'\n"
).lower().strip()
if choice == random_choice:
    print('Great Choice! Way to go. keep going forward....')
else:
    print('Fall into a Hole. Game Over.')
    start = 'OFF'

choices = ['swim', 'wait']
random_choice = random.choice(choices)
# print(random_choice)
if start == 'ON':
    choice = input(
        "You come to a lake. There is an island in the middle of the lake. Type 'wait' to wait for a boat. Type 'swim' to swim across.\n"
    ).lower().strip()

    if choice == random_choice:
        print('Great Choice! Way to go. keep going forward....')
    else:
        print('Attacked by Trout. Game Over.')
        start = 'OFF'

choices = ['red', 'yellow', 'blue']
random_choice = random.choice(choices)
# print(random_choice)
if start == 'ON':
    choice = input(
        "You arrive at the island unharmed. There is a house with 3 doors. One red, one yellow and one blue. Which colour do you choose?\n"
    ).lower().strip()

    if choice == random_choice:
        print('Congratulations! You WON the challenge....')
    elif choice == "red":
        print('Burned by Fire. Game Over.')
    elif choice == "blue":
        print('Eaten by Beasts. Game Over.')
    else:
        print('Drowned by Water. Game Over.')
```

```py
# Welcome to Treasure Island.
# Your mission is to find the treasure.
# You're at a cross road. Where do you want to go? Type 'left' or 'right'
# left
# Great Choice! Way to go. keep going forward....
# You come to a lake. There is an island in the middle of the lake. Type 'wait' to wait for a boat. Type 'swim' to swim across.
# swim
# Great Choice! Way to go. keep going forward....
# You arrive at the island unharmed. There is a house with 3 doors. One red, one yellow and one blue. Which colour do you choose?
# yellow
# Congratulations! You WON the challenge....
```

</details>

<details>
  <summary>5. Importing Modules </summary>

Import from a single module in same folder -

person.py:

```py
name = "Ben"
account_no = "113748919"
age = 21
```

main:

```py
from person import account_no

print(account_no)
```

```py
# 113748919
```

Import from multiple modules in same folder -

person.py:

```py
name = "Ben"
account_no = "113748919"
age = 21
```

school.py:

```py
department = "Economics"
year = 2011
```

main.py:

```py
from person import account_no
from school import year

print(account_no)
print(year)

```

```py
# 113748919
# 2011
```

Import from multiple modules in different folder -

host/init.py:

```py
__all__ = ["person", "school"]
```

host/person.py:

```py
name = "Ben"
account_no = "113748919"
age = 21
```

host/school.py:

```py
department = "Economics"
year = 2011
```

main.py:

```py
from host import *

print(person.account_no)
print(school.year)

```

```py
# 113748919
# 2011
```

</details>

<details>
  <summary>6. Generating Random Numbers </summary>

```py
import random

#Random number between 1 and 10
random_integer = random.randint(1, 10)
print(random_integer)

#Random number between 0 and 1
random_float = random.random()
print(random_float)
```

```py
# 4
# 0.35402952193969894
```

Random number between 0 and 5:

```py
import random

#Random number between 1 and 10
random_integer = random.randint(1, 10)
# print(random_integer)

#Random number between 0 and 1
random_float = random.random()
# print(random_float)

#Random number between 0 and 5
for i in range(21):
    print(f"{i}: {format(round(random.random() * 5,2),'.2f')}")
```

```py
# 0: 2.61
# 1: 1.78
# 2: 1.57
# 3: 4.22
# 4: 0.43
# 5: 2.41
# 6: 2.86
# 7: 3.35
# 8: 4.37
# 9: 1.13
# 10: 0.60
# 11: 0.66
# 12: 3.54
# 13: 3.69
# 14: 2.81
# 15: 2.98
# 16: 3.79
# 17: 3.87
# 18: 3.01
# 19: 3.88
# 20: 0.95
```

Select randomly from list of Choices:

```py
import random

print(random.choice(["Heads", "Tails"]))
```

```py
# Tails
```

```py
import random

random_side = random.randint(0, 1)

if random_side == 1:
    print("Heads")
else:
    print("Tails")
```

```py
# Heads
```

</details>

<details>
  <summary>7. Python Lists </summary>

Get a List Item from the index Position:

```py
states_of_america = [
    "Delaware", "Pennsylvania", "New Jersey", "Georgia", "Connecticut",
    "Massachusetts", "Maryland", "South Carolina", "New Hampshire", "Virginia",
    "New York", "North Carolina", "Rhode Island", "Vermont", "Kentucky",
    "Tennessee", "Ohio", "Louisiana", "Indiana", "Mississippi", "Illinois",
    "Alabama", "Maine", "Missouri", "Arkansas", "Michigan", "Florida", "Texas",
    "Iowa", "Wisconsin", "California", "Minnesota", "Oregon", "Kansas",
    "West Virginia", "Nevada", "Nebraska", "Colorado", "North Dakota",
    "South Dakota", "Montana", "Washington", "Idaho", "Wyoming", "Utah",
    "Oklahoma", "New Mexico", "Arizona", "Alaska", "Hawaii"
]

print(states_of_america[0])
```

```py
# Delaware
```

Get an Item from the end of the list:

```py
states_of_america = [
    "Delaware", "Pennsylvania", "New Jersey", "Georgia", "Connecticut",
    "Massachusetts", "Maryland", "South Carolina", "New Hampshire", "Virginia",
    "New York", "North Carolina", "Rhode Island", "Vermont", "Kentucky",
    "Tennessee", "Ohio", "Louisiana", "Indiana", "Mississippi", "Illinois",
    "Alabama", "Maine", "Missouri", "Arkansas", "Michigan", "Florida", "Texas",
    "Iowa", "Wisconsin", "California", "Minnesota", "Oregon", "Kansas",
    "West Virginia", "Nevada", "Nebraska", "Colorado", "North Dakota",
    "South Dakota", "Montana", "Washington", "Idaho", "Wyoming", "Utah",
    "Oklahoma", "New Mexico", "Arizona", "Alaska", "Hawaii"
]

print(states_of_america[-2])
```

```py
# Alaska
```

Changing the value of an item in the List:

```py
states_of_america = [
    "Delaware", "Pennsylvania", "New Jersey", "Georgia", "Connecticut",
    "Massachusetts", "Maryland", "South Carolina", "New Hampshire", "Virginia",
    "New York", "North Carolina", "Rhode Island", "Vermont", "Kentucky",
    "Tennessee", "Ohio", "Louisiana", "Indiana", "Mississippi", "Illinois",
    "Alabama", "Maine", "Missouri", "Arkansas", "Michigan", "Florida", "Texas",
    "Iowa", "Wisconsin", "California", "Minnesota", "Oregon", "Kansas",
    "West Virginia", "Nevada", "Nebraska", "Colorado", "North Dakota",
    "South Dakota", "Montana", "Washington", "Idaho", "Wyoming", "Utah",
    "Oklahoma", "New Mexico", "Arizona", "Alaska", "Hawaii"
]

states_of_america[1] = "Pencilvania"
print(states_of_america[1])
```

```py
# Pencilvania
```

Adding Items to a List:

```py
states_of_america = [
    "Delaware", "Pennsylvania", "New Jersey", "Georgia", "Connecticut",
    "Massachusetts", "Maryland", "South Carolina", "New Hampshire", "Virginia",
    "New York", "North Carolina", "Rhode Island", "Vermont", "Kentucky",
    "Tennessee", "Ohio", "Louisiana", "Indiana", "Mississippi", "Illinois",
    "Alabama", "Maine", "Missouri", "Arkansas", "Michigan", "Florida", "Texas",
    "Iowa", "Wisconsin", "California", "Minnesota", "Oregon", "Kansas",
    "West Virginia", "Nevada", "Nebraska", "Colorado", "North Dakota",
    "South Dakota", "Montana", "Washington", "Idaho", "Wyoming", "Utah",
    "Oklahoma", "New Mexico", "Arizona", "Alaska", "Hawaii"
]

states_of_america.append("Angelaland")
print(states_of_america[-1])
```

```py
# Angelaland
```

Adding more than one item to the List:

```py
states_of_america = [
    "Delaware", "Pennsylvania", "New Jersey", "Georgia", "Connecticut",
    "Massachusetts", "Maryland", "South Carolina", "New Hampshire", "Virginia",
    "New York", "North Carolina", "Rhode Island", "Vermont", "Kentucky",
    "Tennessee", "Ohio", "Louisiana", "Indiana", "Mississippi", "Illinois",
    "Alabama", "Maine", "Missouri", "Arkansas", "Michigan", "Florida", "Texas",
    "Iowa", "Wisconsin", "California", "Minnesota", "Oregon", "Kansas",
    "West Virginia", "Nevada", "Nebraska", "Colorado", "North Dakota",
    "South Dakota", "Montana", "Washington", "Idaho", "Wyoming", "Utah",
    "Oklahoma", "New Mexico", "Arizona", "Alaska", "Hawaii"
]

states_of_america.extend(["Angelaland", "Lagosland", "Hopeland"])
print(states_of_america[-5:])

```

```py
# ['Alaska', 'Hawaii', 'Angelaland', 'Lagosland', 'Hopeland']
```

Randomly selecting items from a List:

```py
import random

names_string = input("Give me everybody's names, separated by a comma. \n")
names = names_string.split(", ")

person_to_pay = names[random.randint(0, len(names) - 1)]
print(f"{person_to_pay} is going to buy the meal today!")
```

```py
# Give me everybody's names, separated by a comma.
# James, John, Luke, Mary, Ashley, Dan
# Ashley is going to buy the meal today!
```

```py
import random

names_string = input("Give me everybody's names, separated by a comma. \n")
names = names_string.split(", ")

person_to_pay = random.choice(names)
print(f"{person_to_pay} is going to buy the meal today!")
```

```py
# Give me everybody's names, separated by a comma.
# James, John, Luke, Mary, Ashley, Dan
# Ashley is going to buy the meal today!
```

Nested Lists:

```py
fruits = ["Strawberries", "Nectarines", "Apples", "Grapes", "Peaches", "Cherries", "Pears"]
vegetables = ["Spinach", "Kale", "Tomatoes", "Celery", "Potatoes"]

dirty_dozen = [fruits, vegetables]

print(dirty_dozen)

```

```py
# [['Strawberries', 'Nectarines', 'Apples', 'Grapes', 'Peaches', 'Cherries', 'Pears'], ['Spinach', 'Kale', 'Tomatoes', 'Celery', 'Potatoes']]
```

```py
row1 = ["⬜️","️⬜️","️⬜️"]
row2 = ["⬜️","⬜️","️⬜️"]
row3 = ["⬜️️","⬜️️","⬜️️"]
map = [row1, row2, row3]

print(f"{row1}\n{row2}\n{row3}")

position = input("Where do you want to put the treasure? \n")

column_to_index = int(position[0]) - 1
row_to_index = int(position[1]) - 1
map[row_to_index][column_to_index] = "X"

print(f"{row1}\n{row2}\n{row3}")

```

```py
# ['⬜️', '️⬜️', '️⬜️']
# ['⬜️', '⬜️', '️⬜️']
# ['⬜️️', '⬜️️', '⬜️️']
# Where do you want to put the treasure?
# 23
# ['⬜️', '️⬜️', '️⬜️']
# ['⬜️', '⬜️', '️⬜️']
# ['⬜️️', 'X', '⬜️️']
```

RPS Game:

```py
import random

rock = '''
    _______
---'   ____)
      (_____)
      (_____)
      (____)
---.__(___)
'''

paper = '''
    _______
---'   ____)____
          ______)
          _______)
         _______)
---.__________)
'''

scissors = '''
    _______
---'   ____)____
          ______)
       __________)
      (____)
---.__(___)
'''

#Write your code below this line 👇
choice = input(
    "What do you choose? Type 0 for Rock, 1 for Paper or 2 for Scissors? \n")

print('You chose:')

player_choice = None

if choice == '0':
    print(rock)
    player_choice = "rock"
elif choice == '1':
    print(paper)
    player_choice = "paper"
elif choice == '2':
    print(scissors)
    player_choice = "scissors"
else:
    print('Wrong Input. Try Again!')

print('Computer chose:')

computer_choice = random.choice(["rock", "paper", "scissors"])

if computer_choice == "rock":
    print(rock)
elif computer_choice == "paper":
    print(paper)
elif computer_choice == "scissors":
    print(scissors)

if (player_choice == "rock" and computer_choice == "paper") or (
        player_choice == "paper"
        and computer_choice == "scissors") or (player_choice == "scissors"
                                               and computer_choice == "rock"):
    print('You Lose.')
elif (player_choice == "rock" and computer_choice == "scissors") or (
        player_choice == "paper"
        and computer_choice == "rock") or (player_choice == "scissors"
                                           and computer_choice == "paper"):
    print('You Won! Congrats!')
elif player_choice == None:
    print("")
else:
    print("It's a Tie!")

```

```py
# What do you choose? Type 0 for Rock, 1 for Paper or 2 for Scissors?
# 1
# You chose:

#     _______
# ---'   ____)____
#           ______)
#           _______)
#          _______)
# ---.__________)

# Computer chose:

#     _______
# ---'   ____)
#       (_____)
#       (_____)
#       (____)
# ---.__(___)

# You Won! Congrats!
```

```py
import random

rock = '''
    _______
---'   ____)
      (_____)
      (_____)
      (____)
---.__(___)
'''

paper = '''
    _______
---'   ____)____
          ______)
          _______)
         _______)
---.__________)
'''

scissors = '''
    _______
---'   ____)____
          ______)
       __________)
      (____)
---.__(___)
'''

game_images = [rock, paper, scissors]

user_choice = int(input("What do you choose? Type 0 for Rock, 1 for Paper or 2 for Scissors.\n"))

if user_choice >= 3 or user_choice < 0:
  print("You typed an invalid number, you lose!")
else:
  print(game_images[user_choice])
  computer_choice = random.randint(0, 2)
  print("Computer chose:")
  print(game_images[computer_choice])

  if user_choice == 0 and computer_choice == 2:
    print("You win!")
  elif computer_choice == 0 and user_choice == 2:
    print("You lose")
  elif computer_choice > user_choice:
    print("You lose")
  elif user_choice > computer_choice:
    print("You win!")
  elif computer_choice == user_choice:
    print("It's a draw")

```

</details>

<details>
  <summary>8. Python For Loops </summary>

Looping through Lists:

```py
fruits = ["Apple", "Peach", "Pear"]
for fruit in fruits:
	print(fruit)
```

```py
# Apple
# Peach
# Pear
```

```py
student_scores = input("Input a list of student scores ").split()
for n in range(0, len(student_scores)):
  student_scores[n] = int(student_scores[n])
print(student_scores)

highest_score=0
for i in student_scores:
    if i > highest_score:
        highest_score = i

print(f"The highest score in the class is: {highest_score}")
```

```py
# Input a list of student scores 10 20 30 40 70 80 40 30
# [10, 20, 30, 40, 70, 80, 40, 30]
# The highest score in the class is: 80
```

```py
total = 0

for i in range(0,101,2):
    total += i
print(total)
```

```py
# 2550
```

```py
total2 = 0

for number in range(1, 101):
  if number % 2 == 0:
    total2 += number
print(total2)
```

```py
# 2550
```

```py
for number in range(1,101):
    if number % 3 == 0 and number % 5 == 0:
        print("FizzBuzz")
    elif number % 3 == 0:
        print("Fizz")
    elif number % 5 == 0:
        print("Buzz")
    else:
        print(number)
```

```py
# 1
# 2
# Fizz
# 4
# Buzz
# Fizz
# 7
```

```py
#Password Generator Project
import random

letters = [
    'a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o',
    'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z', 'A', 'B', 'C', 'D',
    'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S',
    'T', 'U', 'V', 'W', 'X', 'Y', 'Z'
]
numbers = ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9']
symbols = ['!', '#', '$', '%', '&', '(', ')', '*', '+']

print("Welcome to the PyPassword Generator!")
nr_letters = int(input("How many letters would you like in your password?\n"))
nr_symbols = int(input(f"How many symbols would you like?\n"))
nr_numbers = int(input(f"How many numbers would you like?\n"))

#Eazy Level - Order not randomised:
#e.g. 4 letter, 2 symbol, 2 number = JduE&!91
password = ""
for i in range(nr_letters):
    password += random.choice(letters)
for j in range(nr_symbols):
    password += random.choice(symbols)
for k in range(nr_numbers):
    password += random.choice(numbers)

print(password)

#Hard Level - Order of characters randomised:
#e.g. 4 letter, 2 symbol, 2 number = g^2jk8&P
password2 = ""

while nr_letters > 0 or nr_symbols > 0 or nr_numbers > 0:
    choice = random.randint(0, 2)
    if choice == 0 and nr_letters > 0:
        password2 += random.choice(letters)
        nr_letters -= 1
    elif choice == 1 and nr_symbols > 0:
        password2 += random.choice(symbols)
        nr_symbols -= 1
    elif choice == 2 and nr_numbers > 0:
        password2 += random.choice(numbers)
        nr_numbers -= 1

print(password2)

```

```py
# Welcome to the PyPassword Generator!
# How many letters would you like in your password?
# 3
# How many symbols would you like?
# 3
# How many numbers would you like?
# 3
# qJk##*130
# (z96P%T6)
```

```py
#Hard Level - Order of characters randomised:
#e.g. 4 letter, 2 symbol, 2 number = g^2jk8&P
password2 = []

for i in range(nr_letters):
    password2.append(random.choice(letters))
for j in range(nr_symbols):
    password2 += random.choice(symbols)
for k in range(nr_numbers):
    password2 += random.choice(numbers)

random.shuffle(password2)

mypassword = ""
for char in password2:
    mypassword += char
print(mypassword)
```

```py
# Welcome to the PyPassword Generator!
# How many letters would you like in your password?
# 3
# How many symbols would you like?
# 3
# How many numbers would you like?
# 3
# jgK*+*220
# e3g6*((m9
```

</details>

<details>
  <summary>9. Python Functions </summary>

```py
def my_function():
  print("Hello")
  print("Bye")
my_function ()
```

```py
# Hello
# Bye
```

</details>

<details>
  <summary>10. Python While Loops </summary>

```py
def turn_right():
    turn_left()
    turn_left()
    turn_left()

def jump():
    turn_left()
    move()
    turn_right()
    move()
    turn_right()
    move()
    turn_left()

step = 0
while step < 6:
    move()
    jump()
    step += 1
```

```py
def turn_right():
    turn_left()
    turn_left()
    turn_left()

def jump():
    turn_left()
    move()
    turn_right()
    move()
    turn_right()
    move()
    turn_left()

while not at_goal():
    if front_is_clear():
        move()
    elif wall_in_front():
        jump()
```

</details>

<details>
  <summary>11. Hangman </summary>

```py
#Step 1
#TODO-1 - Randomly choose a word from the word_list and assign it to a variable called chosen_word.
#TODO-2 - Ask the user to guess a letter and assign their answer to a variable called guess. Make guess lowercase.
#TODO-3 - Check if the letter the user guessed (guess) is one of the letters in the chosen_word.

import random

word_list = ["aardvark", "baboon", "camel"]

chosen_word = random.choice(word_list)

guess = input("Guess a letter: ").lower()

for letter in chosen_word:
    print("Right" if letter == guess else "Wrong")
```

```py
# Guess a letter: a
# Right
# Right
# Wrong
# Wrong
# Wrong
# Right
# Wrong
# Wrong
```

```py
#Step 2

import random

word_list = ["aardvark", "baboon", "camel"]
chosen_word = random.choice(word_list)

#Testing code
print(f'Pssst, the solution is {chosen_word}.')

#TODO-1: - Create an empty List called display.
#For each letter in the chosen_word, add a "_" to 'display'.
#So if the chosen_word was "apple", display should be ["_", "_", "_", "_", "_"] with 5 "_" representing each letter to guess.

display = []
for _ in range(len(chosen_word)):
    display += "_"
print(display)

guess = input("Guess a letter: ").lower()

#TODO-2: - Loop through each position in the chosen_word;
#If the letter at that position matches 'guess' then reveal that letter in the display at that position.
#e.g. If the user guessed "p" and the chosen word was "apple", then display should be ["_", "p", "p", "_", "_"].

for index, letter in enumerate(chosen_word):
	if letter == guess:
			display[index] = letter

#TODO-3: - Print 'display' and you should see the guessed letter in the correct position and every other letter replace with "_".
#Hint - Don't worry about getting the user to guess the next letter. We'll tackle that in step 3.
print(display)

```

```py
#TODO-2: - Loop through each position in the chosen_word;
#If the letter at that position matches 'guess' then reveal that letter in the display at that position.
#e.g. If the user guessed "p" and the chosen word was "apple", then display should be ["_", "p", "p", "_", "_"].

word_length = len(chosen_word)
for position in range(word_length):
  letter = chosen_word [position]
  if letter == guess:
    display[position] = letter
```

```py
# Pssst, the solution is aardvark.
# ['_', '_', '_', '_', '_', '_', '_', '_']
# Guess a letter: a
# ['a', 'a', '_', '_', '_', 'a', '_', '_']
```

```py
#Step 3

import random

word_list = ["aardvark", "baboon", "camel"]
chosen_word = random.choice(word_list)
word_length = len(chosen_word)

#Testing code
print(f'Pssst, the solution is {chosen_word}.')

#Create blanks
display = []
for _ in range(word_length):
    display += "_"

#TODO-1: - Use a while loop to let the user guess again. The loop should only stop once the user has guessed all the letters in the chosen_word and 'display' has no more blanks ("_"). Then you can tell the user they've won.

while "_" in display:
    guess = input("Guess a letter: ").lower()
    #Check guessed letter
    for position in range(word_length):
        letter = chosen_word[position]
        print(
            f"Current position: {position}\n Current letter: {letter}\n Guessed letter: {guess}"
        )
        if letter == guess:
            display[position] = letter
    print(display)

```

```py
#TODO-1: - Use a while loop to let the user guess again. The loop should only stop once the user has guessed all the letters in the chosen_word and 'display' has no more blanks ("_"). Then you can tell the user they've won.

while not end_of_game:
  guess = input("Guess a letter: ").lower()

  #Check_guessed letter
  for position in range(word_length):
    letter = chosen_word[position]
    print(
            f"Current position: {position}\n Current letter: {letter}\n Guessed letter: {guess}"
        )
    if letter == guess:
      display[position] = letter

  print (display)

  if "_" not in display:
    end_of_game = True
    print("You win.")
```

```py
# ['b', 'a', 'b', 'o', 'o', '_']
# Guess a letter: n
# Current position: 0
#  Current letter: b
#  Guessed letter: n
# Current position: 1
#  Current letter: a
#  Guessed letter: n
# Current position: 2
#  Current letter: b
#  Guessed letter: n
# Current position: 3
#  Current letter: o
#  Guessed letter: n
# Current position: 4
#  Current letter: o
#  Guessed letter: n
# Current position: 5
#  Current letter: n
#  Guessed letter: n
# ['b', 'a', 'b', 'o', 'o', 'n']
```

```py
#Step 4

import random

stages = [
    '''
  +---+
  |   |
  O   |
 /|\  |
 / \  |
      |
=========
''', '''
  +---+
  |   |
  O   |
 /|\  |
 /    |
      |
=========
''', '''
  +---+
  |   |
  O   |
 /|\  |
      |
      |
=========
''', '''
  +---+
  |   |
  O   |
 /|   |
      |
      |
=========''', '''
  +---+
  |   |
  O   |
  |   |
      |
      |
=========
''', '''
  +---+
  |   |
  O   |
      |
      |
      |
=========
''', '''
  +---+
  |   |
      |
      |
      |
      |
=========
'''
]

end_of_game = False
word_list = ["ardvark", "baboon", "camel"]
chosen_word = random.choice(word_list)
word_length = len(chosen_word)

#TODO-1: - Create a variable called 'lives' to keep track of the number of lives left.
#Set 'lives' to equal 6.

lives = 6

#Testing code
print(f'Pssst, the solution is {chosen_word}.')

#Create blanks
display = []
for _ in range(word_length):
    display += "_"

while not end_of_game:
    guess = input("Guess a letter: ").lower()
    found = False
    #Check guessed letter
    for position in range(word_length):
        letter = chosen_word[position]
        # print(f"Current position: {position}\n Current letter: {letter}\n Guessed letter: {guess}")
        if letter == guess:
            display[position] = letter
            found = True

    if found == False:
        lives -= 1
    else:
        found = False
    if lives == 0:
        print("You lose.")
        print(stages[lives])
        break

    #TODO-2: - If guess is not a letter in the chosen_word,
    #Then reduce 'lives' by 1.
    #If lives goes down to 0 then the game should stop and it should print "You lose."

    #Join all the elements in the list and turn it into a String.
    print(f"{' '.join(display)}")

    #Check if user has got all letters.
    if "_" not in display:
        end_of_game = True
        print("You win.")

#TODO-3: - print the ASCII art from 'stages' that corresponds to the current number of 'lives' the user has remaining.
    print(stages[lives])

```

```py
#Step 4

import random

stages = ['''
  +---+
  |   |
  O   |
 /|\  |
 / \  |
      |
=========
''', '''
  +---+
  |   |
  O   |
 /|\  |
 /    |
      |
=========
''', '''
  +---+
  |   |
  O   |
 /|\  |
      |
      |
=========
''', '''
  +---+
  |   |
  O   |
 /|   |
      |
      |
=========''', '''
  +---+
  |   |
  O   |
  |   |
      |
      |
=========
''', '''
  +---+
  |   |
  O   |
      |
      |
      |
=========
''', '''
  +---+
  |   |
      |
      |
      |
      |
=========
''']

end_of_game = False
word_list = ["ardvark", "baboon", "camel"]
chosen_word = random.choice(word_list)
word_length = len(chosen_word)

#TODO-1: - Create a variable called 'lives' to keep track of the number of lives left.
#Set 'lives' to equal 6.
lives = 6

#Testing code
print(f'Pssst, the solution is {chosen_word}.')

#Create blanks
display = []
for _ in range(word_length):
    display += "_"

while not end_of_game:
    guess = input("Guess a letter: ").lower()

    #Check guessed letter
    for position in range(word_length):
        letter = chosen_word[position]
       # print(f"Current position: {position}\n Current letter: {letter}\n Guessed letter: {guess}")
        if letter == guess:
            display[position] = letter

    #TODO-2: - If guess is not a letter in the chosen_word,
    #Then reduce 'lives' by 1.
    #If lives goes down to 0 then the game should stop and it should print "You lose."
    if guess not in chosen_word:
        lives -= 1
        if lives == 0:
            end_of_game = True
            print("You lose.")

    #Join all the elements in the list and turn it into a String.
    print(f"{' '.join(display)}")

    #Check if user has got all letters.
    if "_" not in display:
        end_of_game = True
        print("You win.")

    #TODO-3: - print the ASCII art from 'stages' that corresponds to the current number of 'lives' the user has remaining.
    print(stages[lives])
```

```py
# Pssst, the solution is baboon.
# Guess a letter: s
# _ _ _ _ _ _

#   +---+
#   |   |
#   O   |
#       |
#       |
#       |
# =========

# Guess a letter: s
# _ _ _ _ _ _

#   +---+
#   |   |
#   O   |
#   |   |
#       |
#       |
# =========

# Guess a letter: s
# _ _ _ _ _ _

#   +---+
#   |   |
#   O   |
#  /|   |
#       |
#       |
# =========
# Guess a letter: s
# _ _ _ _ _ _

#   +---+
#   |   |
#   O   |
#  /|\  |
#       |
#       |
# =========

# Guess a letter: s
# _ _ _ _ _ _

#   +---+
#   |   |
#   O   |
#  /|\  |
#  /    |
#       |
# =========

# Guess a letter: s
# You lose.

#   +---+
#   |   |
#   O   |
#  /|\  |
#  / \  |
#       |
# =========
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
