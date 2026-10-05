---
title: "Lab 09"
description: "Trees & Fractals"
due: "Thursday, February 26th, 23:59"
gradescope_assignment_id:
submission_files:
---

# Lab 9: Trees & Fractals

## Instructions
This worksheet serves as a guide and set of instructions to complete the lab. 

- You **must** use the [starter file, found here](https://snap.berkeley.edu/snap/snap.html#open:https://cs10.org/bjc-r/cur/programming/recur/tree/../../../../prog/recur/lab8-starter-file.xml) to get credit for the lab.
- Additionally, [here is the workbook](https://cs10.org/bjc-r/topic/topic.html?topic=berkeley_bjc/recur/recursion-trees-fractals.topic&course=&novideo&noreading&noassignment) that you can read through for further context and additional (non-required) material. All material was sourced from the CS10 version of The Beauty and Joy of Computing course.

## Submitting
You will need to fill in the blocks under the starter file and submit this to Gradescope. 
- To receive full credit for the coding portion, you will need to complete the required blocks, and the required blocks must pass all tests from the autograder in Gradescope.
- For instructions on how to submit to labs to Gradescope, please see [this page](https://docs.google.com/document/d/1zh-3Mz-4mrfv0lqqI0JHfi31PBUze6QhxFuG4AQUL9s/edit).
  
Please note: you must use the **starter file** above, and you must **NOT** edit the name of any of the required blocks. Failing to do either will result in autograder failure.

## Objectives
Today you will continue to build your knowledge of recursion and understand how we can use recursion to move across data structures (trees, linked lists). We will start by navigating through visual fractals. By the end of lab you will: 
- Explore the idea of representing a problem in terms of itself.
- Practice planning and coding recursive blocks.
- Create your own fractals

## Required Blocks
** It is highly recommended that you work with a partner for this assignment. 
- **DO NOT CHANGE THE COLOR OF YOUR PEN**
- Block 1: snowflake segment levels: (level) size: (size) 
  - You can use only recursion. No HOFs or iteration allowed.
- Block 2: complete snowflake segment levels: (level) size: (size) 
  - You must use Block 1 in your solution
  - Recursion is not used for this question
- Block 3: c-curve segment levels: (level) size: (size) 
  - You can use only recursion. No HOFs or iteration allowed.

## Important Topics mentioned in the Workbook
For better understanding of the lab we highly recommend going through these workbook pages! Topics that are important but not required for this lab will be indicated with an asterisk**. These topics are best reviewed in order and as you complete the lab.
- [Recursion](https://cs10.org/bjc-r/cur/programming/recur/tree/recursive-tree-part-1.html?topic=berkeley_bjc%2Frecur%2Frecursion-trees-fractals.topic&course&novideo&noreading&noassignment)
- [Recursive Tree Part 2](https://cs10.org/bjc-r/cur/programming/recur/tree/recursive-tree-part-2.html?topic=berkeley_bjc%2Frecur%2Frecursion-trees-fractals.topic&course&novideo&noreading&noassignment)
- [Recursive Tree Part 3](https://cs10.org/bjc-r/cur/programming/recur/tree/treepart3.html?topic=berkeley_bjc%2Frecur%2Frecursion-trees-fractals.topic&course&novideo&noreading&noassignment)
- [Base Case and recursive Case](https://cs10.org/bjc-r/cur/programming/recur/tree/base-cases.html?topic=berkeley_bjc%2Frecur%2Frecursion-trees-fractals.topic&course&novideo&noreading&noassignment)
- [Input Sliders!](https://cs10.org/bjc-r/cur/programming/recur/tree/tree-slider.html?topic=berkeley_bjc%2Frecur%2Frecursion-trees-fractals.topic&course&novideo&noreading&noassignment)
- [Self Test: What Was Changed?](https://cs10.org/bjc-r/cur/programming/recur/tree/treechange.html?topic=berkeley_bjc%2Frecur%2Frecursion-trees-fractals.topic&course&novideo&noreading&noassignment)
- [Vary your tree](https://cs10.org/bjc-r/cur/programming/recur/tree/vary-your-tree.html?topic=berkeley_bjc%2Frecur%2Frecursion-trees-fractals.topic&course&novideo&noreading&noassignment)
- [Random Tree](https://cs10.org/bjc-r/cur/programming/recur/tree/random-tree.html?topic=berkeley_bjc%2Frecur%2Frecursion-trees-fractals.topic&course&novideo&noreading&noassignment)
- [Snowflake](https://cs10.org/bjc-r/cur/programming/recur/fractals/snowflake.html?topic=berkeley_bjc%2Frecur%2Frecursion-trees-fractals.topic&course&novideo&noreading&noassignment)
- [C-Curve](https://cs10.org/bjc-r/cur/programming/recur/fractals/c-curve.html?topic=berkeley_bjc%2Frecur%2Frecursion-trees-fractals.topic&course&novideo&noreading&noassignment)

---

## [Block 1: snowflake segment levels: (level) size: (size)](https://cs10.org/bjc-r/cur/programming/recur/fractals/snowflake.html?topic=berkeley_bjc%2Frecur%2Frecursion-trees-fractals.topic&course&novideo&noreading&noassignment)
- Objective:
  - Build a function that can create on side of a coch's snowflalke
  - ![example of one side of a koch's snowflake][sp26-lab09-image1]
 - Notes:
   - You must use recursion, no HOFs or iteration
   - **Each recursive call is <ins>one-third</ins> the size of the caller**
   - **Tip for fractals: The sprite must end in the correct direction (angle!!) at the end
   - ![example of a level three snowflake segment][sp26-lab09-image2]
- Inputs:
  - Level = any number
      - Should be a positive number that indicates the level (2-5 shown below)
      - ![examples of level 2-5 snowflake segments][sp26-lab09-image3]
    - Size = any number
      - Should be any positive number indicates the length of an entire snowflake segment
- Output:
  - None! It is a procedure / non-pure function, so it only displays a visual effect on the stage and does not output any values
    - We are working on a command block! 
- Examples:
  - ![example call to snowflake segment with level 5 and size 200][sp26-lab09-image4]
  - ![example output from call to snowflake segment with level 5 and size 200][sp26-lab09-image5]

---

## Block 2: complete snowflake segment levels: (level) size: (size) 
- Objective:
  - Build a function that will create a koch snowflake. The entire snowflake consists of three copies of the previous fractal, arranged in a triangular shape.
- Notes:
  - You must use the previous block, snowflake segment levels: (level) size: (size), in your solution
  - Recursion is **<ins>not</ins>** used for this question
- Inputs:
  - Level = any number
    -  Should be a positive number that indicates the level
  - Size = any number
    - Should be any positive number indicates the length of an entire snowflake segment
- Output:
  - None! It is a procedure / non-pure function, so it only displays a visual effect on the stage and does not output any values
- Examples:
  - ![example of output of complete snowflake segment levels][sp26-lab09-image6]

---

## [Block 3: c-curve levels: (level) size: (size)](https://cs10.org/bjc-r/cur/programming/recur/fractals/c-curve.html?topic=berkeley_bjc%2Frecur%2Frecursion-trees-fractals.topic&course&novideo&noreading&noassignment) 
- Objective:
  - Build a function that will create a fractal called a c-curve. The fractal should recurse a c-curve shape to create a complex fractal. Please look at this [workbook page](https://cs10.org/bjc-r/cur/programming/recur/fractals/c-curve.html?topic=berkeley_bjc%2Frecur%2Frecursion-trees-fractals.topic&course&novideo&noreading&noassignment) for more instructions.
  - ![example output of c-curve levels][sp26-lab09-image7]
- Notes:
  - You must use recursion. No HOFs.
  - **Each recursive call is <ins>one-half</ins> the size of the caller**
  - ![example call to c-curve with level 2][sp26-lab09-image8]
- Inputs:
  - Level = any number
    - Should be a positive number that indicates the level
  - Size = any number
    - Should be any positive number indicates the total length of the fractal
- Output:
  - None! It is a procedure / non-pure function, so it only displays a visual effect on the stage and does not output any values
- Examples:
  - ![example of output of c-curve levels][sp26-lab09-image9]
  - **<ins>THE COLOR IS TO SHOW THE DIFFERENT PARTS OF THE C-CURVE.</ins>** 

---

**You can always check the validity of your solutions by using the local autograder. Remember to submit on Gradescope!**

[sp26-lab09-image1]: {{ site.baseurl }}/assets/images/lab_images/sp26-lab09-image1.png
[sp26-lab09-image2]: {{ site.baseurl }}/assets/images/lab_images/sp26-lab09-image2.png
[sp26-lab09-image3]: {{ site.baseurl }}/assets/images/lab_images/sp26-lab09-image3.png
[sp26-lab09-image4]: {{ site.baseurl }}/assets/images/lab_images/sp26-lab09-image4.png
[sp26-lab09-image5]: {{ site.baseurl }}/assets/images/lab_images/sp26-lab09-image5.png
[sp26-lab09-image6]: {{ site.baseurl }}/assets/images/lab_images/sp26-lab09-image6.png
[sp26-lab09-image7]: {{ site.baseurl }}/assets/images/lab_images/sp26-lab09-image7.png
[sp26-lab09-image8]: {{ site.baseurl }}/assets/images/lab_images/sp26-lab09-image8.png
[sp26-lab09-image9]: {{ site.baseurl }}/assets/images/lab_images/sp26-lab09-image9.png





