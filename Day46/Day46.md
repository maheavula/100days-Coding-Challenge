## Problem Statement 

Write Program to find sum of elements in an array

Description

Get an array as the input from the user and find the sum of the elements.

Input

Enter the size of array

3

Enter the elements of array

5 10 15

Output

30
## Solution

```python
# Provide your solution here.

size = int(input("enter the size of array= "))
lst = list(map(int, input("enter list values= ").split()))

summ = 0
for i in lst:
    summ += i
print(summ)
