## Problem Statement 

 Write a program to find the double of the given number without using arithmetic operator

Description

For the given input number calculate the double of it without using arithmetic operator.

Input

4

Output

8
## Solution

```python
# Provide your solution here.
num = int(input("number = "))
lst= []
for i in range(1,3):
    lst.append(num)

print(sum(lst))
