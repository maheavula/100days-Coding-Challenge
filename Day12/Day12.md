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

def function(N):
    c = 0
    for i in str(N):
        c = c + int(i)
    return c


n = int(input("enter a number = "))
result = function(n)
print(f"{result}")
