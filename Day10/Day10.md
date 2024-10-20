## Problem Statement 

 Write a program to find Factorial of a number

Description

Get a number from user for which you need to fin the factorial, then calculate the factorial and give it as the output.

Input

4

Output

24

## Solution

```python
# Provide your solution here.
num = int(input("enter a number = "))
fact = 1
for i in range(1,num+1):
    fact *= i
print(fact)
