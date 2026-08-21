---
title: "Lab 12"
description: "HOFs and Functions as Data"
due: "Tuesday, March 10th, 23:59"
gradescope_assignment_id:
submission_files:
---

# Lab 12: HOFs and Functions as Data

## Instructions
This worksheet serves as a guide and set of instructions to complete Lab 6. All material was sourced from the CS10 version of The Beauty and Joy of Computing (BJC) course.

- You **must** use the [starter file, found here](https://snap.berkeley.edu/project?username=jedi_force&projectname=Lab9%20Starter) to get credit for the lab.  
- Additionally, here is the [workbook](https://cs10.org/bjc-r/llab/html/topic.html?topic=berkeley_bjc%2Fhofs%2Fhofs-practice.topic&course&novideo&noreading&noassignment) that you can read through for further context and additional (non-required) material.  
- Please note: The file name **does not equal the lab number!**

## Submitting
You will need to fill in the blocks under **“Lab 9 Starter”** and submit this to Gradescope (again, the file name does not equal the lab number!).  
- To receive full credit, you must complete the required blocks, and those blocks must pass all tests from the Gradescope autograder.  
- For instructions on how to submit labs to Gradescope, please see [this page](https://docs.google.com/document/d/1XAcZc9ypX07-bt0gK6uQ4P-06SrjPRsgiOjERIOlvYU/edit?usp=sharing).
- ![run autograder]({{ site.baseurl }}/assets/images/lab_images/lab6_0.png)

Please note: you must use the **starter file** above, and you must **not** edit the name of any required blocks. Failing to do either will result in autograder failure.

## Objectives
Throughout the course, you’ve been exposed to HOF blocks like `map`, `keep`, and `combine`. You may have used them to carry out relatively simple tasks, like summing a list with `combine`, or filtering based on word length with `keep`. In this lab, you're going to attack some more complicated problems with the help of HOFs.  

By the end of the lab, you will be comfortable implementing and understanding:
- Build non-HOF blocks to use as helper functions in larger HOF problems
- Complete complex, multi-step HOFs problems
- Use HOFs to solve real-life problems, like minimizing or composing functions

## Required Blocks
- Block 1: is (num) a factorion?  
- Block 2: list all factorions between (num1) and (num2)  
- Block 3: is (num) pandigital?  
- Block 4: list all pandigital numbers between (num1) and (num2)  

---

## Important Topics (Workbook)
For better understanding of the lab we highly recommend going through these workbook pages!  
Topics that are important but not required for this lab will be indicated with an asterisk (**). These topics are best reviewed in order and as you complete the lab.

- [HOFs Practice and Treating Functions as Data](https://cs10.org/bjc-r/cur/programming/HOFs/functions-as-data/hofs-practice-introduction-and-warmup.html?topic=berkeley_bjc%2Fhofs%2Fhofs-practice.topic&course&novideo&noreading&noassignment)
- [Factorions](https://cs10.org/bjc-r/cur/programming/HOFs/functions-as-data/factorions.html?topic=berkeley_bjc%2Fhofs%2Fhofs-practice.topic&course&novideo&noreading&noassignment)
- [Functions as Data](https://cs10.org/bjc-r/cur/programming/HOFs/functions-as-data/functions-as-data.html?topic=berkeley_bjc%2Fhofs%2Fhofs-practice.topic&course&novideo&noreading&noassignment)
- [Pandigital](https://cs10.org/bjc-r/cur/programming/HOFs/functions-as-data/pandigital-numbers.html?topic=berkeley_bjc%2Fhofs%2Fhofs-practice.topic&course&novideo&noreading&noassignment)
- [Generalizing “List all”](https://cs10.org/bjc-r/cur/programming/HOFs/functions-as-data/generalizing-list-all.html?topic=berkeley_bjc%2Fhofs%2Fhofs-practice.topic&course&novideo&noreading&noassignment) **
- [Extra for Experience: Composing Functions](https://cs10.org/bjc-r/cur/programming/HOFs/functions-as-data/compose-over-list.html?topic=berkeley_bjc%2Fhofs%2Fhofs-practice.topic&course&novideo&noreading&noassignment) **

---

## Block 1: is (num) a factorion?
**Objective**  
- Create a predicate block that, when input with a number, reports if that number is a factorion (True/False).  
- A number is called a factorion if the number is equal to the sum of the factorials of its digits.  
- Example: 145 is a factorion since 145 = 1! + 4! + 5!.  
- Please use HOFs in your solution.  

**Hint**: Filling out and using the `factorial (num)` block may be extremely helpful.  

**Inputs**  
- `num`: any number  

**Output**  
- Reports a **boolean** (`true` if factorion, otherwise `false`)  

**Examples**  
- ![example factorion check true for 145]({{ site.baseurl }}/assets/images/lab_images/lab6_b1_2.png)  
- ![example factorion check false for 123]({{ site.baseurl }}/assets/images/lab_images/lab6_b1_3.png)  
- ![example factorion check true for 40585]({{ site.baseurl }}/assets/images/lab_images/lab6_b1_4.png)  

---

## Block 2: list all factorions between (num1) and (num2)
**Objective**  
- Create a block that takes two numbers and returns all numbers (including num1 and num2) that are factorions in a list.  

**Inputs**  
- `num1`, `num2`: any numbers  

**Output**  
- Reports a **list** containing all factorions between (and including) num1 and num2  

**Examples**  
- ![example list factorions between 1 and 2000]({{ site.baseurl }}/assets/images/lab_images/lab6_b2_1.png)  
- ![example list factorions between 1 and 50000]({{ site.baseurl }}/assets/images/lab_images/lab6_b2_2.png)  

---

## Block 3: is (num) pandigital?
**Objective**  
- Create a predicate block that reports if the input number is pandigital.  
- A number is called pandigital if it uses all of the digits from 1 to n exactly once, where n is the number of digits in the number.  
  - Example: 15432 is pandigital, but 11132 is not.  

**Inputs**  
- `num`: any number  

**Output**  
- Reports a **boolean**  

**Examples**  
- ![example pandigital check true for 15432]({{ site.baseurl }}/assets/images/lab_images/lab6_b3_1.png)  
- ![example pandigital check false for 11132]({{ site.baseurl }}/assets/images/lab_images/lab6_b3_2.png)  
- ![example pandigital check true for 987654321]({{ site.baseurl }}/assets/images/lab_images/lab6_b3_3.png)  

---

## Block 4: list all pandigital numbers between (num1) and (num2)
**Objective**  
- Create a block that takes two numbers and lists all numbers (including num1 and num2) that are pandigital in a list.  

**Inputs**  
- `num1`, `num2`: any numbers  

**Output**  
- Reports a **list** containing all pandigital numbers between (and including) num1 and num2  

**Examples**  
- ![example list pandigital numbers between 100 and 500]({{ site.baseurl }}/assets/images/lab_images/lab6_b4_1.png)  
- ![example list pandigital numbers between 1 and 10000]({{ site.baseurl }}/assets/images/lab_images/lab6_b4_2.png)  

---

**Remember to submit on Gradescope and complete the conceptual portion!**
