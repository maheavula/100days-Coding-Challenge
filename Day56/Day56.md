## Problem Statement 

Write Program to find whether the numbers of an array be made equal

Description

Check whether the numbers of array be made equal or not

For eg, for the following input it should print yes because

50*2*3 , 75*2*2 and 150*2 are equal to 300 in all cases. So array numbers can be made equal

Input

3

50 75 150

Output

Yes
## Solution

```python
# Provide your solution here.

def function(size, lst):
    for i in range(size):
        while lst[i] % 2 == 0:
            lst[i] /= 2
        while lst[i] % 3 == 0:
            lst[i] /= 3
    for i in range(size):
        if lst[i] != lst[0]:
            return False
    return True

if __name__ == '__main__':
    size = int(input("Enter size of array: "))
    lst = list(map(int, input("= ").split(" ")))
    result = function(size, lst)
    print(result)
