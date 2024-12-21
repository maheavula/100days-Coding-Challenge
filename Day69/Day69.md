## Problem Statement 

Suppose, we have a class A which is the base class and we have a class B which is derived from class A and we have a class C which is derived from class B, we can access the functions of both class A and class B by creating an object for class C.

Hence, this mechanism is called multi-level inheritance. (B inherits A and C inherits B.)

Create a class called Equilateral which inherits from Isosceles and should have a function such that the output is as given below.

Sample Output

I am an equilateral triangle

I am an isosceles triangle I am a triangle
## Solution

```python
# Provide your solution here.

class Isosceles:
    def display(self):
        return "I am isoscelec traingle"

class Equaletral(Isosceles):
    def watch(self):
        return "I am equaleteral traingle"

class C(Equaletral):
    def display2(self):
        return "I am triangle"

obj = C()
print(obj.watch())
print(obj.display())
print(obj.display2())
