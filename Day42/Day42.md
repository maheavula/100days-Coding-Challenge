## Problem Statement 

Write Program to check if two arrays are the same or not

Description

Get two arrays as the input from the user and check whether it is the same or not.

Input

Enter the size of first array :

3

Enter the size of second array :

3

Enter elements of first array :

1 2 3

Enter elements of second array :

1 2 3

Output

Same
## Solution

```python
# Provide your solution here.
def function(size_ar1, size_ar2):

    if size_ar1 != size_ar2:
        return "Size Not same"

    f_list = list(map(str, input("enter first array values = ").split()))
    s_list = list(map(str, input("enter second array values = ").split()))

    if f_list == s_list:
        return "array same"
    else:
        return "array not same"

if __name__ == '__main__':
    size_ar1 = int(input("enter size of first array = "))
    size_ar2 = int(input("enter size of second array = "))
    result = function(size_ar1, size_ar2)
    print(result)

