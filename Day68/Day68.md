## Problem Statement 

Add an element to the set. :

Delete an element from the set. (If the number is not present in the set, then do nothing). :

If the number is present in the set, then print "Yes"(without quotes) else print "No"(without quotes).

Input Format

The first line of the input contains where is the number of queries. The next lines contain query each. Each query consists of two integers and where is the type of the query and is an integer.

Constraints

 

Output Format

For queries of type print "Yes"(without quotes) if the number is present in the set and if the number is not present, then print "No"(without quotes).

Each query of type should be printed in a new line.

Sample Input

8

1 9

1 6

1 10

1 4

3 6

3 14

2 6

3 6

Sample Output

Yes

No

No
## Solution

```python
# Provide your solution here.
def function():
    T = int(input("T= "))
    aq = 1
    dq = 2
    pq = 3
    st = set()
    for i in range(T):
        q, n = map(int, input("= ").split(" "))
        if q == aq:
            st.add(n)
        elif q == dq:
            st.remove(n)
        elif q == pq:
            if n in st:
                print("Yes")
            else:
                print("No")


if __name__ == '__main__':
    function()
