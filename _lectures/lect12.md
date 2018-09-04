---
num: "Lecture 12"
desc: "File permissions, Stacks, Local vs. Global"
ready: true
date: 2018-09-04 09:30:00.00-7:00
---

# Code from class

<https://github.com/ucsb-cs8-m18/code-from-class/tree/master/09-04>

Final next week!

You don't have to print out ic01 tomorrow.

---

iClicker Questions
==================

```
0. What is the octal number that represents the permissions r-x-w---x?

   (a) 614
   (b) 521
   (c) 246
   (d) 241
```

In-Class Questions / Schedule of Events
=======================================

+ Text prediction program (only preserve alphanumeric things)
- file permissions, octal (see <https://ucsb-cs8.github.io/topics/number_conversions/>)
  - chmod changes permissions
- reuse, modularity, encapsulation
  - reuse: if I want to do the same thing multiple times, I can put
    that thing in a function! Then I can just call the function a
    bunch of times instead of copying and pasting the same code a
    bunch of times.
    - What from lab05 is an example of reuse and why?
  - modularity: breaking down things into smaller, simpler pieces. 
    - Your tree drawing function draws triangles!
  - encapsulation: the user of your function doesn't need to know how
    it's implemented--they just need to know how to call it
    - What from lab05 is an example of encapsulation and why?
- push and pop in the context of lists (push is append)
+ RPN calculator example
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
