---
num: "Lecture 1"
desc: "Orientation to the course, a taste of Python"
ready: true
date: 2018-08-07 09:30:00.00-7:00
---

# Use Piazza for questions/announcements

# Gradescope for assignment submissions/grades

# Abstractions and Algorithms

# Functions and calling them

- `print`, `min`, etc.

# Python REPL (Read Eval Print Loop)

- Arithmetic expressions
- Note that `**` is right associative, not left associative.
- `int`, `float`, `bool`
- precedence, associativity
- Booleans/boolean-valued expressions: `True`, `False`, `<`, `==` (note double equals), etc.

# The textbook and the homework

You can start on the homework now---please use the PDF link! You'll need a copy of the textbook.

# IDLE and Python

Stuff I typed on the REPL in class:
```
Python 3.7.0 (v3.7.0:1bf9cc5093, Jun 26 2018, 23:26:24) 
[Clang 6.0 (clang-600.0.57)] on darwin
Type "copyright", "credits" or "license()" for more information.
>>> 2 + 2
4
>>> 2
2
>>> 4 * 7 + 3 - 2
29
>>> 2 ** 3
8
>>> 5 / 2
2.5
>>> type(2)
<class 'int'>
>>> type(2.5)
<class 'float'>
>>> 2 + 3 + 4
9
>>> 2 ** 3 ** 4
2417851639229258349412352
>>> (2 ** 3) ** 4
4096
>>> 2 ** (3 ** 4)
2417851639229258349412352
>>> 5 / 2
2.5
>>> 5 // 2
2
>>> 5 % 2
1
>>> abs(-2)
2
>>> min(2, 5, 1)
1
>>> max(2, 5)
5
>>> 
== RESTART: /Users/lawtonnichols/Desktop/cs8/code-from-class/08-07/hello.py ==
Hello, world!
>>> 
== RESTART: /Users/lawtonnichols/Desktop/cs8/code-from-class/08-07/hello.py ==
Hello, world!
>>> hi;aegru;aegroeghou
Traceback (most recent call last):
  File "<pyshell#17>", line 1, in <module>
    hi;aegru;aegroeghou
NameError: name 'hi' is not defined
>>> 5 / 0
Traceback (most recent call last):
  File "<pyshell#18>", line 1, in <module>
    5 / 0
ZeroDivisionError: division by zero
>>> min(2)
Traceback (most recent call last):
  File "<pyshell#19>", line 1, in <module>
    min(2)
TypeError: 'int' object is not iterable
>>> min()
Traceback (most recent call last):
  File "<pyshell#20>", line 1, in <module>
    min()
TypeError: min expected 1 arguments, got 0
>>> (7 // 2) + (5 % 2)
4
>>> 
== RESTART: /Users/lawtonnichols/Desktop/cs8/code-from-class/08-07/hello.py ==
Hello, world!
3
2
1
>>> 
== RESTART: /Users/lawtonnichols/Desktop/cs8/code-from-class/08-07/hello.py ==
Hello, world!
3
1
>>> print("hi")
hi
>>> 2 > 3
False
>>> 2 >= 3
False
>>> 2 <= 3
True
>>> 2 == 3
False
>>> 3 == 3
True
>>> 2 = 3
SyntaxError: can't assign to literal
>>> 2 != 3
True
>>> 2 < 3 and 4 < 5
True
>>> 2 > 3 or 4 < 5
True
>>> 2 > 3 and 4 < 5
False
>>> not (2 > 3)
True
>>> !True
SyntaxError: invalid syntax
>>> type(True)
<class 'bool'>
>>> (2 < 3) or (5 / 0 < 10)
True
>>> (5 / 0 < 10)
Traceback (most recent call last):
  File "<pyshell#37>", line 1, in <module>
    (5 / 0 < 10)
ZeroDivisionError: division by zero
>>> 
== RESTART: /Users/lawtonnichols/Desktop/cs8/code-from-class/08-07/hello.py ==
Hello, world!
3
2
1
>>> 
== RESTART: /Users/lawtonnichols/Desktop/cs8/code-from-class/08-07/hello.py ==
Hello, world!
starting in 3
starting in 2
starting in 1
starting now!
Hello‚ it's me
I was wondering if after all these years you'd like to meet
To go over everything
They say that time's supposed to heal ya
But I ain't done much healing
Hello‚ can you hear me?
I'm in California dreaming about who we used to be
When we were younger and free
I've forgotten how it felt before the world fell at our feet
There's such a difference between us
And a million miles
Hello from the other side
I must've called a thousand times
To tell you I'm sorry for everything that I've done
But when I call you never seem to be home
Hello from the outside
At least I can say that I tried
To tell you I'm sorry for breaking your heart
But it don't matter. It clearly doesn't tear you apart anymore
>>> 
```

# Code from class

<https://github.com/ucsb-cs8-m18/code-from-class/blob/master/08-07/hello.py>