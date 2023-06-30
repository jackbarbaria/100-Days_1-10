# 100 Days of Code: Days 1 - 10
I've been learning Python through the [100 Days of Code: The Complete Python Pro Bootcamp for 2023](https://www.udemy.com/course/100-days-of-code/) course on Udemy. This course by [Dr. Angela Yu](https://www.udemy.com/user/4b4368a3-b5c8-4529-aa65-2056ec31f37e/) contains a daily collection of video lessons that include smaller coding challenges, where concepts are introduced. At the end of each day, you are challenged with a more difficult Final Project where you bring together all you learned in previous the lessons. I am documenting here the code I've written for each of these daily Final Projects.

## Day 1 - Working with Variables in Python

### Band Name Generator Project

Please check out my Band Name Generator project, using what I learned on Day 1. </br>
[Band Name Generator](https://replit.com/@JackBarbaria/Day1BandNameGenerator?v=1)

```python
print("Welcome to Jazzy Jack's Band Name Generator!!\nHave fun and don't get too excited!!")
user_city = input("What city or town did you grow up in? ")
pet_name = input("What is the name of a pet that you like? ")
print("Here is the name of your band: \n" + user_city + " " + pet_name)
```
Day 1 was all about learning how to use the print, len, and input functions. I also learned how to manipulate strings, and how to create variables in Python. 

## Day 2 - Data Types and Manipulating Strings

### Tip Calculator Project

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


## Day 3 - Control Flow and Logical Operators
### Choose Your Own Adventure
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

## Day 4 - Randomization and Python Lists
### Rock Paper Scissors
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


## Day 5 - Python Loops, Range, and Code Blocks
### Password Generator
The Day 5 final challenge stretched me to the limit. It was fun to watch the instructor's solution after I had written my version and see how Dr. Yu solved this challenge in about half the lines of code that I had written. I'm still excited that I got there at the end. 

[Password Generator](https://replit.com/@JackBarbaria/Day-5-password-generator?v=1)

```python
#Password Generator Project
import random
letters = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z', 'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z']
numbers = ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9']
symbols = ['!', '#', '$', '%', '&', '(', ')', '*', '+']

print("Welcome to the PyPassword Generator!\n")
nr_letters= int(input("How many letters would you like in your password?\n")) 
nr_symbols = int(input(f"How many symbols would you like?\n"))
nr_numbers = int(input(f"How many numbers would you like?\n"))

# generating random letters
let_result = ''
for letter in range(0, (nr_letters)):
  L = random.randint(0, 41)
  let_result += letters[L]

# generating random number
num_result = ''
for number in range(0, (nr_numbers)):
  X = random.randint(0, 9)
  num_result += numbers[X]

# generating random symbols
sym_result = ''
for number in range(0, (nr_symbols)):
  S = random.randint(0, 8)
  sym_result += symbols[S]

# combining the results into one string
combined = let_result + num_result + sym_result

num_of_char = len(combined)

# converting the string to a list
rando_list = []
for app in range(0, (num_of_char)):
  rando_list.append(combined[app])

# randomizing the order of the list
random.shuffle(rando_list)

# converting the shuffled list back to a string
rando_password = ''
for app2 in range(0, (num_of_char)):
  rando_password += rando_list[app2]

print(f"\nYour password is {rando_password}")
```


## Day 6 - Python Functions
### Reeborg's Maze 
The Day 6 lesson focused on how to define your own functions. It also introduced the **while** loop and highlighted the differences between **while** and **for** loops. Today's challenges intruduced me to [Reeborg's World](https://reeborg.ca/index_en.html). At Reeborg's World you use Python to automate the actions of a robot in order to complete a task. In the final challenge of the day, Reeborg is placed in a randomly generated maze, facing in a random direction, and the goal is to guide Reeborg out of the maze. This was a difficult challenge for me, as there were certain conditions that would occur that would cause Reeborg to walk in a circle in an infinite loop. After I slept on on it, I realized I could track the number of turns Reeborg makes and force him to do something different, avoiding the loop.

<br />
<img src="https://i.imgur.com/Ri6DX4v.jpg" height="80%" width="80%" alt="Reeborg's Maze"/>
<br />

## Day 7 - Hangman

Day 7 was entirely devoted to making a **hangman** game. Check out my version of the game here: [Hangman](https://replit.com/@JackBarbaria/Day-7-Hangman-Project?v=1).

<br />
<img src="https://i.imgur.com/wpHw6n1.png" height="40%" width="40%" alt="Hangman"/>
<br />

Today's lesson encouraged me to create a flowchart to break down the game of **hangman** into its indivdual components. This flowchart would become the blueprint for designing the game. Then with the help of the Day 7 challenges, writing the game was broken down into 5 steps: 
1. Picking a word and checking the user's answer.
2. Display blanks for each letter of the word and replacing the blanks with guesses.
3. Checking if the player has won.
4. Keeping track of the player's lives.
5. Improving the user's experience.

I added a couple features that were not in the original guide. I wanted to add some sort of input validation, as I noticed the game would break if I accidently typed two letters for my guess. So, I created a list that included all the capital and lower case letters of the alphabet and the game now checks to see if the input matches this list. If the player's accidently types in "aa" it will not match the validation list and the player will be asked to try again. I also had the program, track previous guesses so if the player picked the same letter twice, they would be asked to chose another letter.

The provided word list is challenging as it only provides the player with a single word to guess. I find it's easier to play **hangman** if you can pick a category (like Movies, or Phrases) and then have a puzzle with multiple words. While I was able to expirement with a list of movie titles, I was having trouble altering the program to allowing the player to choose from multiple puzzle categories. I'll come back this later, after I have learned more Python.

## Day 8 - Function Parameters
### Caesar Cypher Project

Today, I learned how to add parameters and how to pass arguments into functions. This helped me complete the Day 8 challenge to create a program that allows the user to encode and decode messages using a Caesar, or shift cypher.

[Caesar Cypher Program](https://replit.com/@JackBarbaria/Day-8-Caesar-Cypher?v=1)

```python
alphabet = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z']

def caesar(code_text, shift_amount, cypher_direction):
  scrambled_text = ""
  if cypher_direction == "decode":
    shift_amount *= -1
  for letter in code_text:
    if letter not in alphabet:
      new_letter = letter
    else:
      original_index = alphabet.index(letter)
      new_index = original_index + shift_amount
      if new_index < 0:
        new_index += 26
      elif new_index > 25:
        new_index -= 26 
      new_letter = alphabet[new_index]
    scrambled_text += new_letter
  print(f"The {cypher_direction}d text is {scrambled_text}")

import art
print(art.logo) 

Start = True
while Start:
  direction = input("Type 'encode' to encrypt, type 'decode' to decrypt:\n")
  text = input("Type your message:\n").lower()
  shift = (int(input("Type the shift number:\n"))) % 26

  caesar(code_text=text, shift_amount=shift, cypher_direction=direction)
  go_again = input('Type "yes" if you want to go again. Otherwise type "no".\n')
  if go_again == "no":
    Start = False

print("Goodbye")
```

## Day 9 - Dictionaries and Nesting
### Secret Auction Project

Day 9 was focused on Dictionaries and how to nest dictionaries within lists and lists within dictionaries, and even dictionaries within dictionaries. It was wild!! I followed along and built a Secret or Blind Auction program. It always fascinates me to see the differences in the code in my version of program versus the solution presented by the instructor. 

Check out my [Secret Auction Program](https://replit.com/@JackBarbaria/Day-9-Blind-Auction?v=1)

```python
from replit import clear
import art

bid_list = []
def add_bid_info(new_name, new_amount):
  new_bidder = {}
  new_bidder["name"] = new_name
  new_bidder["amount"] = new_amount
  bid_list.append(new_bidder)

more = True
while more == True:
  print(art.logo)
  print("Welcome to the secret auction program.")
  bid_name = input("What is your name?: ")
  bid_amount = int(input("What's your bid?: $"))

  add_bid_info(new_name=bid_name, new_amount=bid_amount)
  
  more_bidders = input("\nAre there any other bidders? Type 'yes' or 'no'.\n")
  if more_bidders == "no":
    more = False
  else:
    clear()

highbidder = ""
highbid = 0
for bid in bid_list:
  dolla = bid["amount"]
  namo = bid["name"]
  if dolla > highbid:
    highbid = dolla
    highbidder = namo

clear()
print(art.celebration)
print(f"The winner is {highbidder} with a bid of ${highbid}")
```
