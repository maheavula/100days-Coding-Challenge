## Problem Statement 
Write a program to find Sum of digits of a number

Description

Get a number from user and then find the sum of the digits in the given number.

E.g. let the number = 341

Sum of digits is 3+4+1= 8

Input

4521

Output

12

## Solution

```python
# Provide your solution here.
def function(lst):
    lst.sort()
    return lst[1]


listt = input("enter a list of values = ").split()
result = function(listt)
print(f"{result}")
