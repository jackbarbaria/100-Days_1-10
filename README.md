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
