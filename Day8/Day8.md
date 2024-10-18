## Problem Statement 

Write a program to find roots of a quadratic equation

Description

Get the values of a, b and c (coefficients of quadratic equation) as input from the user and calculate the roots and print as the output.

Input

Enter the value of a, b and c : 1 -6 9

Output

Roots are equal

Root 1= root 2 = 3.00

## Solution

```python
# Provide your solution here.
import math
a = float(input("a = "))
b = float(input("b = "))
c = float(input("c = "))

discriminant = b*b - (4*a*c)

if discriminant > 0:
    r1 = (-b - math.sqrt(discriminant)) / (2*a)
    r2 = (-b + math.sqrt(discriminant)) / (2*a)
    print(f"There are two, root1 = {r1:.2f} and root2 = {r2:.2f}")
elif discriminant == 0:
    r1 = (-b) / 2*a
    print(f" root1 = {r1:.2f} and None")

else:
    print("No roots, Discriminant < 0")

