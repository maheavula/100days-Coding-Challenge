## Problem Statement 

Write a program to find Number of days in a given month of a given year

Description

Get the number of month and year as input from the user and check the number of days present in that month.

Input

Enter month : 2

Enter year : 2000

Output

29

## Solution

```python
# Provide your solution here.

month = int(input("months = "))
year = int(input("year = "))

if (year % 400 == 0 and year % 4 == 0) or year % 100 != 0:
    if month == 2:
        print("29")
    elif month in [1,3,5,7,8,10,12]:
        print("31")
    else:
        print("30")
else:
    if month == 2:
        print("28")
    elif month in [1,3,5,7,8,10,12]:
        print("31")
    else:
        print("30")
