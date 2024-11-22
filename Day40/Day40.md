## Problem Statement 

 Write a Program to Replace substring in a string

Description

Get a string as input from the user and then get another string which has to be removed from the string.

Get the third input, the new substring which is placed in that substring position.

Finally print the output by replacing the substring with new string.

Input

Enter a string

talentbattle

Enter the substring to be removed :

talent

Enter the new substring :

student

Output

The new string :

studentbattle
## Solution

```python
# Provide your solution here.

full_string = input("enter full string = ").split()
rm_subst = input("enter removing substring = ")
add_subst = input("Enter adding substring = ")

f_string = ','.join(full_string)
fl_string = list(f_string)
for i in rm_subst:
    if i in fl_string:
        fl_string.remove(i)

sh_string = ''.join(fl_string)
print(add_subst + sh_string)
