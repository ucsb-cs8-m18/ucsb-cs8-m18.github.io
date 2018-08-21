---
layout: lab
num: lab03
ready: true
desc: "More functions with test cases"
assigned: 2018-08-16 11:00:00.00-7
due: 2018-08-24 18:30:00.00-7
submit_cs_pnum: 772
---

In this lab, you'll get more practice with

* Writing functions
* Testing function with pytest
* Submitting your functions and test cases to Gradescope

# Step 1: Verify that pytest is working on the machine where you plan to work.

You may choose to work on your own machine, or on a CSIL machine.  Either
way, you will need `pytest` installed.  

As in lab02, we check whether pytest is installed by doing the `import pytest` command
at the Python shell prompt.  If it returns no error message, then `pytest`
is installed.  If you get an error, refer back to
[lab02](/lab/lab02/) for instructions on installing it.

```
[cgaucho@csil-12 ~]$ python3
Python 3.4.3 (default, Aug 9 2016, 15:36:17) [GCC 5.3.1 20160406 (Red Hat 5.3.1-6)] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> import pytest
>>>
```

# Step 2: Make a `~/cs8/lab03` folder

The easiest way to create this is to do the following, which
will work from any directory:

`mkdir -p ~/cs8/lab03`

That form of the `mkdir` command, with the `-p` has the advantage that

* It creates the entire path of directories in case any of the intermediate
   ones don't exist (that is, it will create a `~/cs8` directory too if it
   isn't there yet)
* If the directory being create already exists, it won't complain
* Since the directory being created starts with `~`, it's an absolute
   path, and thus the command works regardless of the current directory.

Then, to get yourself into that directory, type:

`cd ~/cs8/lab03`

Again, since that's an absolute path, it works from any directory.

# Step 3: Create a file called `lab03.py` in your `~/cs8/lab03` directory

To start out lab03, write the line:

```
import pytest
```

Then, copy this function definition into your
lab03.py file.

```
def perimRect(length,width):
   """
   Compute perimiter of rectangle
   """
   return -42.0 # stub  @@@ replace this stub with the correct code @@@

   
```

Then, copy these function definitions into your file.  These are a special kind of function called a <em>test case</em>.  These particular test cases are written in the style used by the <em>pytest</em> testing framework, and they follow these rules:

1. The name of each test cases function must start with `test_` or end with `_test`.
2. Each one ends (typically) with a line of code that starts with the keyword `assert`, followed by a boolean expression.
   * If the expression is `True`, the test case <em>passes</em>
   * If the expression if `False`, the test case <em>fails</em>
3. Each test case function must have a different name (hence: `test_perimRect_1`, `test_perimRect_2`, `test_perimRect_3`, etc.)  They don't have to be consecutive numbers&mdash;we could use `_a`, `_b`, `_c` or anything really, as long as they are all different.

```

def test_perimRect_1():
   assert perimRect(4,5)==18

def test_perimRect_2():
   assert perimRect(7,3)==20

def test_perimRect_3():
   assert perimRect(2.1,4.3)==pytest.approx(12.8)

```

Finally, run the code, and ensure that you don't have any syntax errors
in your Python code.

# Step 4: Test your code by hand

Because I want to be sure that you continue to practice the skill,
test your code by hand first.

That is, select "Run Module" in IDLE, and then type in a few function calls
at the Python Shell Prompt.   Here are a few:

```
>>> perimRect(4,5)
-42.0
>>> perimRect(7,3)
-42.0
>>> 
```

Ok, so that's sort of pointless as long as we haven't fixed the function yet.  The point
is that
* you need to know how to check the value of a function call by typing it in.
* you need to see that right now, the function *always* returns -42.0, no matter what.

There is a reason for that.  We call this a "stub value".  It returns the wrong answer
*on purpose* so that we can check that all of the tests fail.   We want to see all of
the tests fail, THEN see all of the tests pass.  That's the general idea.

* We want so see them *all fail* when the function is wrong
* Then if they *pass* when the function is right, we *trust* the test.

# Step 5: Run pytest on the file so far

As a reminder, you run pytest OUTSIDE of idle, at the regular terminal
prompt.

You may find it helpful to bring up a second terminal window and use

```
cd ~/cs8/lab03
```

to get into the correct directory.  Then use:

```
python3 -m pytest lab03.py
```

You should see three test failures. If you do, then you ready to fix the code so that it works, which is the next step.

(If you need a refresher on how to interpret
the output of `pytest`, refer back to [lab02](/lab/lab02/])


# Step 6: Fixing the code for `perimRect`

So, if you have failing test cases, the thing to do is fix the code so
that the test cases pass.

Of course the formula for the perimiter of a rectangle with length $$ l $$ and width $$ w $$ is, in math notation: $$ p = 2l + 2w $$.   But you'll have to convert that into Python, and use the variables `length` and `width` to get it to work properly.   

