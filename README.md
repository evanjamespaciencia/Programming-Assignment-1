# ECE-2112-PA-1
### **Made by: Evan James G. Paciencia|2ECE-C**
This repository contains Programming Assignment 1 for the course "Advanced Computer Programming" of S.Y. 2026-2027. This assignment covers three Python problems about Module 1 - Base Computing with Python.

## 1. WORD ROTATION PROBLEM
Create a function that accepts a non-empty string and moves the first character of the string to the end while keeping all remaining characters in their original order and the capitalization of every character.
The following functions and methods were used:<br>
- ` ("")[index of first element: index of last element: increment] ` - Slices the character/s at the starting index until the end of the string and the following based on the increment. <br>
<br> Example: ("World")[0:1:1] -> 'w'<br><br>
<br>These built-in functions and methods were combined to create a single defined function that moves the first character of the string to the end while preserving all other characters and their capitalization.
```
def rotate_word(word):
    return(word[1:]+word[:1])

print(rotate_word("python"))
print(rotate_word("logic"))
print(rotate_word("Code"))
print(rotate_word("A"))
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

print(make_username("Ada", "Lovelace"))
print(make_username("Alan", "Turing"))
print(make_username("Ana Maria", "De Leon"))
```
## 3. BOOKEND SWAP PROBLEM
Create a function that accepts a list containing at least two elements. Unpack the list into 3 elements:<br>
- first – the first element.<br>
- middle – a list containing everything between the first and last elements.<br>
- last – the last element<br><br>
<br>Swap the first and last elements of the list while keeping the middle elements in order and leaving the original list unchanged. <br>
There were no functions used in this problem.<br>
<br>These built-in functions and methods were combined to create a function that accepts a list containing at least two elements. Unpack the list into 3 elements: first, the first element, a list containing everything between the first and last elements, and last, the last element
  
<br> Swap the first and last elements of the list while keeping the middle elements in order and leaving the original list unchanged. <br>
The following functions and methods were used:<br>
```
def swap_bookends(items):
    first, *middle, last = items
    return last, *middle, first
print(swap_bookends([1,2,3,4,5,6]))
print(swap_bookends(["red", "green", "blue"]))
print(swap_bookends([8,3]))
```
## Edit Log/History
August 8, 2026 -> Edited examples list for problem 2
