## Problem Statement 

Write a program to find the Factors of a number

Description

Get an input from the user and find the factors of the number.

Input

4

Output

1,2,4  
## Solution

```python
# Provide your solution here.
def function(N):
    lst = []
    for i in range(1,N+1):
        if N % i == 0:
            lst.append(i)
    return ','.join(map(str,lst))

n = int(input("enter a number = "))
result = function(n)
print(f"{result}")
