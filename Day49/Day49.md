## Problem Statement 

 Given 2 integer arrays X and Y of same size. Consider both arrays as vectors and print the minimum scalar product (Dot product) of 2 vectors.

Sample input 1 :

4

1 2 3 4

5 6 7 8

Sample output 1 :

60

Explanation :

(4*5 + 3*6 + 2*7 + 1*8) = 60

Sample input 2 :

4

-1 -2 -3 -4

5 6 -7 -8

Sample output 2 :

-17

Explanation :

(-1*-8 + -2*-7 + -3*6 + -4*5) = -17
## Solution

```python
# Provide your solution here.
size = int(input("enter size of arrays: "))

lst1 = list(map(int, input("= ").split(" ")))
lst2 = list(map(int, input("= ").split(" ")))

min_sum = 0
for i in range(0,size):
    min_sum += lst1[i] * lst2[size-1-i]

print(min_sum)

