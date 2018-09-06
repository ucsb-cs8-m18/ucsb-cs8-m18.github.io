---
num: "Lecture 13"
desc: "ic01, stacks"
ready: true
date: 2018-09-05 09:30:00.00-7:00
---

# Code from class

<https://github.com/ucsb-cs8-m18/code-from-class/tree/master/09-05>

---

```
iClicker Questions
==================

0. What does the following code return when called with f(2)?

   def f(x):
     if x == 0:
       return 0
     else:
       return f(x-1)

   (a) 0
   (b) 1
   (c) 2
   (d) None of the above

1. What about f(-2)?
   
   (a) 0
   (b) -1
   (c) -2
   (d) None of the above
```

In-Class Questions / Schedule of Events
=======================================

- The Shakespeare text prediction program works now!
- local vs. global
  - variables defined inside a function are called *local*
    variables. They don't affect any variables defined with the same
    name elsewhere. This is good for encapsulation.
  - different functions have different *spaces* for variables. These
    are called namespaces.
  - a new namespace is made for every function call (example on
    p. 208)
  - *global* variables are those defined outside of any function
    - they can be accessed anywhere, but you need to use special code
      to update them inside of functions
- a very quick taste of recursion (more to come tomorrow)
- ic01!
- stacks, push and pop (starts at __main__)
  - <https://www.cs.ucsb.edu/~pconrad/cs8/topics.beta/theStack/>