## Problem Statement 

 Write a program to reverse a given number

Description

Get an input from the user and the print the reverse of the given number as the output

E.g. let the number be 324 then the reverse of the number is 423

Input

675

Output

576
## Solution

```python
# Provide your solution here.
num = int(input("enter a number = "))
ss = ""
new_num = num
for i in range(len(str(num))):
    r = int(new_num) % 10
    new_num = int(new_num) / 10
    ss += str(r)

print(ss)

