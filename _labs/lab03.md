---
title: "Lab 03"
description: "Conditionals, Reporters, & Abstraction"
due: "Tuesday February 3rd, 23:59"
gradescope_assignment_id:
submission_files:
---

# Lab 3: Conditionals, Reporters, & Abstraction

## Instructions
This worksheet serves as a guide and set of instructions to complete Lab 3. All material was sourced from the CS10 version of The Beauty and Joy of Computing (BJC) course.

- You **must** use the [starter file, found here](https://snap.berkeley.edu/snap/snap.html#open:https://cs10.org/bjc-r/prog/conditionals/lab3-starter-code-v2.xml) to get credit for the lab.
- Additionally, here is the [workbook](https://cs10.org/bjc-r/llab/html/topic.html?topic=berkeley_bjc%2Fintro_pair%2F2-conditionals-testing-su21.topic&course=cs10_fa21.html&novideo&noreading&noassignment) that you can read through for further context and additional (non-required) material.

## Submitting
You will need to fill in the blocks under **“Lab 3: Conditionals, Reporters, & Abstraction”** and submit this to Gradescope.
- To receive full credit, you must complete the required blocks, and those blocks must pass all tests from the Gradescope autograder.
- For instructions on how to submit labs to Gradescope, please see [this page](https://docs.google.com/document/d/1XAcZc9ypX07-bt0gK6uQ4P-06SrjPRsgiOjERIOlvYU/edit?usp=sharing).

Please note: you must use the **starter file** above, and you must **not** edit the name of any required blocks. Failing to do either will result in autograder failure.

## Objectives
So far, you've practiced writing scripts that carry out short sequences of commands (they run every block, in order). In this lab you will explore conditionals for more complex behavior. By the end of the lab, you will:
- Implement conditional statements in your code.
- Practice writing and reading functions with booleans and boolean operators.
- Understand the use of reporter functions and their outcomes.

## Required Blocks
- [Block 1: traffic signal (color)](#block-1-traffic-signal-color)
- [Block 2: letter grade (number)](#block-2-letter-grade-number)
- [Block 3: is (num1) between (num2) and (num3)](#block-3-is-num1-between-num2-and-num3)
- [Block 4: sum of two smallest (num1) and (num2) and (num3)](#block-4-sum-of-two-smallest-num1-and-num2-and-num3)

## Important Topics mentioned in the Workbook
For better understanding of the lab we highly recommend going through these workbook pages! Topics that are important but not required for this lab will be indicated with an asterisk **. These topics are best reviewed in order and as you complete the lab.

- [Introduction: why do we need conditionals?](https://cs10.org/bjc-r/cur/programming/conditionals/conditionals-intro.html?1&1&1&2&2&2&3&3&3&4&4&topic=berkeley_bjc%2Fintro_pair%2F2-conditionals-testing-su21.topic&course=cs10_fa21.html&novideo&noreading&noassignment)
- [If and If-else](https://cs10.org/bjc-r/cur/programming/conditionals/if-and-if-else.html?1&1&1&2&2&2&3&3&3&4&4&topic=berkeley_bjc%2Fintro_pair%2F2-conditionals-testing-su21.topic&course=cs10_fa21.html&novideo&noreading&noassignment)
- [More Complex Boolean Expressions](https://cs10.org/bjc-r/cur/programming/conditionals/complex-booleans.html?1&1&1&1&2&2&2&3&3&3&4&4&topic=berkeley_bjc%2Fintro_pair%2F2-conditionals-testing-su21.topic&course=cs10_fa21.html&novideo&noreading&noassignment)**
- [Predicates](https://cs10.org/bjc-r/cur/programming/conditionals/predicates.html?1&1&1&1&2&2&2&2&3&3&3&4&4&topic=berkeley_bjc%2Fintro_pair%2F2-conditionals-testing-su21.topic&course=cs10_fa21.html&novideo&noreading&noassignment)
- [The Max block](https://cs10.org/bjc-r/cur/programming/functions/review-max-block.html?1&1&1&1&2&2&2&2&3&3&3&3&4&4&topic=berkeley_bjc%2Fintro_pair%2F2-conditionals-testing-su21.topic&course=cs10_fa21.html&novideo&noreading&noassignment)

---

## Block 1: Traffic signal (color)
**Objective**
- Create a **reporter** block that, when given a traffic light color, reports the appropriate action (see below).

**Inputs**
- `color` = any text  
  Any text can be typed, but the autograder will test the three traffic light colors: **Red**, **Green**, **Yellow**.

**Output**
- Reports **Text**. Case-sensitive mappings:
  - Input: `Green` → Output: `Go`
  - Input: `Red` → Output: `Stop`
  - Input: `Yellow` → Output: `Yield`

**Examples**
- ![example of traffic signal reporter 'Yellow' with output 'Yield']({{ site.baseurl }}/assets/images/lab_images/lab3_b1_1.png)
- ![example of traffic signal reporter 'Red' with output 'Stop']({{ site.baseurl }}/assets/images/lab_images/lab3_b1_2.png)
- ![example of failed traffic signal reporter 'Cheese' with output 'did not report']({{ site.baseurl }}/assets/images/lab_images/lab3_b1_3.png)

---

## Block 2: letter grade (number)
**Objective**
- Create a reporter block that, when given a percentage, says the associated letter grade.  
  Example: `letter grade (74)` should say **C**.

**Standardized Letter Grades**
- **A**: 90–100  
- **B**: 80–89.99  
- **C**: 70–79.99  
- **D**: 60–69.99  
- **F**: < 60  
*Note: the autograder is sensitive to decimals and should work for all non-negative numbers (e.g., 89.99123123).*

**Inputs**
- `number` = any number  
  You may assume users will input a non-negative number ≤ 100.

**Output**
- Reports **Text** (case-sensitive, no extra spaces or quotes).

**Examples**
- ![example of letter grade reporter '89.999' with output 'B']({{ site.baseurl }}/assets/images/lab_images/lab3_b2_1.png)
- ![example of letter grade reporter '70' with output 'C']({{ site.baseurl }}/assets/images/lab_images/lab3_b2_2.png)
- ![example of letter grade reporter '2' with output 'F']({{ site.baseurl }}/assets/images/lab_images/lab3_b2_3.png)

---

## Block 3: is (num1) between (num2) and (num3)
**Objective**
- Create a **predicate** block that determines if a number is between two other numbers.  
  Return **true** if the first number is between the other two or equal to either boundary.

**Notes**
- `num1`, `num2`, and `num3` can be the same numbers.
- `num2` and `num3` may be in any order (e.g., `num3` can be less than `num2`).

**Inputs**
- `num1`, `num2`, `num3` = any numbers.

**Output**
- Reports a **boolean** (`true` or `false`).

**Examples**
- ![example of is '3' between '1' and '5' and reports 'True']({{ site.baseurl }}/assets/images/lab_images/lab3_b3_1.png)
- ![example of is '9' between '1' and '5' and reports 'False']({{ site.baseurl }}/assets/images/lab_images/lab3_b3_2.png)
- ![example of is '88' between '36' and '-5' and reports 'False']({{ site.baseurl }}/assets/images/lab_images/lab3_b3_3.png)
- ![example of is '4' between '4' and '4' and reports 'True']({{ site.baseurl }}/assets/images/lab_images/lab3_b3_4.png)

---

## Block 4: sum of two smallest (num1) and (num2) and (num3)
**Objective**
- Edit a reporter block named **“sum of two smallest”** that takes three numbers and reports the sum of the two smallest.

**Notes**
- If the two greatest numbers are the same, report the smallest plus either of the two equal numbers.
- If all three numbers are the same, report the sum of any two of them.

**Inputs**
- `num1`, `num2`, `num3` = any numbers.

**Output**
- Reports a **Number** (the sum of the two smallest inputs).

**Examples**
- ![example of sum of two smallest '2' and '5' and '5' and reports '7']({{ site.baseurl }}/assets/images/lab_images/lab3_b4_1.png)
- ![example of sum of two smallest '9' and '9' and '9' and reports '18']({{ site.baseurl }}/assets/images/lab_images/lab3_b4_2.png)
- ![example of sum of two smallest '1' and '12' and '2' and reports '3']({{ site.baseurl }}/assets/images/lab_images/lab3_b4_1.png)

> **Hint:** Look at the [max block](https://cs10.org/bjc-r/cur/programming/functions/review-max-block.html?1&1&1&2&2&2&3&3&3&4&4&topic=berkeley_bjc%2Fintro_pair%2F2-conditionals-testing-su21.topic&course=cs10_fa21.html&novideo&noreading&noassignment). How does it work?

---

**You can always check the validity of your solutions by using the local autograder. Remember to submit on Gradescope and complete the conceptual portion!**
