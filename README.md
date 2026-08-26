# ECE-2112-PA-1
### **Made by: Evan James G. Paciencia|2ECE-C**
This repository contains Programming Assignment 1 for the course "Advanced Computer Programming" of S.Y. 2026-2027. This assignment covers three Python problems about Module 1 - Base Computing with Python.

## 1. WORD ROTATION PROBLEM
Create a function that accepts a non-empty string and moves the first character of the string to the end while keeping all remaining characters in their original order and the capitalization of every character.
The following functions and methods were used:<br>
- ` ("")[index of first element: index of last element: increment] ` - Slices the character/s at the starting index until the end of the string and the following based on the increment. <br>
<br> Example: ("World")[0:1:1] -> 'w'<br><br>
- ` len() ` - Gets the length of the string.<br>
<br> Example: len("world") -> 5<br>
<br>These built-in functions and methods were combined to create a single defined function that moves the first character of the string to the end while preserving all other characters and their capitalization.
```
def rotate_word(word):
    l=int(len(word))
    return(word[1:l:1]+word[0:l:l])

print(rotate_word(input("enter a word")))
```
## 2. USERNAME BUILDER PROBLEM
Create a function that accepts two strings, the first and last name. While converting all letters to lowercase, remove all spaces from the first and last names, then join the processed first and last names with a period (.).
<br> The following functions and methods were used:<br><br>
- ` "".lower() ` - Changes all uppercase characters to their lowercase versions.<br>
  <br> Example: "My Name Is".lower() -> 'my name is'<br><br>
- ` "".replace(a, b)` - Replaces every element/character in a using b.<br>
  <br> Example: "my name is".replace(" ","") -> 'mynameis'<br>
<br>These built-in functions and methods were combined to create a function that accepts two strings, first and last name. While converting all letters to lowercase, remove all spaces from the first and last names, then join the processed first and last names with a period (.).
```
def make_username(first_name,last_name):
    return((first_name.lower().replace(" ", "")+"."+last_name.lower().replace(" ", "")))

print(make_username(input("Enter first name"), input("Enter last name")))
```
## 3. BOOKEND SWAP PROBLEM
