## Problem Statement 

Write Program to remove duplicate elements in an array

Description

Get an array as input from the user and then remove all the duplicate elements in that array.

Input

Enter the size of array

5

Enter the elements of array

35 35 45 60 60

Output

35 45 60
## Solution

```python
# Provide your solution here.
size = int(input("enter size of array= "))

lst = list(map(int, input("enter array elements= ").split(" ")))

for i in set(lst):
    print(i, end=" ")

