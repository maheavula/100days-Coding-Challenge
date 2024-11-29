## Problem Statement 

Write Program to find longest palindrome in an array

Description

Get an array as the input from the user and find the longest palindrome in that array.

Input

Enter the size of array

3

Enter the elements of array

121 10456 1000001

Output

1000001
## Solution

```python
# Provide your solution here.

size = int(input("enter size of array= "))

lst = list(map(int, input("enter array elements= ").split(" ")))

lst1 = []
for i in lst:
    if i == int(str(i)[::-1]):
        lst1.append(i)
print(max(lst1))
