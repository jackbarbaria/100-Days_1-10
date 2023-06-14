# Day 1 - Working with Variables in Python

## Band Name Generator Project

Please check out my Band Name Generator project, using what I learned on Day 1. </br>
[Band Name Generator](https://replit.com/@JackBarbaria/Day1BandNameGenerator?v=1)

```python
print("Welcome to Jazzy Jack's Band Name Generator!!\nHave fun and don't get too excited!!")
user_city = input("What city or town did you grow up in? ")
pet_name = input("What is the name of a pet that you like? ")
print("Here is the name of your band: \n" + user_city + " " + pet_name)
```
Day 1 was all about learning how to use the print, len, and input functions. I also learned how to manipulate strings, and how to create variables in Python. 

# Day 2 - Data Types and Manipulating Strings

## Tip Calculator Project

Check out the Tip Calculator project I created using the concepts I learned during Day 2. I learned about different data types and how to convert between them. I also learned how to manipulate strings and numbers. 

[Tip Calculator](https://replit.com/@JackBarbaria/Day-2-Tip-Calculator?v=1)

```python
print("Welcome to Jazzy Jack's tip calculator.\nFor those of us who are math challenged, this is the tool for you!")
total_bill = input("What is the total bill? $")
tip_percentage = input("What percentage tip would you like to give? 12, 15, 20, etc? ")
no_people = input("How many people to split the bill? ")
tipsy = "1." + tip_percentage
tipsy = float(tipsy)
split = (float(total_bill) * tipsy)/float(no_people)
print(f"Each person should pay: ${split:.2f}")
```


# Day 3 - Control Flow and Logical Operators
## Choose Your Own Adventure
Check out my choose your own adventure game written using what I learned during Day 3!

[Treasure Island - Choose Your Own Adventure](https://replit.com/@JackBarbaria/Day-3-treasure-island?v=1)

```python
print('''
*******************************************************************************
          |                   |                  |                     |
 _________|________________.=""_;=.______________|_____________________|_______
|                   |  ,-"_,=""     `"=.|                  |
|___________________|__"=._o`"-._        `"=.______________|___________________
          |                `"=._o`"=._      _`"=._                     |
 _________|_____________________:=._o "=._."_.-="'"=.__________________|_______
|                   |    __.--" , ; `"=._o." ,-"""-._ ".   |
|___________________|_._"  ,. .` ` `` ,  `"-._"-._   ". '__|___________________
          |           |o`"=._` , "` `; .". ,  "-._"-._; ;              |
 _________|___________| ;`-.o`"=._; ." ` '`."\` . "-._ /_______________|_______
|                   | |o;    `"-.o`"=._``  '` " ,__.--o;   |
|___________________|_| ;     (#) `-.o `"=.`_.--"_o.-; ;___|___________________
____/______/______/___|o;._    "      `".o|o_.--"    ;o;____/______/______/____
/______/______/______/_"=._o--._        ; | ;        ; ;/______/______/______/_
____/______/______/______/__"=._o--._   ;o|o;     _._;o;____/______/______/____
/______/______/______/______/____"=._o._; | ;_.--"o.--"_/______/______/______/_
____/______/______/______/______/_____"=.o|o_.--""___/______/______/______/____
/______/______/______/______/______/______/______/______/______/______/_____ /
*******************************************************************************
''')
print("Welcome to Treasure Island.")
print("Your mission is to find the treasure.\n\n") 

#first choice "The Road"
print("Before you is a cobblestone road. To the left the road looks rough and worn and leads towards the sea. To the right the road looks less traveled, and leads towards a dark wooded area.\n\n")
the_road = input("Do you go left or right? L or R? ")
if the_road == "R":
  print('You travel along the road into the dark woods. The ominous screech of an owl startles you as you trip over a loose cobblestone. "Hoot... hoot" is the last thing you hear as you lose conciousness from the hard impact of the ground.\n\nGame over.')

#second choice "The Beach"
else:
  print("You travel along the road towards the sea. The sound of the surf sooths your ears and the smell of the salt water brightens yor spirits. As you reach the shore, you can clearly see an island not far off, maybe 300-400 yards away. It doesn't seem too far away to swim. Though it may be better to wait for a boat\n\n")
  the_beach = input("Do you swim to the island or wait for a boat? Type 'S' for swim or 'W' for wait: ")
  if the_beach == "S":
    print("You jump into the water and start swimming towards the island. After just a few strokes in, you feel a sharp pain. A jellyfish has stung you in the back and you can't feel your legs. As the waves push you back to the shore, all you can do is fight to keep your head above the water.\n\nGame over.")

  #third choice "The Door"
  else:
    print('You wait about 5 minutes and before long an old man in a small dingy rows up to you and offers to take you to the island. "Ah! Another treasure hunter, I see," the old man rasps. "I take suckers like you across and not a one has returned unscathed. But since you insist..."\n\n')
    print("Before long, you have reached the island. The old man bids you adieu. On the island you see one lonely building with three doors. Red, Yellow, and Blue.") 
    the_door = input("Which door will you open? Type 'R' for Red, 'Y' for Yellow, and 'B' for Blue: ")
    if the_door == "R" or the_door == "B":
      print("You open the door and an irrestible force pulls you into it's gaping maw. You see nothing but darkness.\n\nGame over.")

    #Winner!!
    else:
      print("\n\nThe door opens smoothly and before you is an open chest, overflowing with gold and jewels. Congratulations! You have found the treasure and won the game!!")
```

# Day 4 - Randomization and Python Lists
## Rock Paper Scissors
The Day 4 challenge. Who will win... you or the computer, in this no holds barred, winner takes all, rock/paper/scissors game?!

[Rock, Paper, Scissors Game!](https://replit.com/@JackBarbaria/Day-4-rock-paper-scissors?v=1)

```python
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
import random

pic = [rock, paper, scissors]

players_choice = int(input("What do you choose? Type 1 for Rock, 2 for Paper, or 3 for Scissors.\n"))-1

if players_choice != 0 and players_choice != 1 and players_choice != 2:
  print("That is an invalid choice. You've lost before you even started.")
else:
  print(pic[players_choice])

# Computer choses randomly:  
  print("Computer chose:")
  computers_choice = random.randint(0, 2)
  print(pic[computers_choice])

# player chose rock
  if players_choice == 0 and computers_choice == 0:
    print("You are equally matched as this challenge ends in a draw.")
  elif players_choice == 0 and computers_choice == 1:
    print("Hang you head in shame as you have been defeated by the computer!")
  elif players_choice == 0 and computers_choice == 2:
    print("Victory is yours!!!")

# player chose paper
  elif players_choice == 1 and computers_choice == 0:
    print("You have chosen wisely and crushed your opponent!")
  elif players_choice == 1 and computers_choice == 1:
    print("Alas, it is a stalement... this time.")
  elif players_choice == 1 and computers_choice == 2:
    print("You have chosen poorly and have brought dishonor to your family.")

# player chose scissors
  elif players_choice == 2 and computers_choice == 0:
    print("You've lost. Walk away tall.")
  elif players_choice == 2 and computers_choice == 1:
    print("Winner, winner, chicken dinner!!")
  elif players_choice == 2 and computers_choice == 2:
    print("It's a tie. Can you believe it?")
```
