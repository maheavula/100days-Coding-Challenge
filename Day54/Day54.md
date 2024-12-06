## Problem Statement 

Given an integer array of size N. Write Program to find whether Arrays are disjoint or not. Two arrays are said to be disjoint if they have no elements in common.

Sample input 1:

4

2 -4 -1 -3

3

1 3 5

Sample output 1:

Disjoint

Sample input 2:

5

1 5 -7 6 3

4

2 4 6 8

Sample output 2:

Not disjoint. ( 6 is common)
## Solution

```python
# Provide your solution here.

def disjoint(m,lst1,n,lst2):
    isnotdisjoint = False
    for i in lst1:
        if i in lst2:
            isnotdisjoint = True

    if isnotdisjoint:
        return "Not disjoint"
    else:
        return "Disjoint"

if __name__ == '__main__':
    m = int(input("enter size: "))
    lst1 = list(map(int, input("= ").split(" ")))
    n = int(input("enter size: "))
    lst2 = list(map(int, input("= ").split(" ")))

    result = disjoint(m,lst1,n,lst2)
    print(result)
