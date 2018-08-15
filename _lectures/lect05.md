---
num: "Lecture 5"
desc: "pytest, floating point numbers are weird, (im)mutability"
ready: true
date: 2018-08-15 09:30:00.00-7:00
---

# Code from today's lecture

<https://github.com/ucsb-cs8-m18/code-from-class/tree/master/08-15>

You run pytest on a file (e.g., called "file.py") with
```
python3 -m pytest file.py
```

---

Turn in your homeworks in the correct format, please

---

Midterm next week! You'll have to write code on paper, so practice that (and practice running code in your head). You do get a cheat sheet, though!

---

In the terminal:
```
idle3 &
```
runs idle3 in the background, so you get access to your terminal prompt

---

iClicker Questions
==================

0. What is the value of x after the following code executes, assuming the user types "42"?

   x = float(input("Enter a number: "))

   (a) "42"
   (b) 42
   (c) 42.0
   (d) Something else

1. Consider the following code:

   def f(x):
     print(x**2 + 1) # not returning anything

   Assume you've loaded this into the REPL, and then type:
   >>> 3 * f(2) + 1

   What should you get back?

   (a) 16
   (b) 16.0
   (c) Error

In-Class Questions / Schedule of Events
=======================================

-1. For loop, and its sequential equivalent.

0. Together, let's change our calculate_grade function from last time to print out "A", "B", ..., "F" instead of "pass"/"fail"!

1. Together, let's add tests for this function and test our implementation using pytest. Maybe we should add an "invalid" option in case the numbers are out of range, or if the types are incorrect.

2. Floating point is inaccurate (sum([0.1] * 10)), python math library (sqrt, pi, etc.).

3. By yourself, write a 2D distance function and some tests for it. pytest.approx() will be necessary.

4. Immutable vs. mutable objects
