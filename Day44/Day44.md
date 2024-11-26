## Problem Statement 

Write Program to find number of even and odd elements in an array

Description

Get an array as input from the user and then count the number of even and odd elements present in the array.

Input

Enter size of array

4

Enter the elements :

1 3 4 5

Output

Number of even elements :

1

Number of odd elements :

3
## Solution

```python
# Provide your solution here.
def function(size, lst):
    e_c, o_c = 0, 0
    for i in lst:
        if i % 2 == 0:
            e_c += 1
        else:
            o_c += 1
    print(f"number of even elements \n {e_c}")
    return f"number of odd elements \n {o_c}"


if __name__ == '__main__':
    size = int(input("enter size= "))
    lst = list(map(int, input("enter lsit values= ").split()))
    result = function(size, lst)
    print(result)
