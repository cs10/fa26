---
title: "Lab 04"
description: "Iteration"
due: "Thursday, February 5th, 23:59"
gradescope_assignment_id:
submission_files:
---

# Lab 4: Iteration

## Instructions
This worksheet serves as a guide and set of instructions to complete Lab 4. All material was sourced from the CS10 version of The Beauty and Joy of Computing (BJC) course.

- You **must** use the [starter file, found here](https://snap.berkeley.edu/snap/snap.html#present:Username=jedi_force&ProjectName=Lab%3a%20Lists%20%2b%20Loops&editMode&noRun) to get credit for the lab.
- **This lab has NO workbook.** All the instructions are within this sheet and the starter file

## Submitting
You will need to fill in the blocks under the starter file, **“Lab 4: Lists + Loops”**, and submit this to Gradescope.
- To receive full credit, you must complete the required blocks, and those blocks must pass all tests from the Gradescope autograder.
- For instructions on how to submit labs to Gradescope, please see [this page](https://docs.google.com/document/d/1XAcZc9ypX07-bt0gK6uQ4P-06SrjPRsgiOjERIOlvYU/edit?usp=sharing).

Please note: you must use the **starter file** above, and you must **not** edit the name of any required blocks. Failing to do either will result in autograder failure.

## Objectives
Previously in the lab, we have worked with iteration (loops) when creating polygons. In lecture, we saw how we can use iteration with variables and with lists. By the end of the lab, you will be comfortable implementing and understanding:
- Iterative functions
- Functions using the list data type.
- The ordered characteristic of lists
- The differences between the various loops
- When to use certain loops
- How to filter and keep items from a list
- How to use variables with lists

## Required Blocks
**Please note, all functions must be completed iteratively. HOFs and Recursion are banned.**
- Block 1: add all numbers from num1: _ to num2: _
- Block 2: report only even numbers from list: _
- Block 3: add start num: _ until > than stop num: _ and is odd
  - For each and For i blocks are also banned for this problem
- Block 4: is num: _ prime?
- Block 5: report only prime numbers from the list: _

---

## Block 1: add all numbers from num1: _ to num2: _
**Objective**
- Add all the numbers together in the range from num1 to num2. The starting number will be num1, and you will continuously add numbers until you reach num2 (the final number to add)

**Inputs**
- `num1`: integer
- `num2`: integer

**Output**
- Reports an `integer`

**Examples**
- ![example of adding all numbers between 1 and 5 with output 15]({{ site.baseurl }}/assets/images/lab_images/lab4_b1_1.PNG)
  - add all numbers from num1: "1" to num2: "5" will add 1 + 2 + 3 + 4 + 5 and output 15
- ![example of adding all numbers between 3 and 7 with output 25]({{ site.baseurl }}/assets/images/lab_images/lab4_b1_2.PNG)
  -  add all numbers from num1: "3" to num2: "7" will add 3 + 4 + 5 + 6 + 7 and output 25
- ![example of adding all numbers between -4 and 2 with output -7]({{ site.baseurl }}/assets/images/lab_images/lab4_b1_3.PNG)
  -  add all numbers from num1: "-4" to num2: "2" will add -4 + -3 + -2 + -1 + 0 + 1 + 2 and output -7
- ![example of adding all numbers between 2 and 2 with output 2]({{ site.baseurl }}/assets/images/lab_images/lab4_b1_4.PNG)
  - add all numbers from num1: "2" to num2: "2" will not add but start and end at 2, outputting 2

---

## Block 2: report only even numbers from list: _
**Objective**
- Report a new list that only contains numbers that are even (i.e. divisible by 2). You should be returning a new list that only keeps the even numbers.
- You may use the “mod" block. Mod stands for modulus. Given two numbers, a (the dividend) and b (the divisor), the modulus operation a mod b returns the remainder when a is divided by b. For example, 4 mod 2 is 0 since 4 is divisible by 2. 4 mod 3 is 1. [See this Wikipedia article](https://en.wikipedia.org/wiki/Modulo) for more information on modulus.

**Inputs**
- input: `list` (of integers)

**Output**
- Reports a `list` 

**Examples**
- ![example of report only even letters with a list containing 1, 2, 3, 4, 5]({{ site.baseurl }}/assets/images/lab_images/lab4_b2_1.PNG)
  - report only even numbers from `[1, 2, 3, 4, 5]` will return `[2, 4]`.
- ![example of report only even letters with a list containing 2, 4, 6, 8]({{ site.baseurl }}/assets/images/lab_images/lab4_b2_2.PNG)
  - report only even numbers from `[2, 4, 6, 8]` will return `[2, 4, 6, 8]`.
- ![example of report only even letters with a list containing -2, -4, -6, -8]({{ site.baseurl }}/assets/images/lab_images/lab4_b2_3.PNG)
  - report only even numbers from `[-2, -4, -6, -8]` will return `[-2, -4, -6, -8]`.
- ![example of report only even letters with a list containing 1, 3, 5, , 7]({{ site.baseurl }}/assets/images/lab_images/lab4_b2_4.PNG)
  - report only even numbers from `[1, 3, 5, 7]` will return `[ ]`.

---

## Block 3: add start num: _ until > than stop num: _ and is odd
**Objective**
- Add numbers continuously starting at a start number until the added numbers are greater than the stop number AND the added numbers are odd. Both of these conditions need to be true until the loop terminates. 
- Each time the loop is iterated through, the output number will be added to by a number incrementing by 1 starting at the start num. 

**Notes**
- __**For this function, you will need the "repeat until" block. You are NOT allowed to use the "for i" loop OR the "for each" loop.**__

**Inputs**
- `start num`: integer
- `stop num`: integer

**Output**
- Reports a **integer**.

**Restrictions**
- Cannot use the "for i" OR "for each" blocks

**Examples**
- ![example of add 1 until > than 2 and is odd with output 3]({{ site.baseurl }}/assets/images/lab_images/lab4_b3_1.PNG)
  - add start num: `1` until > than stop num: `2` and is odd will add 1 + 2 and output 3.
- ![example of add 1 until > than 7 and is odd with output 15]({{ site.baseurl }}/assets/images/lab_images/lab4_b3_2.PNG)
  - add start num: `1` until > than stop num: `7` and is odd will add 1 + 2 + 3 + 4 + 5 and output 15.
- ![example of add 3 until > than 6 and is odd with output 7]({{ site.baseurl }}/assets/images/lab_images/lab4_b3_3.PNG)
  - add start num: `3` until > than stop num: `6` and is odd will add 3 + 4 and output 7.

---

## Block 4: is num: _ prime?
**Objective**
- Evaluates the number and returns true if the number is prime, and return false if the number is NOT prime. To do this, you will need to check if all the numbers smaller than the given number and greater than 1 are divisible by the given number. 

**Notes**
- A prime number is a natural number greater than 1 that has no positive divisors other than 1 and itself.
- 0 and 1 are neither prime nor composite, so the domain will be greater than 1.

**Inputs**
- `num`: integer

**Output**
- Reports a **boolean**.

**Examples**
- ![example of is 17 prime and reports true]({{ site.baseurl }}/assets/images/lab_images/lab4_b4_1.PNG)
  - is num: `17` prime would output `true`
- ![example of is 10 prime and reports false]({{ site.baseurl }}/assets/images/lab_images/lab4_b4_2.PNG)
  - is num: `10` prime would output `false`
- ![example of is 2 prime and reports true]({{ site.baseurl }}/assets/images/lab_images/lab4_b4_3.PNG)
  - is num: `2` prime would output `true`


---

## Block 5: report only prime numbers from the list: _

**Objective**
- Report a new list that only contains prime numbers. This function should filter out any non-prime numbers from the input list. 
- The order of the items should still be preserved - just filtered.

**Notes**
- You can and should use the "is num: _ prime?" block you just made!
- **There is a error in one of the test cases:** 
  - report only prime number from list: `[2, 4, 6, 8]` will return an empty list when it __should__ return `[2]`


**Inputs**
- input: list

**Output**
- Reports a **list**.

**Examples**
- ![example of report only prime numbers from a list containing 2, 3, 4, 5]({{ site.baseurl }}/assets/images/lab_images/lab4_b5_1.PNG)
  - report only prime numbers from list: `[2, 3, 4, 5]` will output `[2, 3, 5]`
- ![example of report only prime numbers from a list containing 11, 7, 6, 0]({{ site.baseurl }}/assets/images/lab_images/lab4_b5_2.PNG)
  - report only prime numbers from list: `[11, 7, 6, 0]` will output `[11, 7]`
- ![example of report only prime numbers from a list containing 4, 6, 8, 10]({{ site.baseurl }}/assets/images/lab_images/lab4_b5_3.PNG)
  - report only prime numbers from list: `[4, 6, 8, 10]` will output `[ ]`


---

## **(OPTIONAL)** Challenge Block 6: report the duplicates in list: _

**Objective**
- Write a function that takes a list of integers and returns a list of all the integers that appear more than once in the input list. The returned list should not contain any duplicates. If there are no duplicates, then the function should report any empty list. 
- The order of the items should still be preserved - just filtered.

**Notes**
- This block is optional and not required for the lab!
- There is a built-in function in Snap! called "uniques". You are **NOT** allowed to use this function.

**Inputs**
- input: list

**Output**
- Reports a **list**.

**Restrictions**
- Cannot use the "uniques" block

**Examples**
- ![example of report the duplicates of a list containing 1, 2, 1, 3, 2, 3]({{ site.baseurl }}/assets/images/lab_images/lab4_b6_1.PNG)
  - report the duplicates in list: `[1, 2, 1, 3, 2, 3]` will output `[1, 2, 3]`
- ![example of report the duplicates of a list containing 4, 4, 3, 10, 33, 4]({{ site.baseurl }}/assets/images/lab_images/lab4_b6_2.PNG)
  - report the duplicates in list: `[4, 4, 3, 10, 33, 4]` will output `[4]`
- ![example of report the duplicates of a list containing 7, 2, 3, 2, 7]({{ site.baseurl }}/assets/images/lab_images/lab4_b6_3.PNG)
  - report the duplicates in list: `[7, 2, 3, 2, 7]` will output `[7, 2]`
- ![example of report the duplicates of a list containing 1, 4, 6, 3]({{ site.baseurl }}/assets/images/lab_images/lab4_b6_4.PNG)
  - report the duplicates in list: `[1, 4, 6, 3]` will output `[ ]`


---
**You can always check the validity of your solutions by using the local autograder. Remember to submit on Gradescope and complete the conceptual portion!**
