## Problem Statement 

Write a Program to check if two strings are Anagram or not

Description

Get two strings as input from the user and check whether it is Anagram or not.

Input

sunlight thgiluns

Output

Anagram
## Solution

```python
# Provide your solution here.
strings = input("enter a string = ").split()

l = len(strings)
for i in range(0,2):
    for j in strings[0]:
        for k in j:
            if k not in strings[1]:
                print("not anagram")
                break
            else:
                print("anagram")
                break
        break
    break
