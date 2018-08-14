---
num: "Lecture 4"
desc: "if/else, for, input"
ready: true
date: 2018-08-14 09:30:00.00-7:00
---

# Code from class

<https://github.com/ucsb-cs8-m18/code-from-class/tree/master/08-14>

Python round function: <https://docs.python.org/3.7/library/functions.html#round>

# Logging into CSIL from MacOS or Linux

```
ssh -X pconrad@csil-21.cs.ucsb.edu
```

The first time you'll get a message such as:

```
ECDSA key fingerprint is SHA256:ANJ7ced3JXpxKnu8OhnS3f8Z0rE9aIKA+eHHgVlEzVc.
Are you sure you want to continue connecting (yes/no)? yes
```

Just say yes.

Machines are 01-48

CTRL/D can be used to exit.


For Windows, the program is MobaXTerm

To use it, look for "New Session" in upper left,

Then "ssh" upper left.

Then enter `csil-15.cs.ucsb.edu` (or whatever number)
where it asks for host.

Then, you'll be prompted for username and password.

# If you get this message when running `idle3`

or any other program that needs graphics...

```
_tkinter.TclError: no display name and no $DISPLAY environment variable
```

On Windows: Use MobaXTerm instead of a program such as PuTTY.

On Mac: You need to install XQuartz ... go to XQuartz.org, download, follow instructions, and try again.

Also: on Mac or Linux, maybe you forgot the -X part. If that still doesn't work, see me and I'll follow the instructions on this page with you: <https://stackoverflow.com/questions/39622173/cant-run-ssh-x-on-macos-sierra>.

---

# Installing pytest

Mac:

One of the following will work:
```
pip3 install pytest
python3 -m pip install pytest
```

Windows:

open command prompt, and type:
```
python -m pip install pytest
```
If that doesn't work, you'll need to add python to your PATH using this: <https://projects.raspberrypi.org/en/projects/using-pip-on-windows/5>

---

When you use SSH, you connect to another computer. Changes you make to the files on that computer don't appear on your own computer.

---

The line "import blah" asks Python to look for a file named blah.py. So don't name your Python program "turtle.py", because then "import turtle" won't find the correct module.

---

iClicker Questions
==================

0. What does the following code print out?

    x = 5
    if x < 7:
        print(x)
        x = x + 7
    else:
        print(x)
        x = x - 7
    if x < 7:
        print(x)

    (a) 5
        12
        5

    (b) 5
        12

    (c) 5

    (d) None of the above

1. How many things are wrong with the following code? It's supposed to print out "0\n1\n2\n3\n4\n5\n6", where each \n is a new line.
    
    for i in range(10):
        if i < 7:
            print(i)

    (a) 0
    (b) 1
    (c) 2
    (d) ≥ 3

In-Class Questions
==================

0. Write a program that takes a price input from the user, adds 7.75% tax to it, and then outputs the new price.

1. Write a function called calculate_grade that takes in a percentage, and prints a string:
   That string should be "pass" if the percentage is ≥ 60, and "fail" if it's smaller than 60.

2. Change the function to return the string instead of printing it.