
## Problem Statement 

The weather report of Magicland is Good if the number of sunny days in a week is strictly greater than the number of rainy days.

Given 7 integers A1,A2,A3,A4,A5,A6,A7 where Ai=1 denotes that the ith day of week in Magicland is a sunny day, Ai=0 denotes that the ith day in Magicland is a rainy day. Determine if the weather report of Magicland is Good or not.

Input Format

First line will contain T, number of testcases. Then the testcases follow.

Each testcase contains of a single line of input, 7 space separated integers A1,A2,A3,A4,A5,A6,A7.

Output Format

For each testcase, print "YES" if the weather report of Magicland is Good, otherwise print "NO". Print the output without quotes.

You may print each character of the string in uppercase or lowercase (for example, the strings "yEs", "yes", "Yes" and "YES" will all be treated as identical).
## Solution

```python
# Provide your solution here.
def function():
    T = int(input("T= "))
    c1 = 0
    c0 = 0
    for i in range(T):
        lst = list(map(int, input("= ").split(" ")))
        c1 = lst.count(1)
        c0 = lst.count(0)
        if c1 > c0:
            print("Yes")
        else:
            print("No")

if __name__ == '__main__':
    function()
