## Problem Statement 

 Given an array, rotate the array by one position in clock-wise direction.

Example 1:

Input:

N = 5

A[] = {1, 2, 3, 4, 5}

Output:

5 1 2 3 4

Example 2:

Input:

N = 8

A[] = {9, 8, 7, 6, 4, 2, 1, 3}

Output:

3 9 8 7 6 4 2 1
## Solution

```python
# Provide your solution here.
def function():
    N = int(input("N= "))
    A = list(map(int, input(" ").split(" ")))
    val = A[-1]
    A.remove(val)
    A.insert(0, val)
    print(' '.join(map(str, A)))

if __name__ == '__main__':
    function()
