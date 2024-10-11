
## Problem Statement 

Write a program to identify if the character is a vowel or consonant.

## Description
Take an input character from the user and check whether the given input is a vowel or consonant.

Input

A

Output

Vowel

Input

m

Output

Consonant

Input

3

Output

Invalid Input

## Solution

```python
# Provide your solution here.
char = input("")

vowels = ['A','E','I','O','U','a','e','i','o','u']
if len(char) != 1:
    print("Length should be one character")
elif char.isdigit():
    print("Invalid input")
elif char.isalpha():
    if char in vowels:
        print("Vowel")
    else:
        print("Consonant")
else:
    print("Invalid input")

```
