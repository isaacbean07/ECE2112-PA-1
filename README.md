# ECE2112-PA-1
Isaac Benedict R. Deangkinay

This repository contains a python code of ECE2112 Experiment 1, Programming Assignment 1. This Experiment contains the introduction of Python programming with three different problems

# A. Word Rotation Problem

> OBJECTIVES: Create a function named ```rotate_word()```that accepts a non-empty string Move the first character of the string to the end while keeping all remaining characters in their original order. Preserve the capitalization of every character.

## Discussion
### Functions Used
```python
def rotate_word(text):
    text[0]
    text[1:]
    return text[1:] + text[0]
```
The function ```rotate_word(text)``` utilizes string indexing and string slicing in order to satisfy the objective. The function has ```text[1:]``` will slice the letter at an index of 1 (which is the second letter) to the last index of the last letter of a word that is given in the variable text. Furthermore, ```text[0]``` extracts the character at index 0 (which is the first letter) and attaches to after the ```text[1:]``` syntax. No stop argument will default the string to be complete regardless of how many characters it has. No step argument defaults the step size to 1. Lastly, the ```return``` will become ```text[1:] + text[0]``` as a function of the output of ```rotate_word(text)``` when the code is executed.

# B. Username Builder Problem
> OBJECTIVES: Create a function named make ```username()``` that accepts two strings: first name and last name. The function must convert all letters to lowercase; remove all spaces from the first name; remove all spaces from the last name; and join the processed first and last names using one period (.).

## Discussion
### Functions Used
```python
def make_username(first_name, last_name):
   return first_name.lower().replace(" ", "")+"."+last_name.lower().replace(" ", "")
```
The function ```make_username(first_name, last_name):``` utilizes string concatenation in order to satisfy the objective. The function has ```first_name.lower()``` will convert every character in the string lowercase form while ```.replace(" ", "")``` will eliminate spacce characters present in the string. These two is concatenated with each other to both the ```first_name``` and the ```last_name```. Lastly, the ```return``` will become ```first_name.lower().replace(" ", "")+"."+last_name.lower().replace(" ", "")``` as a function of the output of ```make_username(first_name, last_name)``` when the code is executed.

# C. Bookend Swap Problem
> OBJECTIVES: Create a function named ```swap_bookends()``` that accepts a list containing at least two elements. Unpack the list into three variables: first – the first element; middle – a list containing everything between the first and last elements; and last – the last element. Using these variables, return a new list in which the first and last elements have exchanged positions. The elements in middle must remain in their original order. Do not modify the input list

## Discussion
### Functions Used
```python
def swap_bookends(items):
    first, *middle, last = items
    return  [last, *middle, first]
```
The function ```swap_bookends(items)``` utilizes the given extended sequence unpacking to allocate each elements present to a specific position in its list regardless of how long it is in order to satisfy the objective. The function has ```first, *middle, last = items``` will allocate the first element as the first one, in contrast, the last elements will be in last. The elements left will be allocated within the middle with ```*middle```. Lastly, the ``` return  [last, *middle, first]``` will return the list in a pattern in such a way that the last is followed by the original sequence of the middle and last is the first element of the list when the code is executed.

## README FILE VERSION HISTORY
*
*
* August 2
Thank you and Godbless
