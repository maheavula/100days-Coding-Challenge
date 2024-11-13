## Problem Statement 

Write a Program to Remove vowels from a string

Description

Get a string as the input from the user and then remove all the vowel letters from the string and give the output.

Input

remove

Output

rmv
## Solution

```python
# Provide your solution here.

string = input("enter a string = ")

wo_ov = ""
for i in string:
    if i in ['a','e','i','o','u','A','E','I','O','U']:
        pass
    else:
        wo_ov += i

print(wo_ov)
