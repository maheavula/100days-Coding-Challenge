## Problem Statement 

Write a Program to print Non-repeating characters in a string

Description

Get a string as the input from the user and print the non-repeating characters in a string.

Input

Hello

Output

H e o
## Solution

```python
# Provide your solution here.

string = input("enter a string = ")

dit = {}

for i in string:
    if i in dit:
        dit[i] += 1
    else:
        dit[i] = 1
for i, j in dit.items():
    if j > 1:
        pass
    else:
        print(f"{i}", end=" ")
