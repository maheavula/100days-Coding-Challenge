## Problem Statement 

Write a program to print Pyramid pattern using stars

Description

Get the number of lines as the input and print stars in that many lines or rows in a pyramid shape.

Input

4

Output

  *

 ***

*****

*******
## Solution

```python
# Provide your solution here.
rows = int(input("enter number of rows = "))

for r in range(1,rows+1):
    for c in range(r*2-1):
        print("*",end="")
    print()


