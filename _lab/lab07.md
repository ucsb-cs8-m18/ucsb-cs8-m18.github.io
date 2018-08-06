---
layout: lab
num: lab07
ready: true
desc: "min/max, index vs. value"
assigned: 2018-09-06 11:00:00.00-7
due: 2018-09-13 18:30:00.00-7
submit_cs_pnum: 780
---

# THE DEADLINE FOR THIS ASSIGNMENT IS STRICT.

At the due date/time listed, submissions will be disabled, and whatever you have submitted by that time will be your final submission for this lab.

NO EXCEPTIONS except for true medical/family emergencies with
documentation from the Office of Student Life.  You are being told NOW to get started and not to put off
work on this assignment.


# You may pair or work alone on this lab.

# Instructions

This lab proceeds in an identical fashion to lab06.  The topics are different,
but the way of working is the same.

For this lab, you will create two files:

* `lab07.py`, a file containing some function definitions
* `lab07_tests.py`, a file containing some test cases

There is starter code for each of these (.py files) at the following link:

* <https://github.com/ucsb-cs8-m18/lab07-starter-code>

I suggest you proceed as follows:

1.  Create a directory called ~/cs8/lab07 (using the `mkdir` command) and `cd` into that directory.
2.  Use `idle3` (you might try `idle3 &` if you want to keep your prompt handy) to bring up idle3.
3.  Use "New File" to create empty files called `lab07.py` and `lab07_tests.py` in that `~/cs8/lab07` directory.
4.  ONE AT A TIME, copy the function definitions from the starter code, and the tests that go along with those, and get the tests to pass.
   * By one a a time, what I mean is, at your first step, copy ONLY the first function definition from  the starter code `lab07.py` and copy only the test cases from `lab07_tests.py` that go with that function definition.
   * Then, before you move on to the next function definition and <em>its</em> tests, get all of the tests from the one you just copied to pass.
   * Then, and only then, copy the next function definition and its tests into your files.
   * Repeat this until you have ALL of the function definitions and their tests, and all of them pass.
   
Note that what you are given differs from function to function: either a complete function definitions 
* In some cases you are given a function definition that is complete, but contains a bug.  In this case, you 
   need to fix the function definition.
* In some cases you are given a function definition that is correct. In this case, the code is there for you as an example&mdash;it is code that may be helpful to you in writing the other function definitions in the lab.   There is nothing you need to do other than study the code to learn how it works.
* In some cases, you are given a stub.

When you've done that, you are ready to try submitting to Gradescope for a final grade.  HOWEVER, you are encouraged to try submitting to Gradescope earlier, for several reasons:

* You can get partial credit if some of your tests pass for some of your functions
* You will have a backup of your file in case you accidentally delete yours from CSIL, or in case your laptop dies
* You can move code between your laptop and CSIL by downloading your code from the Gradescope submission
* You can ask the instructor or TA questions about your code on Piazza in a private instructor post.

# A Useful tip

As you know, this Unix shell command runs the tests in lab07_tests.py

```
python3 -m pytest lab07_tests.py
```

If you have LOTS of tests in your file, and you ONLY want to run some of them, you can use `-k string` to run ONLY the tests that contain a certain string.  For example, suppose you want to focus ONLY on the tests for `isList`.  You can run:

```
python3 -m pytest lab07_tests.py -k isList
```

Change `isList` to any function that you want, and only the tests that contain that string will be run.  The others will be "de-selected".


# Submission

### Navigate to the page for submitting {{page.num}}

Navigate to that page, and upload your `{{page.num}}.py` file.

