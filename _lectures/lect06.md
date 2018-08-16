---
num: "Lecture 6"
desc: "Formatting, mutability, swapping, word-counting example"
ready: true
date: 2018-08-16 09:30:00.00-7:00
---

# Code from classs

<https://github.com/ucsb-cs8-m18/code-from-class/tree/master/08-16>

[Python print documentation](https://docs.python.org/3/library/functions.html#print)
[Python isspace documentation](https://docs.python.org/3/library/stdtypes.html#str.isspace)

# Pair Programming

<https://www.youtube.com/watch?v=rG_U12uqRhE>

Try to choose a partner near the same prior experience and confidence level as yourself.

You will learn more than if you and your partner are at very disparate levels of experience/confidence.

# Strong Style Pairing

All code goes through two minds.

<http://llewellynfalco.blogspot.com/2014/06/llewellyns-strong-style-pairing.html>

---

iClicker Questions
==================

0. Consider the following code:
   
   l = [[1,2,3], [4,5,6], [7,8,9]]
   for inner_l in l:
       for n in inner_l:
           print(n + 1)

   Assuming you run this code in the REPL, what is the second thing that gets printed?

   (a) 1
   (b) 2
   (c) 3
   (d) Something else


In-Class Questions / Schedule of Events
=======================================

0. Immutable vs. mutable objects, and parameter passing. How do function calls look in memory?

1. Formatted output. Month/Day/Year, Day/Month/Year, 10×10 times table example.

2. Swapping variables.

3. Word count example.

4. Together, let's write a function that draws a bunch of concentric turtle graphics circles using a loop.