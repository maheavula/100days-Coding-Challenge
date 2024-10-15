## Problem Statement 

Write a program to identify if the number is even or odd

Description

Get a number as input from the user and check whether the given number is odd or even

Input

10

Output

Even

Input

5

Output

Odd

## Solution

```python
# Provide your solution here.
num = int(input("enter a number\n"))

if num % 2 == 0:
    print("Even")
else:
    print("Odd")
