## Problem Statement 

Write a Program to Toggle each character in a string

Description

Get an input string from user and then convert the lower case of alphabets to upper case and all upper-case alphabets into lower case.

Input

Hello

Output

hELLO
## Solution

```python
# Provide your solution here.

lst = list(map(str, input("enter list of numbers = ").split()))

len_lst = []

for i in lst:
    if i == i[::-1]:
        len_lst.append(len(i))

ind = len_lst.index(max(len_lst))

print(lst[ind])