Once you have the code correct, try testing both using interactive testing as well as by running `pytest`.

# Step 7: Read these instructions about how the rest of the lab will work

In each of the steps that remain, you will add an additional function definition,
and some test cases.

You should try to make the function pass the test cases that you put in.

In some cases you'll be given the test cases.  In other cases, you have to supply
these test cases yourself.

At each step, you should first try to get the test cases to pass by running
pytest at the Unix command line as shown.

* Please do this BEFORE submitting to Gradescope
* Please DO NOT submit to Gradescope without testing locally first
* You can submit to Gradescope to see partial progress, but only if you have function definitions for `perimRect`, `areaRect`, `isString`, and `isNumber`. If you want to submit your work to Gradescope to see partial points, please make functions with those names (they can return silly things, like 42 or something, if you haven't started them yet. Just as long as they're there the autograder won't complain.)

If you do, proceed to the next function definition and set of test cases.

If you pass your own tests, but NOT the instructor supplied tests, then try to
see if you can figure out why.  Is there some case that you did not consider?
The problems may have hints.

You can also ask questions on Piazza. This is a good situation to use a "private
post" to the instructors.  We can see your submissions on Gradescope,
so you don't have to share your code with us--just tell us your name, which lab you are
working on, and which step you need a hint for with instructor tests not passing.

Once you understand all how this is going to work, you are ready to start coding
the additional functions.

# Step 8: Write an `areaRect` function and some test cases for it

Now, add the definition of a function called `areaRect`.

It should have two parameters, length and width, and return the area.

Although it is tempting to write the function correctly from the start,
since the definition is SO easy, I encourage you to follow the practice
of initially putting in a stub such as the following, so that you can
"test the test":

```
   return -999
```

In addition, define three test cases.

The code for the first two test cases should look like this:

```

def test_areaRect_1():
   assert areaRect(3,4)==12

def test_areaRect_2():
   assert areaRect(0.5,0.4)==pytest.approx(0.2)


```

The third test case should be one that you come up with yourself. The restrictions are that it must be:

* a function called `test_areaRect_3`
* it should have an `assert` statement
* the assert keyword should be followed by a call to `areaRect` with some other argument values, different from the ones in the first two test cases, followed by a test for equality operator `==`, and the value that you expect `areaRect` to return for those argument values

Please write this third test case.

Then:

* test your code with "Run Module" to make sure it compiles ok (i.e. no red error messages)
* use `python3 -m pytest lab03.py -k areaRect` to run just the test cases for the `areaRect` function (there should be three of them, and three skipped test cases)
* they should all fail (because you have a stub value, -999)
* finally, replace the code in the function definition for areaRect with the correct code, and see all the tests pass.


# Step 9: Write an `isString` function and some test cases for it

Here is an example of a function that tests whether something is a list or not.


```
def isList(x):
   """
   returns True if argument is of type list, otherwise False
   """
   
   return ( type(x) == list )   # True if the type of x is a list
```

Your job is to write a similar function that takes a parameter `x` and returns
`True` if `x` is a string (type `str` in Python), and returns `False` if it is
not a string.

Here's a stub for that function.  Add it into your lab03.py file.

```
def isString(x):
   """
   returns True if argument is of type str, otherwise False
   """
   
   return "stub" 


```

And here are three test cases. Add those also:

```
def test_isString_1():
   assert isString("UCSB")

def test_isString_2():
   assert not isString(42)

def test_isString_3():
   assert not isString(["UCSB"])
```

Then, add two more test cases, following the examples above. Those
test cases should be functions named `test_isString_4` and
`test_isString_5`.  One of those should check something that you think
*is* a string, and one more that you think checks something that is
*NOT* a string.   Try to come up with different test cases than the ones given.

Finally, go through all the same steps that you did before:

* make sure the file compiles ok
* test with `pytest` and see the tests fail
* fix the function and see the `pytest` tests pass

As a reminder, you can use `-k blah` to run only the tests that have `blah` in their name&mdash;for example, for this step, you'd use:

```
python3 -m pytest lab03.py -k isString
```


# Step 10: Write an `isNumber` function and some test cases for it

Our last function is one called `isNumber` that should take a parameter `x` and return
`True` if the value `x` refers to is either of type `int` or of type `float`.  In any other case, it should return `False`.

You should write the function definition, and you should write exactly five test cases,
with function names:

* `test_isNumber_1`
* `test_isNumber_2`
* `test_isNumber_3`
* `test_isNumber_4`
* `test_isNumber_5`

Follow the model from earlier.

Test your code with:

```
python3 -m pytest lab03.py -k isNumber
```

Then test your code by submitting to Gradescope.

# Step 11: See each test passing on Gradescope; profit.

At this point, you should see that you have a full score for each test on Gradescope. I have some hidden tests that are being run, so you won't see your full grade until after the deadline passes.

