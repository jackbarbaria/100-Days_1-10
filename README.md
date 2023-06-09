# Day 1 - Working with Variables in Python

## print() function
The function is declared like this:
`print('what to print')` 
```python	
print("Hello World!")
```
**Output:**
```
Hello world!
```

The quoted text is a **string**. Single or double quotes can be used.
## String Manipulation

New lines can be created with a **/n**).

```python	
print("Hello World!\nHello World")
```

**Output:**
```
Hello world!
Hello world!
```

</br>

String Concatenation is done with the "**+**" sign.
```python	
print("Hello" + "Jack")
```
**Output:**
```
HelloJack
```
## input() function
The `input()` function allows user input. 
Syntax: **input(*prompt*)**

```python	
print("Hello " + input("What is your name? ") + "!")
```
**Output:**
```
What is your name? Jack
Hello Jack!
```

## len() function
The len() function returns the number of items in an object.

```python
print(len("Jack"))
```
**Output:**
```
4
```
The output is 4 because the length of the string within the **len** function is four characters long.

## Python Variables
**Variables** are containers for storing data values. A variable is created the moment you first assign a value to it. 
```python
name = input("What is your name? ")
print(name)
```
In the above example the input typed by the user is stored in the "**name**" variable. Then the stored variable is referenced by the **print()** function.

**Output:**
```
What is your name? Jack
Jack
```

## Day 1 - Band Name Generator Project
Please check out my Band Name Generator project, using what I learned on Day 1. </br>
[Band Name Generator](https://replit.com/@JackBarbaria/Day1BandNameGenerator?v=1)
