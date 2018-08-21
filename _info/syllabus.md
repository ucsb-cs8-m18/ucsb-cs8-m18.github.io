---
title: "Syllabus, CMPSC 8, Summer 2018"
layout: handout
ready: false
---

Basic Facts
-----------

* **Course Web Site**: <http://ucsb-cs8-m18.github.io>
* **Instructor**:  Lawton Nichols
   * Email is lawtonnichols [at] cs [dot] ucsb [dot] edu, but please use Piazza for course-related communication.
* **Lecture**: TWR  9:30 am – 10:50am, Psych 1924, ATTENDANCE REQUIRED.
* **TAs**: {{site.ta_list_full}} (contact via Piazza.com)
* **Lab** Thursdays at either 11, 12:30, 2, or 3:30, Phelps 3525, ATTENDANCE REQUIRED.                                         
* **Office Hours**: 
  - Lawton: Tuesdays 11:00am–1:00pm, Trailer 936
  - Yun: Wednesdays 8:00am–9:00am, Bioengineering 3205
  - Harmeet: Wednesdays 4:00pm–5:00pm, CSIL
  - Muqsit: Thursdays 5:00pm–6:00pm, Trailer 936
* **Textbook**: Perkovic - Introduction to Computing Using Python: An Application Development Focus (2nd Edition)
* **Piazza Sign-up Page**: <https://piazza.com/ucsb/summer2018/cs8nichols>
* **Gradescope**: Go to <https://gradescope.com/>, and create a student account with entry code **9DJJKG**. Make sure your name is exactly as it appears in GOLD.

Trailer 936 location:<br />
![Trailer 936 location](/images/936.png)

Official UCSB Catalog Description
---------------------------------

<div style="background-color:#eee; border: 8px inset #333; font-size:90%; margin:1em; width:45em; padding: 0.5em;" markdown="1">

CMPSC 8: Introduction to Computer Science

Not open for credit to students who have completed Computer Science 16 or Engineering 3.

Introduction to computer program development for students with little to no programming experience. Basic programming concepts, variables and expressions, data and control structures, algorithms, debugging, program design, and documentation.

</div>


## A Few Course Policies In Brief

* If you are registered for another UCSB course  that overlaps with this one, you MUST HAVE specific written permission from both instructors, or I am within my rights to give you a failing grade on any work you miss as a result, and will NOT make any accommodations for you.  This includes exams.
* You are permitted one sheet of notes on exams—details later on the syllabus.
* Collaboration is only permitted when specifically allowed for—otherwise, you must do your own work.
   * On most homework assignments  you may collaborate with at most one other person (who must be named).
* Attendance is required at all lectures and labs (discussion sections)
   * You may not turn in homework on behalf of another student, or ask someone else to turn in yours.
   * I recognize that some absences (e.g. minor illnesses, mishaps, etc.) are unavoidable.  Litigating whether each of these is "excused" or not isn't a good use of anyone's time, so instead we just drop the lowest grade from everyone's homework grades.  In this way, absenses (or failure to turn in homework) does not unduly penalize your grade unless it becomes excessive.

You may NOT: 

* Have someone else turn in your homework for you (that will be considered academic dishonesty).
* Leave homework in a mailbox or slide it under a door
* Drop it off with the instructor to be graded later.

## What this course is about 

This course is an introduction to Computer Science, and programming. 

Computer Science is the study of <strong>abstractions </strong>and <strong>algorithms</strong>. 

* In Computer Science, an <strong>abstraction</strong> is a useful representation of something from the real world that allows us to work with it more easily or efficiently.

* An <strong>algorithm</strong> is a well-defined, step-by-step sequence of instructions that can be used to mechanically determine the solution to some well-defined problem.

You probably use <strong>abstractions</strong> and <strong>algorithms</strong> every day—for example:

* If you pick up any textbook, you'll probably find an index in the back of the book. The index is an <strong>abstraction</strong>—whether the book is about biology, modern art, political science, or computers, the &quot;way the index works&quot; is the always the same. It is composed of the same pieces (topics and page numbers), and organized in the same way (alphabetically by topic, then lists of page numbers in numerical order from smallest to largest.)

* If you are looking in the index of a U.S. history textbook for &quot;Gettysburg&quot; you'll probably use an <strong>algorithm</strong> to find the entry quickly. Here the input to the algorithm is some topic, and the output is a list of pages on which that topic appears.

