## Problem Statement 

Write a program to identify if the number is Strong number or not

Description

Get a number as input from user and then check whether that number is a strong number or not. A number is said to be strong number if the sum of the factorial of each digit in the number is same as that of the number.

E.g. let the number be 145

Here 1! + 4! + 5! is 1 + 24 + 120 which is equal to 145 itself.

Input

121

Output

Not a strong number

Input

2

Output

Strong number
## Solution

```python
# Provide your solution here.

def function(N):
    stg = 0
    for i in N:
        fact = 1
        for j in range(1,int(i)+1):
            fact *= j
        stg += fact
    return stg == int(N)

n = input("enter a list of values = ")
result = function(n)
if result:
    print(f"{n},It is a strong number")
else:
    print(f"{n},It is not a strong number")

