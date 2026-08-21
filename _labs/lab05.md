---
title: "Lab 05"
description: "Lists + HOFs"
due: "Tuesday, February 10th, 23:59"
gradescope_assignment_id:
submission_files:
---

# Lab 5: Lists + HOFs

## Instructions
This worksheet serves as a guide and set of instructions to complete Lab 5. All material was sourced from the CS10 version of The Beauty and Joy of Computing (BJC) course.

- You **must** use the [starter file, found here](https://snap.berkeley.edu/snap/snap.html#open:https://cs10.org/bjc-r/prog/hofs/list-and-HOFs-starter.xml) to get credit for the lab.
- Additionally, [here is the workbook](https://cs10.org/bjc-r/topic/topic.html?topic=berkeley_bjc/lists/lists-I.topic&course=&novideo&noreading&noassignment) that you can read through for further context and additional (non-required) material.
- **This lab has a workbook.** Please use the "run autograder" block for testing. **Do not** use the other predicate blocks found in the autograder block sections.

## Submitting
You will need to fill in the blocks under the starter file and submit this to Gradescope.
- To receive full credit, you must complete the required blocks, and those blocks must pass all tests from the Gradescope autograder.
- For instructions on how to submit labs to Gradescope, please see [this page](https://docs.google.com/document/d/1zh-3Mz-4mrfv0lqqI0JHfi31PBUze6QhxFuG4AQUL9s/edit).

Please note: you must use the **starter file** above, and you must **not** edit the name of any required blocks. Failing to do either will result in autograder failure.

## Objectives
In the last lecture, you explored lists, a collection of elements that can be accessed by their position. By the end of the lab, you will:
- Understand and implement lists into your code
- Practice using higher order functions in your code
- Understand the use and importance of higher order functions

## Required Blocks
**Please note, you must use HOFs for this lab. Iteration and recursion are banned unless otherwise specified.**
- Block 1: acronym of list (wordlist)
- Block 2: acronym keep only capitals (input)
- Block 3: exaggerate (input)
- Block 4: expand (input)

## Important Topics mentioned in the Workbook
For better understanding of the lab we highly recommend going through these workbook pages! Topics that are important but not required for this lab will be indicated with an asterisk**. These topics are best reviewed in order and as you complete the lab.

- [What good are lists?](https://cs10.org/bjc-r/cur/programming/lists/hof/what-good-are-lists.html?topic=berkeley_bjc%2Flists%2Flists-I.topic&course&novideo&noreading&noassignment)
- [Transforming each item of a list](https://cs10.org/bjc-r/cur/programming/lists/hof/transforming-each-item-of-a-list.html?topic=berkeley_bjc%2Flists%2Flists-I.topic&course&novideo&noreading&noassignment)
- [Choosing some items from a list](https://cs10.org/bjc-r/cur/programming/lists/hof/choosing-some-items-from-a-list.html?topic=berkeley_bjc%2Flists%2Flists-I.topic&course&novideo&noreading&noassignment)
- [Combining all the items of a list](https://cs10.org/bjc-r/cur/programming/lists/hof/combining-all-the-items-of-a-list.html?topic=berkeley_bjc%2Flists%2Flists-I.topic&course&novideo&noreading&noassignment)
- [Composing higher order functions to solve more complicated problems](https://cs10.org/bjc-r/cur/programming/lists/hof/composing-higher-order-functions-to-solve-more-complicated-problems.html?topic=berkeley_bjc%2Flists%2Flists-I.topic&course&novideo&noreading&noassignment)

---

## Block 1: acronym of list (wordlist)

**Objective**
- Create a reporter block that reports the first letter of each string, all joined together.

**Notes**
- You should not use map or combine when creating your block
- You must use hyperblocks! Use of HOFs and iterative blocks will fail the tests!
- Try the join block

**Inputs**
- `wordlist`: list

**Output**
- Reports: **text**

**Examples**
- ![example with input "computer science" outputs "cs"][sp26-lab05-image1]
- ![example with input "data structures" outputs "ds"][sp26-lab05-image2]

---

## Block 2: acronym keep only capitals (input)

**Objective**
- Create a reporter block that reports the first letter of each string with a capital letter in the front, all joined together.

**Notes**
- Experiment with the unicode of block
- You must use HOFs. Use of iterative blocks will fail the tests.

**Inputs**
- `input`: text (usually a sentence or phrase)

**Output**
- Reports: **text** (an acronym of the text only selecting words with a capital letter in the front)

**Examples**
- ![example with input "University of California Berkeley" outputs "UCB"][sp26-lab05-image3]
- ![example with input "The Beauty and Joy of Computing" outputs "TBJC"][sp26-lab05-image4]

---

## Block 3: exaggerate (input)

**Objective**
- Write a reporter exaggerate that takes a sentence as input and reports an exaggerated version.
- It should replace "good" with "great," "bad" with "terrible," and "like" with "love"
- It should replace every number with twice the number.

**Inputs**
- `input`: text (usually a sentence)

**Output**
- Reports: **text**

**Examples**
- ![example showing text transformation with word replacements][sp26-lab05-image5]
- ![example showing text transformation with number doubling][sp26-lab05-image6]
- ![example showing combined word and number transformations][sp26-lab05-image7]

---

## Block 4: expand (input)

**Objective**
- Write an expand reporter that takes a sentence as input, and reports a sentence that's the same except that each number in the input is replaced by that many copies of the following word

**Notes**
- If the last word is a number, add the number unmodified.

**Inputs**
- `input`: text (usually a sentence)

**Output**
- Reports: **text**

**Examples**
- ![example showing number expansion with following words][sp26-lab05-image8]
- ![example showing multiple number expansions][sp26-lab05-image9]
- ![example showing edge case with number at end][sp26-lab05-image10]

---

**You can always check the validity of your solutions by using the local autograder. Remember to submit on Gradescope!**

[sp26-lab05-image1]: {{ site.baseurl }}/assets/images/lab_images/sp26-lab05-image1.png
[sp26-lab05-image2]: {{ site.baseurl }}/assets/images/lab_images/sp26-lab05-image2.png
[sp26-lab05-image3]: {{ site.baseurl }}/assets/images/lab_images/sp26-lab05-image3.png
[sp26-lab05-image4]: {{ site.baseurl }}/assets/images/lab_images/sp26-lab05-image4.png
[sp26-lab05-image5]: {{ site.baseurl }}/assets/images/lab_images/sp26-lab05-image5.png
[sp26-lab05-image6]: {{ site.baseurl }}/assets/images/lab_images/sp26-lab05-image6.png
[sp26-lab05-image7]: {{ site.baseurl }}/assets/images/lab_images/sp26-lab05-image7.png
[sp26-lab05-image8]: {{ site.baseurl }}/assets/images/lab_images/sp26-lab05-image8.png
[sp26-lab05-image9]: {{ site.baseurl }}/assets/images/lab_images/sp26-lab05-image9.png
[sp26-lab05-image10]: {{ site.baseurl }}/assets/images/lab_images/sp26-lab05-image10.png
