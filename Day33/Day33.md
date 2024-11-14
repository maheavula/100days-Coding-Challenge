## Problem Statement 

Write a Program to check if String is a palindrome or not

Description

Get an input string from the user and then check whether it is a palindrome string or not.

Input

noon

Output

Palindrome

Input

Talent

Output

Not a Palindrome
## Solution

```python
# Provide your solution here.

string = input("enter a string =")

if string == string[::-1]:
    print("Palindrome")
else:
    print("Not a palindrome")
