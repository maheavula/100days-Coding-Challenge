## Problem Statement 

Write a program to Replace all 0’s with 1 in a given integer

Description

Get a number as input from the user and find the zeros present in that number.

Then convert the zeros into one and then print it.

Input

310020

Output

311121
## Solution

```python
# Provide your solution here.
num = int(input("enter a num = "))
new_s = ""
for i in str(num):
    if i == '0':
        new_s += '1'
    else:
        new_s += i

print(new_s)
