## Problem Statement 

Write a program to find Fibonacci series up to n

Description

Fibonacci series is a special series where nth term is the sum of previous two terms in the series. The series starts with 0 and 1 as the first and second term of the series respectively.

Here you need to get the value for nth term from user and then print Fibonacci series containing n terms.

Input

5

Output

0,1,1,2,3

Input

8

Output

0,1,1,2,3,5,8,13

## Solution

```python
# Provide your solution here.

def function(N):
    a = 0
    b = 1
    lst = [a,b]
    for i in range(1,N-1):
        c = a + b
        a = b
        b = c
        lst.append(c)
    return ','.join(map(str, lst))

n = int(input("enter a number = "))
result = function(n)
print(f"{result}")
