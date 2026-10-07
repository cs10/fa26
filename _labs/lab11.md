---
title: "Lab 10"
description: "Recursive Reporters"
due: "Tuesday, March 3rd, 23:59"
gradescope_assignment_id:
submission_files:
---

# Lab 10: Recursive Reporters

## Instructions
This worksheet serves as a guide and set of instructions to complete the lab. 

- You **must** use the [starter file, found here](https://snap.berkeley.edu/snap/snap.html#present:Username=jedi_force&ProjectName=Lab%20Starter%20-%20recursive%20reporters) to get credit for the lab.
- Additionally, [here is the workbook](https://cs10.org/bjc-r/cur/programming/recur/recursive-reporters/recursive-reporters-intro.html?topic=berkeley_bjc%2Frecur%2Frecursive-reporters-part1.topic&course&novideo&noreading&noassignment) that you can read through for further context and additional (non-required) material. All material was sourced from the CS10 version of The Beauty and Joy of Computing course.

## Submitting
You will need to fill in the blocks under the starter file and submit this to Gradescope. 
- To receive full credit for the coding portion, you will need to complete the required blocks, and the required blocks must pass all tests from the autograder in Gradescope.
- For instructions on how to submit to labs to Gradescope, please see [this page](https://docs.google.com/document/d/1zh-3Mz-4mrfv0lqqI0JHfi31PBUze6QhxFuG4AQUL9s/edit).
  
Please note: you must use the **starter file** above, and you must **NOT** edit the name of any of the required blocks. Failing to do either will result in autograder failure.

## Objectives
Recursion is arguably the second most important topic in this course (after abstraction of course). In today’s lab you will implement what you know about recursion into reporter blocks.  By the end of the lab, you will:
- Understand how reporters use combiners instead of sequences.
- Practice planning and coding recursive reporters.
- Implement higher order functions in non iterative solutions

## Required Blocks:
**<ins>It is highly recommended that you work with a partner for this assignment</ins>**
- Block 1: ends-e (input)
- Block 2: numbers (input)
- Block 3: count parking spots(n)

## Important Topics mentioned in the Workbook
For better understanding of the lab we highly recommend going through these workbook pages! Topics that are important but not required for this lab will be indicated with an asterisk**. These topics are best reviewed in order and as you complete the lab.
- [Recursive Reporters](https://cs10.org/bjc-r/cur/programming/recur/recursive-reporters/recursive-reporters-intro.html?topic=berkeley_bjc%2Frecur%2Frecursive-reporters-part1.topic&course&novideo&noreading&noassignment)
- [Plurals of Words](https://cs10.org/bjc-r/cur/programming/recur/recursive-reporters/plurals-of-words.html?topic=berkeley_bjc%2Frecur%2Frecursive-reporters-part1.topic&course&novideo&noreading&noassignment)
- [What Is Pascal's Triangle?](https://cs10.org/bjc-r/cur/programming/recur/recursive-reporters/pascals-triangle.html?topic=berkeley_bjc%2Frecur%2Frecursive-reporters-part1.topic&course&novideo&noreading&noassignment)
- [Pascal's Triangle](https://cs10.org/bjc-r/cur/programming/recur/recursive-reporters/pascals-triangle-selftest.html?topic=berkeley_bjc%2Frecur%2Frecursive-reporters-part1.topic&course&novideo&noreading&noassignment)
- [How Long Does This Computation Take?](https://cs10.org/bjc-r/cur/programming/recur/recursive-reporters/pascals-triangle-how-long-does-the-computation-take.html?topic=berkeley_bjc%2Frecur%2Frecursive-reporters-part1.topic&course&novideo&noreading&noassignment) **
- [Even Numbers](https://cs10.org/bjc-r/cur/programming/recur/recursive-reporters/even-number-filter-without-generalization.html?topic=berkeley_bjc%2Frecur%2Frecursive-reporters-part1.topic&course&novideo&noreading&noassignment)
- [Sorting a List](https://cs10.org/bjc-r/cur/programming/recur/recursive-reporters/recursively-sorting-even-odd.html?topic=berkeley_bjc%2Frecur%2Frecursive-reporters-part1.topic&course&novideo&noreading&noassignment) + [Cont](https://cs10.org/bjc-r/cur/programming/recur/recursive-reporters/recursively-sorting-merge.html?topic=berkeley_bjc%2Frecur%2Frecursive-reporters-part1.topic&course&novideo&noreading&noassignment) ** 

---

## Block 1: ends-e(input)
- Objective: 
  - Edit a reporter block, ends-e, that takes a list of words as input, and reports a list of those words from the input whose last letter is e 
- Note
  - **<ins>You must use recursion, no HOFs or iteration</ins>** 
- Inputs:
  - Input = anything
    - Input should be a list of words
- Output:
  - Reports: a list
    - A list if all the words from the list that ends with e
    - If there are no words that end with e, the reporter reports an empty list
- Examples:
  - ![example call to ends e with a 5 word list][sp26-lab10-image1]
  - ![example call to ends e an empty list][sp26-lab10-image2]
  - ![example call to ends e with a different 5 word list][sp26-lab10-image3]

---

## Block 2: numbers (input)
- Objective: 
  - Edit a reporter block, numbers, that takes a list of mixed words and numbers as input, and reports a list of just the numbers from the input list.
- Notes:
  - **<ins>You must use recursion, no HOFs or iteration</ins>** 
- Input = anything
  - Input should be a list of words, strings, and numbers
- Output:
  - Reports: a list
    - A list if all the items in the list that are numbers
    - If there are no numbers in the list, the reporter reports an empty list
- Examples:
  - ![example call to numbers with a 4 element list containing two numbers][sp26-lab10-image4]
  - ![example call to numbers with a list containing an element with the division operator][sp26-lab10-image5]
  - ![example call to numbers with a list containing an ellipse][sp26-lab10-image6]

---

## Block 3: count parking spots (n)
- Objective: 
  - A straight parking lot has “n” contiguous spots in a single row. You have an unlimited supply of three vehicle types:
    - Scooter: occupies 1 spot
    - Car: occupies 2 spots
    - Van: occupies 3 spots
  - Vehicles must exactly fill the lot (no gaps and no overhang). Two parking spots are considered different if any spot in the row is covered by a different vehicle (i.e., order and placement matter).
  - Write a function count parking spots(n) that returns the number of distinct parking spots that exactly fill a lot of length n using scooters, cars, and vans.
- Notes:
  - **<ins>You must use recursion, no HOFs or iteration</ins>** 
  - Hints:
    - Think “first choice, rest of the problem.”
    - From the leftmost open spot, branch on placing:
      - a scooter (uses 1 spot),
      - a car (uses 2 spots),
      - a van (uses 3 spots)
      - Each choice reduces the remaining available parking spots to n−1, n−2, or n−3.
      - Base cases: if n == 0, that’s one valid way; if n < 0, that branch is impossible.
- Inputs
  - N = number of available parking spots 
- Output:
    - Reports: Number
      - The number of combinations of vehicles we can use to park in the available spots
- Examples:
  - count parking spots(0) → 1 (the empty layout)
  - count parking spots(2) → 2 because the valid parking combinations are:
    - Scooter, Scooter
    - Car
  - count parking spots(3) → 4 because the parking combinations are:
    - Scooter, Scooter, Scooter
    - Scooter, Car
    - Car, Scooter
    - Van

---

**You can always check the validity of your solutions by using the local autograder. Remember to submit on Gradescope!**

[sp26-lab10-image1]: {{ site.baseurl }}/assets/images/lab_images/sp26-lab10-image1.png
[sp26-lab10-image2]: {{ site.baseurl }}/assets/images/lab_images/sp26-lab10-image2.png
[sp26-lab10-image3]: {{ site.baseurl }}/assets/images/lab_images/sp26-lab10-image3.png
[sp26-lab10-image4]: {{ site.baseurl }}/assets/images/lab_images/sp26-lab10-image4.png
[sp26-lab10-image5]: {{ site.baseurl }}/assets/images/lab_images/sp26-lab10-image5.png
[sp26-lab10-image6]: {{ site.baseurl }}/assets/images/lab_images/sp26-lab10-image6.png







