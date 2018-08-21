---
num: "Lecture 7"
desc: "while, command line args"
ready: true
date: 2018-08-21 09:30:00.00-7:00
---

# Code From Class

<https://github.com/ucsb-cs8-m18/code-from-class/tree/master/08-21>

Stubs and test-driven development
=================================
TDD stands for "test-driven development"

Everything your program needs to do is turned into
a test case. You write the tests *first*, before
writing the program! When the tests pass, you can
be reasonably confident that it works fine
(assuming you made very thorough tests).

A *stub* a piece of code used to stand in for some
other programming functionality. In this class it
will be used as a temporary substitute for
yet-to-be-developed code.

---

iClicker Questions
==================

```
0. What does the following code print?

   v = 0
   i = 1
   while i <= 5:
       v = v + i
       i = i + 1
   print(v)

   (a) 10
   (b) 15
   (c) 21
   (d) None of the above
```

In-Class Questions / Schedule of Events
=======================================

- stubs, TDD, example with calculate grade
+ elif version of calculate grade
- if name == __main__:
- importing
- shebang (`#!/usr/bin/env python3`)
  - command line args (shebang not necessary)
- Absolute vs. relative paths (book has nice tree)
- while, infinite loops
+ Fibonacci
