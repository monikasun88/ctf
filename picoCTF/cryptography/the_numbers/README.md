# [The Numbers](`https://play.picoctf.org/practice/challenge/68?category=2&page=1`)

## Status: Completed

```python

import string 
cipher="16 9 3 15 3 20 6 { 20 8 5 14 21 13 2 5 18 19 13 1 19 15 14 }".split(" ")
key={str(i+1):f for i,f in enumerate(string.ascii_lowercase)}
print("".join([key.get(v, v) for v in cipher]))

```