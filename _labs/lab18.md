---
title: "Lab 18"
description: "Linear Recursion in Python"
due: "Thursday, April 23rd, 11:59PM"
gradescope_assignment_id:
submission_files:
---

# Lab 18: Linear Recursion in Python

## Instructions
This worksheet serves as a guide and set of instructions to complete the lab. 

- You must use the starter file, [found here](https://drive.google.com/file/d/1ft08tsnakq7pRxhBPSLI8mhlAcKtVBVc/view?usp=drive_link), to get credit for the lab.
- There is no workbook for this lab. Review the [Lab 8 workbook](https://cs10.org/bjc-r/llab/html/topic.html?topic=berkeley_bjc%2Frecur%2Frecursive-reporters-part1.topic&course&novideo&noreading&noassignment) for review on recursive functions

## Notes
- **<ins>All functions for this lab must use recursion</ins>**

## Submitting:
You will need to complete **<ins>Exercises 1-3</ins>** and submit this to Gradescope. 
- To receive full credit, you will need to complete the required functions, and the required functions must pass all tests from the autograder in Gradescope.
- For instructions on how to submit labs to Gradescope, please see [this page](https://docs.google.com/document/d/1XAcZc9ypX07-bt0gK6uQ4P-06SrjPRsgiOjERIOlvYU/edit?usp=sharing).

Please note, you must use the [starter file](https://drive.google.com/file/d/1ft08tsnakq7pRxhBPSLI8mhlAcKtVBVc/view?usp=drive_link), and you must NOT edit the name of any of the required functions. Failing to do either for these will result in the autograder failing.

## Running Doctests:
To run doctests embedded within the docstring of a function, you can use the command `python3 -m doctest -v <file_name>.py`

To run all doctests you can run `python3 -m doctest <file_name>.py`

## Objectives:
Recursion is arguably the second most important topic in this course (after abstraction of course). You’ve seen and worked with many examples of recursion in Snap, although it’s time we practice in Python. In today’s lab you will implement what you know about recursion into Python functions.  By the end of the lab, you will:
- Understand how to implement linear recursion in Python
- Practice planning and coding recursive functions.
- Implement higher order functions in non iterative solutions

## Required Functions:
- Function 1: sum_digits(num)
- Function 2: gcd(a, b)
- Function 3: decimal_to_binary(n)

---

## Exercise 1: sum_digits(num)

**Objective**
Create a function that separates each digit of the input and then sums the digits together

**Notes**
- Use modular arithmetic (% 10) to attain the last digit of a number
- Use floor division (// 10) to strip the number of the last digit

**Inputs**
- num = some integer
  - The number to be recursively called

**Output**
- Reports: Integer
- Your output should report the result of separating your input and adding the digits together

**Examples**
- Doctests available
  - `python3 -m doctest <labfilename>.py` to run autograder
    - Must be in correct parent file

---

## [Exercise 2: gcd(a,b)](https://docs.google.com/presentation/d/1uQ9eGYyW103jQCLhVSGJPzGoA3C6o1i1jVqGH_8yiZ0/edit#slide=id.g30f9423a9ce_45_9)

**Objective**
Create a function that finds the greatest common divisor of two positive integers

**Notes**
- Modular arithmetic will help here

**Inputs**
- a = positive integer
- b = positive integer

**Output**
- Reports: Integer
- Your output should be the greatest common divisor of your two input integers

**Examples**
- Doctests available
  - `python3 -m doctest <labfilename>.py` to run autograder
    - Must be in correct parent file

---

## Exercise 3: decimal_to_binary(n)

**Objective**
Create a function that converts a non-negative integer to its binary representation

**Notes**
- Use the str function to output a string instead of an integer

**Inputs**
- n = some integer
  - the non-negative integer to be converted

**Output**
- Reports: String
- Your output should be a string representing the converted binary representation

**Examples**
- Doctests available
  - `python3 -m doctest <labfilename>.py` to run autograder
    - Must be in correct parent file

---

**Remember to submit on Gradescope and complete the conceptual portion!**
