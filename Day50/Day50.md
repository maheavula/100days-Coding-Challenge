## Problem Statement 

Given an integer array of size N. Write Program to find sum of positive square elements in the array.

Sample input 1 :

4 1 2 3 4

Sample output 1 :

30

Explanation :

(1 + 4 + 9 + 16) = 30

Sample input 2 :

4 -1 -2 -3 -4

Sample output 2 :

30

Explanation :

(1 + 4 + 9 + 16) = 30
## Solution

```python
# Provide your solution here.
size = int(input("enter the size: "))
lst = list(map(int, input(" ").split(" ")))

summ = 0
for i in lst:
    summ += i**2
print(summ)
