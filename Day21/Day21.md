## Problem Statement 

Write a program to identify if the number is Palindrome or not

Description

Get a number as input from the user and check whether that number is a Palindrome or not.

Input

121

Output

Palindrome

Input

34

Output

Not a Palindrome
## Solution

```python
# Provide your solution here.
num = int(input("enter a number = "))
n_num = num
new_n = ""
for i in range(len(str(num))):
    q = int(n_num) % 10
    n_num = int(n_num) / 10
    new_n += str(q)
if num == new_n:
    print("Palindrome Number")
else:
    print("Not a palindrome")
    
