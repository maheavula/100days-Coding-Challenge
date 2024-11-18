## Problem Statement 

Write a Program to calculate the Frequency of characters in a string

Description

Get a string as the input from the user and find the frequency of characters in the string.

Input

program

Output

The frequency of a is 1

The frequency of g is 1

The frequency of m is 1

The frequency of o is 1

The frequency of p is 1

The frequency of r is 2
## Solution

```python
# Provide your solution here.
string = input("enter a string = ")

dit = {}
for i in string:
    if i in dit:
        dit[i] += 1
    else:
        dit[i] = 1

for i, j in sorted(dit.items()):
    print(f"The frequency of {i} is {j}")


