## Problem Statement 


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

