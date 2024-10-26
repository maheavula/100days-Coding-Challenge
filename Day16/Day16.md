## Problem Statement 

Write a program to identify if the number is Perfect number or not

Description

Get the input from the user and check whether that number is a perfect number or not.

E.g. Let number is 28, factors of 28 are 1,2,4,7,14. Now the sum of all these factors are 28 itself.

Input

28

Output

Perfect Number

Input

4

Output

Not a perfect number 
## Solution

```python
# Provide your solution here.
def function(N):
    lst = []
    for i in range(1 , N):
        if N % i == 0:
            lst.append(i)
    return sum(lst) == N

n = int(input("enter a number = "))
result = function(n)
if result:
    print("perfect number")
else:
    print("Not a perfect number")
