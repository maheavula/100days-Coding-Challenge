## Problem Statement 

Write a Program to Toggle each character in a string

Description

Get an input string from user and then convert the lower case of alphabets to upper case and all upper-case alphabets into lower case.

Input

Hello

Output

hELLO
## Solution

```python
string = input("enter a string = ")
new_str = ""
for i in string:
    if i.isupper():
        new_str += i.lower()
    elif i.islower():
        new_str += i.upper()

print(new_str)
