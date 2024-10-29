## Problem Statement 

Write a program to identify if the number is Armstrong number or not

Description

Get an input number from user and check whether the given number is an Armstrong number or not.

E.g. Let the number be 1634,

Here 1^4 + 6^4 + 3 ^4 + 4^4 = 1634

Therefore, this is an Armstrong number

Input

153

Output

Armstrong number

Input

121

Output

Not an Armstrong number  
## Solution

```python
# Provide your solution here.
num = int(input("enter a num= "))

num_l = len(str(num))
new_n = 0
for i in str(num):
    new_n += int(i)**num_l

if new_n == num:
    print("Armstrong")
else:
    print("Not armstrong")

