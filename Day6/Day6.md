## Problem Statement 

 Write a program to find the Quadrants in which coordinates lie

Get the value of x and y coordinates as input from the user and check in which quadrant the point lies and print it.

Input

10 20

Output

This point lies in first quadrant.

Input

-10 20

Output

This point lies in second quadrant.

## Solution

```python
# Provide your solution here.
q1 = int(input("q1 = "))
q2 = int(input("q2 = "))
if q1 > 0 and q2 > 0:
    print("This point lies on the first Quadrant")
elif q1 < 0 and q2 > 0:
    print("This point lies on the second Quadrant")
elif q1 > 0 and q2 < 0:
    print("This point lies on the third Quadrant")
elif q1 < 0 and q2 < 0:
    print("This point lies on the fourth Quadrant")
else:
    print("This point lies at origin")
