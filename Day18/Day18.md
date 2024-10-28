## Problem Statement 

Write a program to Add two fractions

Description

Get the values for numerator and denominator of two fractions, then add that fractions. Consider the following format

x3/y3 = (x1/y1) + (x2/y2)

here x3 = (x1*y2) + (x2*y1) and y3 = (y1*y2)

Input

2  3

4  3

Output

2/1   
## Solution

```python
# Provide your solution here.
x1, x2 = map(int,input("").split())
y1, y2 = map(int,input("").split())

x3 = (x1*y2) + (x2*y1)
y3 = (y1*y2)

gcd = 1
for i in range(1,min(x3,y3)+1):
    if x3 % i == 0 and y3 % i == 0:
        gcd = i

x3 = x3 // gcd
y3 = y3 // gcd

print(f"{x3}/{y3}")
