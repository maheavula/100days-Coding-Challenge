## Problem Statement 

Given an integer array of size N, write a program to sort the array;

Sample input 1:

4

2 4 1 3

Sample output 1:

1 2 3 4

Sample input 2:

5

1 5 7 5 3

Sample output 2:

1 3 5 5 7

 
## Solution

```python
# Provide your solution here.
size = int(input("enter the size: "))

lst = list(map(int, input(" ").split(" ")))
l = len(lst)
for i in range(l):
    for j in range(l-i-1):
        if lst[j] > lst[j+1]:
            lst[j], lst[j+1] = lst[j+1], lst[j]

print(lst)

