## Problem Statement 

Given an integer array of size N. Write Program to find maximum product subarray in a given array.

Sample input 1:

4

2 -4 -1 -3

Sample output 1:

8 = {2, -4, -1}

Sample input 2:

5

1 5 -7 5 3

Sample output 2:

15 = {5, 3}
## Solution

```python
# Provide your solution here.
size = int(input("Enter a size: "))

lst = list(map(int, input("enter array values: ").split(",")))

max_prd = lst[0]

for i in range(size):
    prd = lst[i]
    max_prd = max(max_prd, prd)
    for j in range(i+1, size):
        prd *= lst[j]
        max_prd = max(max_prd, prd)

print(max_prd)
