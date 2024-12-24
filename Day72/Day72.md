## Problem Statement 

In this problem you will have to implement a simple editor. The editor maintains the content of a string S and have two following functions:
 

"+ i x": insert a string x into the current string S after the i'th character of the S (we use 1-indexing in this problem). When i equals to 0 it mean we add x at the beginning of S.
"? i len": Print the sub-string of length len starting at position i'th of S.
At the beginning, the editor holds an empty string. There will be Q queries of the two types described above.

Input

The first line contains the integer Q. Each line in the next Q lines contains one query.

Output

For each query of the second type, print out the answer sub-string in one line.

Sample Input

5

+ 0 ab

+ 1 c

? 1 3

+ 2 dd

? 1 5

Sample Output

acb

acddb
## Solution

```python
# Provide your solution here.
def insert(string_S, sub, pos_i=0):
    return string_S[:pos_i] + sub + string_S[pos_i:]



Q = int(input("Q= "))
S = ""
for i in range(Q):
    query = input().split(" ")
    c = query[0]
    i = int(query[1])

    if c == '+':
        sub = query[2]
        if i == '0':
            S = sub + S
        else:
            S = insert(S, sub, i)
    else:
        l = int(query[2])
        print(S[i-1:l+1])

