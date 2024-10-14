## Problem Statement 

Write a program to identify of the a number is positive or negative

Description

Get an input number from the user and check whether it is a positive or negative number.

Input :

-10

Output : 

Negative number

Input :

0

Output :

Neither positive nor negative

Input :

15

Output : 

Positive number

## Solution

```python
# Provide your solution here.
num = int(input("enter a number\n"))
if num > 0:
    print("positive number")
elif num == 0:
    print("neither positive not negative")
else:
    print("negative number")

