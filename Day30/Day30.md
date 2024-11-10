## Problem Statement 

Write a Program to print Length of the string without using strlen() function

Description

Get a string as input from user and print the length of the string without using strlen() function.

Input

Hello

Output

5
## Solution

```python
# Provide your solution here.
string = input("enter a string = ")
count = 0
for i in string:
    count += 1

print(count)
