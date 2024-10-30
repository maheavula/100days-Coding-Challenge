## Problem Statement 

 Write a program to identify if the number is Prime number or not

Description

Get a number as input from the user and check whether that number is prime or not.

A prime number is a number with factors as 1 and that number itself.

Input

1

Output

1 is not a prime number

Input

5

Output

5 is a prime number  

 
## Solution

```python
# Provide your solution here.
num = int(input("enter a number = "))

for i in range(2,num):
    if num % i == 0:
        print("Not prime number")
        break
else:
    print("Prime number")


