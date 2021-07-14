# HackerRank

### :space_invader: Company Logo
**Goal:** To count 3 top-high of number of characters in each words.

```
import math
import os
import random
import re
import sys
import collections

s = sorted(input().strip())
s_counter = collections.Counter(s).most_common()
#print(s_counter)
s_counter = sorted(s_counter, key=lambda x: (x[1] * -1, x[0]))

for i in range(0, 3):
    print(s_counter[i][0], s_counter[i][1])
```
**Example Result:** <br/>
input = 'elephantttt'
```
t 4
e 2
a 1
```


### :space_invader: Division
**Goal:** 
- The first line should contain the result of integer division, a//b. 
- The second line should contain the result of float division, a/b .
```
if __name__ == '__main__':
    a = int(input())
    b = int(input())
    
    print("{}\n{}".format(a//b, a/b))
```
**Example Result:** <br/>
input = '5'and '3' <br/>
output = '1' and '1.66667' <br/>


### :space_invader: Weird or Not Weird (If Clause)
**Goal:** 
- If  is odd, print Weird.
- If  is even and in the inclusive range 2of 5 to , print Not Weird.
- If  is even and in the inclusive range 6of20  to , print Weird.
- If  is even and greater than , print Not Weird.

```
if __name__ == '__main__':
    n = int(input().strip())
    
    if (n in range (6, 21) or n % 2 != 0):
        print("Weird")
    else: print("Not Weird")
 ```
 **Example Result:** <br/>
input = 20 <br/>
output = Weird <br/>


### :space_invader: Print the square of each number on a separate line. (For loop)
```
if __name__ == '__main__':
    n = int(input())
    
    [print(i**2) for i in range(n)]
```
 **Example Result:** <br/>
input = 5 <br/>
output = 0,1,4,9,16 <br/>
