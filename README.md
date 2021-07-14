# Hackerrank

### Company Logo
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


### Division
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
