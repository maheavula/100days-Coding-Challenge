## Problem Statement 

Write a Program to Count the sum of numbers in a string

Description

Get a string from the user and find the sum of numbers in the string.

Input

Hello56

Output

11
## Solution

```python
# Provide your solution here.
string_num = input("enter a string number = ")

s = 0
for i in string_num:
    if i.isdigit():
        s += int(i)

print(s)
