## Problem Statement 

Write a Program to Capitalize the first and last letter of each word of a string

Description

Get a string from the user and then change the first and last letter to uppercase.

Input

programming

Output

ProgramminG
## Solution

```python
# Provide your solution here.

string = input("enter a string = ")

new_str =""
l = len(string)
for i in range(l):
    if i == 0 or i == l-1:
        new_str += string[i].upper()
    else:
        new_str += string[i]

print(new_str)
