## Problem Statement 

Check if two strings match where one string contains wildcard characters

Description

Get two strings as input from the user, first with wildcard characters (* and ?) and second without wildcard characters.

Then check whether they match or not.

Input

Ta**nt

Talent

Output

Yes they match
## Solution

```python
# Provide your solution here.
def function(input1, input2):

    la, lb = len(input1), len(input2)
    count = 0
    star_c = input1.count('*')
    quat_c = input2.count("?")
    if la == lb:
        for i in range(la):
            if input1[i] == input2[i]:
                pass
            else:
                count += 1
    else:
        return "Not Matched"

    if (star_c == count) or (quat_c == count):
        return "Yes they match"
    else:
        return "No, they dont match"

if __name__ == '__main__':
    input1 = input("enter first wild string = ")
    input2 = input("enter second normal string = ")
    result = function(input1, input2)
    print(result)

