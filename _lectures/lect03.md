---
num: "Lecture 3"
desc: "Python turtle graphics"
ready: true
date: 2018-08-09 09:30:00.00-7:00
---

# Code from today's lecture

Click on any of the `.py` files here to see the turtle stuff: <https://github.com/ucsb-cs8-m18/code-from-class/tree/master/08-09>

Stuff from the REPL:

```
Python 3.7.0 (v3.7.0:1bf9cc5093, Jun 26 2018, 23:26:24) 
[Clang 6.0 (clang-600.0.57)] on darwin
Type "copyright", "credits" or "license()" for more information.
>>> def sum(x, y):
    x + y

    
>>> sum(5, 7)
>>> def sum(x, y):
    return x + y

>>> sum(5, 7)
12
>>> def print_some_stuff():
    print("hi")
    print("bye")

    
>>> print_some_stuff()
hi
bye
>>> int(True)
1
>>> int(False)
0
>>> def tup_add(x, y):
    first_entry_of_x = x[0]
    first_entry_of_y = y[0]
    second_entry_of_x = x[1]
    second_entry_of_y = y[1]
    return (first_entry_of_x + first_entry_of_y, second_entry_of_x + second_entry_of_y)

>>> tup_add((1, 2), (2, 3))
(3, 5)
>>> assert(1 < 2)
>>> assert(2 < 1)
Traceback (most recent call last):
  File "<pyshell#23>", line 1, in <module>
    assert(2 < 1)
AssertionError
>>> def tup_add2(x, y):
    assert(len(x) == 2 and len(y) == 2)
    return (x[0] + y[0], x[1] + y[1])

>>> tup_add((1, 2), (2, 3))
(3, 5)
>>> tup_add((1, 2, 3), (2, 3, 4))
(3, 5)
>>> tup_add2((1, 2), (2, 3))
(3, 5)
>>> tup_add2((1, 2, 3), (2, 3, 4))
Traceback (most recent call last):
  File "<pyshell#31>", line 1, in <module>
    tup_add2((1, 2, 3), (2, 3, 4))
  File "<pyshell#27>", line 2, in tup_add2
    assert(len(x) == 2 and len(y) == 2)
AssertionError
>>> range(10)
range(0, 10)
>>> list(range(10))
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
>>> for x in range(10):
    print(x)

    
0
1
2
3
4
5
6
7
8
9
>>> 
```

---

Precedence: the way parentheses get added when the operations are different: (2 ** 3) + 5 - (7 / 8)

Associativity: the way parentheses get added when the operations have the same precedence: (2 + 3) + 4 vs. 2 ** (3 ** 4), also 2 + 3 - 4 because + and - have the same precedence level

Evaluation order: the way the left hand sides of operations get evaluated before the right hand sides, or the way that function arguments get evaluated before a function gets called

---

Parameters vs. arguments

---

iClicker Questions
==================

0. How many things are wrong with this function definition? (It's supposed to add the two numbers you give it.)
  
     def sum(x, y):
        return x + y

   (a) 0
   (b) 1
   (c) 2
   (d) 3
   (e) ≥ 4

1. What is the result of int(True)?

   (a) 0
   (b) 1
   (c) Error


In-Class Problems
=================

0. Write a Python function that takes two tuples
   (tuples look like «(4, 5, 6)») of length 2, and
   sums together their corresponding parts.

   That is, given (1, 2) and (2, 3), your function
   should give back (3, 5).

1. Does your function still work if you give it
   tuples of sizes > 2? Sizes < 2?

   What would you need to guarantee that the
   arguments you were given were of the correct
   size?

`assert` function