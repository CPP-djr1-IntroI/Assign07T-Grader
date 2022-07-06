## Intro to C++ I

# Assign07-Grader

**Goals:**

1. Use parallel arrays to solve a problem

2. Continue coding using well-defined functions

3.  Write one function at a time and test before going on

4.  Reuse existing functions as much as possible

## Problem

The results of a true-false Quiz given to a Computer Science class over
the Web have been saved in a file called: **quiz.txt**. The information
available for each student consists of a student identification number
and the student's answers for up to 25 true-false questions. The first
line of data consists of the number of true-false answers followed
by the actual answers to the Quiz where a 1 stands for true and 0 stands
for false. Each subsequent line contains a student ID number and the
student\'s answers to the Quiz. There are an unknown number of students
in the datafile and at most 25 questions.

You are to write a C++ program that will print information for each
student shown below.

The following is a sample datafile that might be used in your program:

<pre>
10 0 1 0 0 1 0 0 1 0 1
1080 0 1 1 0 1 0 1 1 0 1
1340 0 1 0 1 0 1 1 1 0 0
1462 1 1 0 1 1 1 0 0 1 0
1512 1 0 1 0 1 0 1 0 1 0
1341 0 1 1 0 1 1 1 1 1 1
1401 1 1 0 0 1 0 0 1 1 1
1463 1 1 1 1 1 1 1 1 1 1
1464 0 1 0 0 1 0 0 1 0 1
</pre>

Your output must look exactly like the following:

<pre>
STUDENT ID: 1080   	  GRADE: 80.0
                	  1  2  3  4  5  6  7  8  9 10
CORRECT ANSWERS:	  0  1  0  0  1  0  0  1  0  1
YOUR ANSWERS:		  0  1  1  0  1  0  1  1  0  1
--------------------------------------------------

STUDENT ID: 1340   	  GRADE: 50.0
                	  1  2  3  4  5  6  7  8  9 10
CORRECT ANSWERS:	  0  1  0  0  1  0  0  1  0  1
YOUR ANSWERS:		  0  1  0  1  0  1  1  1  0  0
--------------------------------------------------
and so on

--------------------------------------------------
SUMMARY STATISTICS

                	  1  2  3  4  5  6  7  8  9 10
TOTAL CLASS MISSED:	  X  X  X  X  X  X  X  X  X  X

CLASS AVERAGE:        XX.XX
</pre>


## Notes

1.  Minimally, a data file must consist of at least the first line of
    true/false answers.
2.  I will run your program on the test data supplied and few more
    files, so make sure you test all border cases.
3.  Save all output to a file called **graderresults.txt**. No output
    should go to the screen.

Challenge

Provide a histogram of
the class scores. The histogram information must be maintained in an
array as you go through and grade the quizzes. Then after the CLASS
AVERAGE is printed out above, print out a histogram as shown below. The
range of scores is inclusive of the score on the left but exclusive of
the score on the right. As an example, 30-40 means >= 30 and < 40,
EXCEPT 90-100 which is \>=90 and \<= 100.

<pre>
--------------------------------------------------
HISTOGRAM
SCORES:
 00-10: *
 10-20: 
 20-30:
 30-40: *
 40-50: **
 50-60: *
 60-70: **
 70-80: *****
 80-90: ****
90-100: **
--------------------------------------------------
</pre>


**To complete this assignment you must submit the following:**

1.  **An electronic Solution of your program on GitHub**

    a.  You are to click on the Assign07 Link to accept this
        assignment as we've done in lab. Once accepted, code up a
        complete solution to the above assignment specification. Your
        complete solution is to be pushed to GitHub no later than the
        date and time specified above for your specific section. I will
        only grade your solution from the proper location on GitHub.

    b.  Pay attention to the example output above. Your program's output
        must look **exactly** like the example output! The spacing and
        newlines in your output must match exactly.

    c.  Make sure that your program compiles and runs correctly with no
        errors and no warnings. If you get any errors, double check that
        you typed everything correctly. Be aware that C++ is
        case-sensitive.

2.   **An electronic copy of your program (punetidAssign07Grader.pdf) is 
to be emailed to ryandj@pacificu.edu**