* If you are looking for a parking lot on campus, you might use an <strong>abstraction</strong> called a &quot;map&quot; to locate the parking lot. You know the features of a map, and how it corresponds to the reality of a college campus, and parking spaces. The way a map can work to help you find a parking lot (or garage) is the same whether it's a map of UCSB, Downtown Santa Barbara, or the Staples Center in LA.

* If you are searching through a parking lot (or garage) to either (a) find a parking space, or (b) determine that there are no spaces left, you probably use an <strong>algorithm</strong> to do that—again, without even thinking about what you are doing.


## Algorithms have to be both designed, and &quot;coded&quot; so the computer can carry them out 

In the case of using an index, this is probably an algorithm you may have learned in grade school, and it has been so long since you learned it, that now you don't even think about it—you just do it. Finding a space in a parking lot—and knowing when to give up and look elsewhere—is &quot;just common sense&quot;; this probably isn't something you were ever &quot;taught&quot;, or even have to think very much about. You just do it.

Computers don't currently have this capability—i.e. the capability to &quot;pick up things by common sense&quot;—and it seems unlikely that they  will within our lifetime—unless there are major breakthroughs in the field of Artificial Intelligence. Such breakthroughs have been predicted for a while, but they haven't happened yet. (Maybe you'll be the one to figure out how to achieve this!)

So, for the time being at least, it falls to humans to design algorithms that computers can use to solve problems. In many cases, these algorithms are &quot;just common sense&quot;—the computer equivalent of looking for an empty parking space in a parking lot (and knowing when to give up). Algorithms like this are easy to design. Many of the algorithms we'll see in this course are like that.

In other cases, the algorithms are very complex, or very subtle, and coming up with them is a deep intellectual challenge. Furthermore, the impact of a better algorithm on society can be very large. For example, new algorithms in the field of computational science—modeling chemical and biological reactions with computer simulations—can lead to breakthroughs such as new drugs to fight disease, or renewable sources of energy.

And often, what goes along with finding a good algorithm is finding a good abstraction of the real world concepts we are interested in: cells, molecules, oil fields, words, sentences, students, courses, GPAs, etc. Algorithms and abstractions really go hand-in-hand.

## Coding, or Writing Software, or Programming

Coding is expressing algorithms in a programming language.

Human languages such as English and Spanish are not very well suited for expressing algorithms—at least not for expressing them to a computer (they have their problems for communicating with humans too!). So, special languages are used. In this course, we'll learn the Python programming language. We choose Python rather than Java or C++ because:

* If you are learning your first programming language, Python is easier to learn than the others
* Learning Python provides a good foundation for learning C, C++ or Java
* If you only learn one programming language, Python is a good choice—in spite of being easy to learn, it is not a &quot;toy&quot; language by any means. It is widely used by scientists and web application developers just for starters. Many internal systems at Google are based on Python code.
 
This course provides you with the opportunity to become a pretty good beginning programmer, and be well prepared for an intermediate programming course such as CS16 (the first course that counts towards the CS major at UCSB, and which requires at least one quarter of prior programming experience.)

I say that the course &quot;provides an opportunity,&quot; because you will only become a good beginning-level programmer if <strong>you</strong> put a lot of time and effort into this course—that is true no matter how much thought and attention I put in my lectures, assignments, and exams

## The swimming/guitar/painting analogy

You cannot learn to swim, play guitar, or paint from a textbook or a lecture. You can only:

* learn  to swim by spending many hours in the pool
* learn to play guitar by spending many hours playing the instrument
* learn to paint by spending many hours putting brush to canvas

The same is true of programming. Programming is not a series of facts to be memorized—you cannot &quot;cram&quot; for a computer science exam. You must practice, practice, practice.

<div style="page-break-before:always;">
&nbsp;
</div>

# What you need to learn to become <br />a skilled beginning level programmer


So, what is it that you need to know to be a skilled beginning-level programmer in Python? Here's the  list of what you'll need to be ready for CMPSC&nbsp;16 (aka CS16, the next programming course):

<table border="1" cellspacing="1" cellpadding="1" id="topicTable">
  <tr>
    <td><ul class="style11">
      <li>Problem solving
        <ul>
            <li>breaking down a problem into a sequence of steps</li>
          <li>abstracting specific problems into general ones<br />
            and finding general solutions</li>
        </ul>
      </li>
      <li>Memory concepts
        <ul>
            <li>variables, primitive vs. reference variables, name, type, value</li>
          <li>assignment statements</li>
          <li>scope of variables</li>
        </ul>
      </li>
      <li>Control structures
        <ul>
            <li>for loops, if/else, while loops</li>
        </ul>
      </li>
      <li>Lists in Python (similar to arrays in other languages)
        <ul>
            <li>index vs. value, finding sum, min, max, average, count of elements matching some condition, making a new list of elements containing only those that match some condition</li>
        </ul>
      </li>
    </ul>    </td>
    <td><ul class="style11">
      <li>Functions
        <ul>
            <li>function call vs. function definition</li>
          <li>formal vs. actual parameters (arguments)</li>
        </ul>
      </li>
      <li>Testing
        <ul>
            <li>How to test your code</li>
        </ul>
      </li>
      <li>Input/output concepts
        <ul>
            <li>Writing to the terminal</li>
          <li>Reading from the keyboard</li>
          <li>Reading and writing to files</li>
          <li>Neatly formatting output</li>
        </ul>
      </li>
      <li>Program style
        <ul>
            <li>How to write code that other people can read and understand</li>
        </ul>
      </li>
    </ul>    </td>
  </tr>
</table>



Final Course Grades
===================

The formula to determine your course grade average is explained in the table below.

Regardless of any other policies spelled out here, the average used to determine your final letter grade may be no higher than one full letter grade higher than your exam average.

Thus,

-   reasonably good performance on exams is very important to earning a good final grade in the course.
-   an A or B should not be out of reach for anyone that has a reasonably good mastery of course concepts (enough to earn a B or C on the exams), and puts in hard work on the labs and homeworks.

To convert final averages to letter grades, a standard 10 point scale will be used, with the upper and lower ends of each range as +/- grades, except
for A+ grades, see below.  There is no "rounding up"; a grade of 86.9999 is a B and a grade of 87.0000 is a B+.

| Grade Item                | Percentage of Final Grade |
|---------------------------|---------------------------|
| Midterm     | 25 %                      |
| Final       | 30 %                      |
| Labs | 25 % |
| Hwks | 18 % |
| iClicker | 2%  |

## Grade assignment policy
<table border="2">
  <tr>
    <td>A+</td>
    <td>97-100</td>
    <td>A</td>
    <td>93-97</td>
    <td>A-</td>
    <td>90-93</td>
  </tr>
  <tr>
    <td>B+</td>
    <td>87-90</td>
    <td>B</td>
    <td>83-87</td>
    <td>B-</td>
    <td>80-83</td>
  </tr>
  <tr>
    <td>C+</td>
    <td>77-80</td>
    <td>C</td>
    <td>73-77</td>
    <td>C-</td>
    <td>70-73</td>

  </tr>
  <tr>
    <td>D+</td>
    <td>67-70</td>
    <td>D</td>
    <td>63-67</td>
    <td>D-</td>
    <td>60-63</td>

  </tr>
    <td>F</td>
    <td>Below 60</td>

</table>
<p><strong>Curving: </strong>The grade  scale above represents the <em>minimum</em> letter grade you will be assigned—at the instructor's discretion, the grading scale  may be altered <em>in the students' favor</em> if this will be better reflect the students' mastery of the material. Thus, <em>if</em> there is a "curve", it will be applied at the <em>end</em>, not to individual assignments.</p>
<p><strong>A+ grades: </strong>These may be awarded to the very best performing students in the class—but the cutoff for A+ grades will be determined at the end of the course at the discretion of the instructor (there is no pre-determined cutoff---an average of 97 or more doesn't guarantee you an A+ grade.)</p>



<div style="page-break-before:always;">
&nbsp;
</div>



Attendance
==========

This course moves quickly. So attendance is very important.  This is even more true in the summer.

Missing homework: Drop the lowest one
-------------------------------------------------------

I will
drop the lowest homework grade (which may be
zeros if you miss an assignment.) Each homework
will be of equal weight, regardless of the total points 
listed on the assignment.

Homework grading
----------------

There are a lot of students in this class and very few TAs, so there's a very good possibility that the TAs won't be able to grade the entirety of your homeworks without going over their 20-hours-a-week work limit. If that happens, the TAs will randomly pick a subset of questions to grade for the homework, grade only those, and your grade for that homework will be (graded questions score / points possible on the graded questions).

Notes sheets on exams
---------------------

-   You are permitted one HANDWRITTEN 8.5 x 11 (standard US letter size paper) sheet of notes for each exam.
-   You are permitted only one sheet per exam.
-   Your notes sheet will be collected and WILL NOT BE RETURNED
-   So, if you need a copy of it, make a copy BEFORE you come to the exam.

<!--Questions about grades
----------------------

**Summary: regrade requests must be made only on GradeScope, and always within one week.**

From time to time, the people who grade your papers may make clerical
errors in grading (e.g. adding up points wrong or applying a rubric
incorrectly.) For this reason, you are encouraged to review your
grades as they are posted to Gradescope and Gauchospace. You will
typically get an email as soon as each grade is posted. From the time
the grade is posted, you will have one calendar week to post regrade
requests. These must be made ONLY through Gradescope, ON the correct
problem. (Don't request a regrade for question 4 on the page for
question 7.)

Please note that <b>regrade requests based on clerical errors or
applying a rubric incorrectly are always welcome</b>. Over the course
of the quarter, we'll grade over 10,000 individual problems, so it is
unlikely that we won't make at least some mistakes.

<b>More problematic are challenges to the rubric itself</b>, e.g. "I
don't think you should have taken off so many points for that error"
or "I think I deserve more partial credit for that incorrect
answer". The instructor and TA will always listen, but please know
that we've put a great deal of thought, time and experience into
determining the rubric, and we've done our best to apply it to all
students equitably. You may have a different point of view, we will
not always agree with your assessment—in fact, we seldom will. <b>As
such, regrade requests on this basis are not encouraged.</b> It is
important to approach such conversations in a respectful manner,
accepting that the instructor, TA and grader have been given
responsibility for determining course standards, and applying those in
a fair way to all students.

In any case, once the two week deadline for challenges has passed,
each grade becomes final---and it is your responsibility to come to
scheduled TA or instructor office hours to have this discussion. If
you cannot make office hours, you may request an appointment, but you
must request the appointment within ONE WEEK of the assignment being
posted. If you wait until the last office hours opportunity during the
two week window, and you are not able to be seen (e.g. because of a
long line of students), then you lose the right to appeal your grade.
-->

<div style="page-break-before:always;">
&nbsp;
</div>


Late Labs
---------

The policy is simple, and is based on the idea that the primary
purpose of the deadlines is to allow the TA manage his/her
workload. The number of labs in this course requires that he/she not
have to do "context switching" between grading different labs. All
labs must be graded in one sitting, or he/she just won't be able to
keep up with the workload.

So:

-   If you want your work to be graded without penalty, turn it in on time.
-   If you turn in your lab late, you RISK GETTING A ZERO.
-   We will grade late labs ONLY if it creates no extra inconvenience for the graders, and we WILL impose a penalty between 10-20% (see the individual grading rubrics for the labs.)
-   There is NO GUARANTEE that late labs will be graded at all. The TA will simply start work at some point after the deadline, and grade until he/she is finished. At that time, he/she will "close the books" on that particular lab, and any work not submitted at that time will NOT be considered.

Accommodations for disabilities
-------------------------------

Students with disabilities may request academic accommodations for exams online through the UCSB Disabled Students Program at http://dsp.sa.ucsb.edu/. Please make your requests for exam accommodations through the online system as early in the quarter as possible to ensure proper arrangement.

Managing stress
---------------

Personal concerns such as stress, anxiety, relationships, depression, cultural differences, can interfere with the ability of students to succeed and thrive. For helpful resources, please contact UCSB Counseling & Psychological Services (CAPS) at 805-893-4411 or visit <http://caps.sa.ucsb.edu/> .

Responsible scholarship
-----------------------

Honesty and integrity in all academic work is essential for a valuable educational experience.  The Office of Judicial Affairs has policies, tips, and resources for proper citation use, recognizing actions considered to be cheating or other forms of academic theft, and students’ responsibilities, available on their website at: http://judicialaffairs.sa.ucsb.edu.  Students are responsible for educating themselves on the policies and to abide by them.

Furthermore, for general academic support, students are encouraged to visit Campus Learning Assistance Services (CLAS) early and often. CLAS offers instructional groups, drop-in tutoring, writing and ESL services, skills workshops and one-on-one consultations. CLAS is located on the third floor of the Student Resource Building, or visit http://clas.sa.ucsb.edu


<div style="page-break-before:always" markdown="1">

![Python cartoon](https://foo.cs.ucsb.edu/8wiki/LocalImages/python.jpg)

(Image credit: [Randall Munroe](http://xkcd.com/353/))

Standard Disclaimer
-------------------

This syllabus is as accurate as possible, but is subject to change at
the instructor's discretion, within the bounds of UC policy.

(end of syllabus)

</div>


