## Problem Statement 

Write Program to find the array type

Description

Get an array as input from the user and check the type of the array, whether it is odd, even or mixed type.

Input

Enter size of array :

3

Enter elements 

1 3 5

Output

Odd
## Solution

```python
# Provide your solution here.

def function(size, lst):
    c_e, c_o = 0, 0
    for i in lst:
        if i % 2 == 0:
            c_e += 1
        else:
            c_o += 1

    if size == c_e:
        return "Even"
    elif size == c_o:
        return "Odd"
    else:
        return "Mixed"

if __name__ == '__main__':
    size = int(input("enter size = "))
    lst = list(map(int, (input("enter a list of values= ").split())))
    result = function(size, lst)
    print(result)
