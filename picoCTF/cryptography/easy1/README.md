# [Easy 1](`https://play.picoctf.org/practice/challenge/43?category=2&page=1`)

## Status: Completed

[One time pad](https://en.wikipedia.org/wiki/One-time_pad)

```python

import string

def decode_letter(kl, cl):
    table_key = dict()
    letters = [l for l in string.ascii_lowercase]
    for i in range(0, 26):
        letters_inc = letters[i:] + letters[:i]
        table_key[letters[i]] = {letters_inc[i]:l for i,l in enumerate(letters)}
    return(table_key[kl.lower()][cl.lower()])

def decode_message(k, c):
    return("".join([decode(k[i], c[i]) for i,u in enumerate(c)]).upper())

# Wikipedia example
decode_message("XMCKL", "EQNVZ")

# picoCTF flag
decode_message("SOLVECRYPTO", "UFJKXQZQUNB")

```

Flags tried:
- MTUFBSQOJGP
- YJCLHMSIVGN