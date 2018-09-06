---
num: "Lecture 14"
desc: "Stacks, recursion"
ready: true
date: 2018-09-06 09:30:00.00-7:00
---

# Code from class

<https://github.com/ucsb-cs8-m18/code-from-class/tree/master/09-06>

---

lab06 is due Saturday, because why not

I added some topics to the final webpage, but it's nothing you wouldn't have found yourself in the homework/lab descriptions and lecture notes

---

iClicker Questions
==================

```
0. What does f(3) return?

   def f(x):
     if x == 0 or x == 1:
       return 1
     else:
       return f(x-1) + f(x-2)

  (a) 1
  (b) 2
  (c) 3
  (d) None of the above
```

Schedule of Events
==================

- stacks, push and pop (starts at __main__)
  - <https://www.cs.ucsb.edu/~pconrad/cs8/topics.beta/theStack/>
- raising your own exceptions and pytest-ing them (lab07, largestInt and tests):
    ```
    def test_largestInt_01():
      with pytest.raises(ValueError):
        result = largestInt("not a list")
    ```
- recursion ([slides are here](/lectures/Lecture15_Recursion.pdf))
- lab06, hasAnE, tupleContainingStringsOfLength3 examples