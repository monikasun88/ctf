# [Mod 26](`https://play.picoctf.org/practice/challenge/144?category=2&page=1`)

## Status: Completed

[rot13](https://en.wikipedia.org/wiki/ROT13)

```

cvpbPGS{arkg_gvzr_V'yy_gel_2_ebhaqf_bs_ebg13_GYpXOHqX}

```

## Vim Implementation

1. Move cursor to input text line.
2. Type `g?` for Vim internal ROT13 cypher.
3. Type `$` to move to end of line.  

In full the command is `g?$`.