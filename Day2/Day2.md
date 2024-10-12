
## Problem Statement 

Write a program to identify if the character is an alphabet or not.

## Description:

Take an input character from user and check whether it is an alphabet or not.

Input :

A

Output: 

Alphabet

Input:

7

Output:

Not an alphabet

## Solution

```python
# Provide your solution here.
print("enter a character")

char = input("")
if char.isalpha():
    print("Alphabet")
else:
    print("Not a Alphabet")

