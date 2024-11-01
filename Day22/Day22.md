## Problem Statement 

Write a program to express a number as a sum of two prime numbers

Description

Get a number as input from the user and express that number as sum of two prime numbers.

Input

4

Output

4 can be expressed as sum of 2 and 2
## Solution

```python
# Provide your solution here.
num = int(input("enter a number = "))
lst = []
for i in range(2,num):
    for j in range(2,i):
        if i % j == 0:
            break
    else:
        lst.append(i)
found = False
n = len(lst)
for i in range(n):
    for j in range(i, n):
        if lst[i] + lst[j] == num:
            print(f"{num}  can be expressed as {lst[i]} and {lst[j]}")
            found = True

if not found:
    print("no pairs are there")
