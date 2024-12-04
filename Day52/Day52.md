## Problem Statement 

Given an integer array of size N, write a program to reverse the array;

Sample input 1:

4

2 4 1 3

Sample output 1:

3 1 4 2

Sample input 2:

5

1 5 7 5 3

Sample output 2:

3 5 7 5 1
## Solution

```python
# Provide your solution here.

N = int(input("enter the size of an array"))

array = list(map(int, input("enter array elements: ").split(" ")))

if N % 2 == 0:
    l = int(N/2)
    for i in range(l):
        temp = array[i]
        array[i] = array[N-i-1]
        array[N-i-1] = temp
else:
    l = int(N/2)
    for i in range(l):
        temp = array[i]
        array[i] = array[N - i - 1]
        array[N - i - 1] = temp

print(array)
