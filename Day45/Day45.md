## Problem Statement 

Write Program to find smallest and largest element in an array

Description

Get an array as input from the user and then find the smallest and largest element in the array.

Input

Enter the size of array :

5

Enter the elements :

10 20 5 40 30

Output

Smallest Number :

5

Largest Number :

40
## Solution

```python
# Provide your solution here.
size = int(input("enter the size of array= \n"))
lst = list(map(int, input("enter the elements= \n").split(" ")))
lst.sort()
print(f"smallest number: \n{lst[0]}")
print(f"largest number: \n{lst[-1]}")
