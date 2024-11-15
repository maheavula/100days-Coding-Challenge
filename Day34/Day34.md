## Problem Statement 

Write a Program to Remove brackets from an algebraic expression

Description

Get an algebraic expression as input from the user and then remove all the brackets in that.

Input

7x+(2*y)

Output

7x+2*y
## Solution

```python
# Provide your solution here.

exp = input("enter a algebra expression = ")

new_exp = ""
for i in exp:
    if i == '(' or i == ')':
        pass
    else:
        new_exp += i
print(new_exp)
