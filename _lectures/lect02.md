---
num: "Lecture 2"
desc: "SSH, More Python data types, and functions"
ready: true
date: 2018-08-08 09:30:00.00-7:00
---

# Connecting to CSIL through SSH

<https://ucsb-cs8.github.io/topics/x11/>

Either
`ssh -X username@csil-XX.cs.ucsb.edu` or
`ssh -Y username@csil-XX.cs.ucsb.edu`
where XX with a number between 01 and 48.

On Windows, `csil-XX.cs.ucsb.edu` is the hostname.

Use the `idle3` command to start IDLE from the remote machine.

# Functions

In Math: $$ f(x) = x^2 $$

In Python:

```python
def f(x):
   " multiply x times itself "
   return x * x
```

# return vs. print

* I give you a dollar and you give me something tangible in return (that I can hold in my hand)

vs.

* I give you a dollar and you "do something for me" 

Economists call this a "good" vs. a "service".

This is an analogy for return vs. print.  We'll explain more in lecture today and future lectures.

# Code from today's lecture

From the REPL:

```python
Python 3.7.0 (v3.7.0:1bf9cc5093, Jun 26 2018, 23:26:24) 
[Clang 6.0 (clang-600.0.57)] on darwin
Type "copyright", "credits" or "license()" for more information.
>>> True or False
True
>>> True and False
False
>>> 5 == 5
True
>>> x = 5
>>> x
5
>>> x = x + 1
>>> x
6
>>> 2 + 2
4
>>> this_is_a_ASDFASDFASFvar23145971234987iable =5
>>> this_is_a_ASDFASDFASFvar23145971234987iable
5
>>> 234asdf = 5
SyntaxError: invalid syntax
>>> True = 5
SyntaxError: can't assign to keyword
>>> if = 5
SyntaxError: invalid syntax
>>> print("hello")
hello
>>> "Hello 123!"
'Hello 123!'
>>> type("Hello 213!")
<class 'str'>
>>> 'hello!'
'hello!'
>>> x = 'hello!'
>>> print(x)
hello!
>>> print('Lawton's')
    
SyntaxError: invalid syntax
>>> print("Lawton's")
    
Lawton's
>>> print('Lawton\'s')
    
Lawton's
>>> print("""Lawton's"s""")
    
Lawton's"s
>>> print("asdf\nasdf)
    
SyntaxError: EOL while scanning string literal
>>> print("asdf\nasdf")
    
asdf
asdf
>>> print("asdf\tasdf")
    
asdf  asdf
>>> "asdf" + "jkl"
    
'asdfjkl'
>>> "asdf" * "jkl"
    
Traceback (most recent call last):
  File "<pyshell#27>", line 1, in <module>
    "asdf" * "jkl"
TypeError: can't multiply sequence by non-int of type 'str'
>>> "asdf" * 3
    
'asdfasdfasdf'
>>> 1 < 2
    
True
>>> "3.7" in "Python 3.7.0 Shell"
    
True
>>> "3.6" not in "Python 3.7.0 Shell"
    
True
>>> s = "python"
    
>>> s[0]
    
'p'
>>> s[1]
    
'y'
>>> s[10]
    
Traceback (most recent call last):
  File "<pyshell#35>", line 1, in <module>
    s[10]
IndexError: string index out of range
>>> s[-1]
    
'n'
>>> len("asdf")
    
4
>>> int(2.5)
    
2
>>> bool(0)
    
False
>>> bool(1)
    
True
>>> bool(12341234)
    
True
>>> 
 RESTART: /Users/lawtonnichols/Desktop/cs8/code-from-class/08-08/functions.py 
>>> square
    
<function square at 0x109957730>
>>> 
 RESTART: /Users/lawtonnichols/Desktop/cs8/code-from-class/08-08/functions.py 
16
>>> 
 RESTART: /Users/lawtonnichols/Desktop/cs8/code-from-class/08-08/functions.py 
None
>>> 
 RESTART: /Users/lawtonnichols/Desktop/cs8/code-from-class/08-08/functions.py 
16
>>> 
 RESTART: /Users/lawtonnichols/Desktop/cs8/code-from-class/08-08/functions.py 
16
>>> 
 RESTART: /Users/lawtonnichols/Desktop/cs8/code-from-class/08-08/functions.py 
16
>>> 
 RESTART: /Users/lawtonnichols/Desktop/cs8/code-from-class/08-08/functions.py 
25
>>> 
 RESTART: /Users/lawtonnichols/Desktop/cs8/code-from-class/08-08/functions.py 
49
>>> 
 RESTART: /Users/lawtonnichols/Desktop/cs8/code-from-class/08-08/functions.py 
49
1.999999987845058
>>> 
 RESTART: /Users/lawtonnichols/Desktop/cs8/code-from-class/08-08/functions.py 
49
2.00001000001393
>>> 
 RESTART: /Users/lawtonnichols/Desktop/cs8/code-from-class/08-08/functions.py 
49
1.999999987845058
3.999999975690116
>>> [1, 2, 3]
    
[1, 2, 3]
>>> type([1,2,3])
    
<class 'list'>
>>> l = [1,2,3]
    
>>> l
    
[1, 2, 3]
>>> [1,2,3] + [4,5,6]
    
[1, 2, 3, 4, 5, 6]
>>> 1 in [1,2,3]
    
True
>>> l
    
[1, 2, 3]
>>> l[0]
    
1
>>> l[-1]
    
3
>>> sum(l)
    
6
>>> l
    
[1, 2, 3]
>>> l[0] = 4
    
>>> l
    
[4, 2, 3]
>>> (1, 2, 3)
    
(1, 2, 3)
>>> type((1,2,3))
    
<class 'tuple'>
>>> (1,2,3) + (4,5,6)
    
(1, 2, 3, 4, 5, 6)
>>> t = (1,2,3)
    
>>> t[0]
    
1
>>> t[0] = 4
    
Traceback (most recent call last):
  File "<pyshell#61>", line 1, in <module>
    t[0] = 4
TypeError: 'tuple' object does not support item assignment
>>> sum(t)
    
6
>>> (1,2)
    
(1, 2)
>>> def id(x):
  return x

>>> id(5)
    
5
>>> 5 + 5
    
10
>>> id(5) + id(5)
    
10
>>> id(5) + id(5) + id(5)
    
15
>>> def id(x):
    print(x)
    return x

    
>>> id(5)
    
5
5
>>> id(5) + id(6) + id(7)
    
5
6
7
18
>>> id(5) + (id(6) + id(7))
    
5
6
7
18
>>> 2 ** 3 ** 4
    
2417851639229258349412352
>>> (2 ** 3) ** 4
    
4096
>>> 5 + 7 / 3
    
7.333333333333334
>>> id(5) + id(7) / id(3)
    
5
7
3
7.333333333333334
>>> id(5) + (id(7) / id(3))
    
5
7
3
7.333333333333334
>>> plus(id(5), divide(id(7), id(3)))
    
Traceback (most recent call last):
  File "<pyshell#83>", line 1, in <module>
    plus(id(5), divide(id(7), id(3)))
NameError: name 'plus' is not defined
>>> 2 + 3 + 4
    
9
>>> 2 ** (3 ** 4)
    
2417851639229258349412352
>>> 2 ** 3 ** 4
    
2417851639229258349412352
>>> def g(x):
    return x + 1

    
>>> 
    
>>> 
    
>>> 
```

Derivative/functions sample code:

<https://github.com/ucsb-cs8-m18/code-from-class/blob/master/08-08/functions.py>