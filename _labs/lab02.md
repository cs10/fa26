---
title: # Lab 02: 

description: Build Your Own Blocks
due: Thursday, January 29th, 2359 hrs
gradescope_assignment_id: 
submission_files:
---

# Lab 2: Build Your Own Blocks

## Instructions: 
This worksheet serves as a guide and set of instructions to complete lab 2. All material was sourced from the CS10 version of The Beauty and Joy of Computing course.

- You **must** use the [starter file, found here](https://snap.berkeley.edu/snap/snap.html#open:https://cs10.org/bjc-r/prog/loop/lab2-starter-code-v3.xml) to get credit for the lab.
- Make sure to log in first before you start the lab! (upper left, cloud icon)
- DO NOT modify the "Autograde" sprite. You should only modify the blocks pertinent to the "Lab" sprite.
- Remember to save your work as you progress through the lab.
    - You can save your work by clicking the page icon on the upper left corner and choosing to save your work on the cloud or directly to your computer
- [Here is the workbook](https://cs10.org/bjc-r/cur/programming/loops/repeat-n/introduction-to-repeat-n.html?1&2&2&3&topic=berkeley_bjc%2Fintro_pair%2F2-loops-variables.topic&course=cs10_fa21.html&novideo&noreading&noassignment) that you can read through for further context and additional (non-required) material. 

## Submitting: 
- You will need to fill in the blocks under "Lab 2: Build Your Own Blocks" and submit this to Gradescope. Note that the titles of the starter files may not always match up. 
- To receive full credit, you will need to complete the required blocks, and the required blocks must pass all tests from the autograder in **Gradescope**. 
    - For instructions on how to submit to labs to Gradescope, please see this [doc](https://docs.google.com/document/d/1XAcZc9ypX07-bt0gK6uQ4P-06SrjPRsgiOjERIOlvYU/edit?usp=sharing).

 Please note, you **must** use the [starter file](https://snap.berkeley.edu/snap/snap.html#open:https://cs10.org/bjc-r/prog/loop/lab2-starter-code-v3.xml), and you must NOT edit the name of any of the required blocks. Failing to do either for these will result in the autograder failing.

## Objectives: 
In this lab, you will learn to create your own blocks and procedures. By the end of the lab, you will be comfortable implementing:
- New procedures
- Input variables
- Loops and iteration
- Arithmetic operations in your code (such as addition, division, subtraction, etc.)
- Generalized procedures
- Creating new shapes and visualizations (such as polygons, flowers, etc.)

## Required Blocks: 
- [Block 1:  draw a polygon with (sides) sides of (length) length](#block-1--draw-a-polygon-with-sides-sides-of-length-length)
- [Block 2: draw a square leaved flower with (leaves) leaves of (size) size](#block-2-draw-a-square-leaved-flower-with-leaves-leaves-of-size-size)

> **Please do not change the pen hue color when attempting the flower field block as it tends to mess up the autograder

> **Please do not change block names

## Important Topics mentioned in the CS 10 Workbook: 
For better understanding of the lab we highly recommend going through these workbook pages! Topics that are important but not required for this lab will be indicated with an asterisk**
- [Don't repeat yourself; Let Snap! do it for you](https://cs10.org/bjc-r/cur/programming/loops/repeat-n/introduction-to-repeat-n.html?1&1&2&2&2&3&3&4&4&4&5&topic=berkeley_bjc%2Fintro_pair%2F2-loops-variables.topic&course=cs10_fa21.html&novideo&noreading&noassignment)
- [Keeping track of your progress through a loop:](https://cs10.org/bjc-r/cur/programming/loops/for/introduction-to-for.html?1&1&2&2&3&topic=berkeley_bjc%2Fintro_pair%2F2-loops-variables.topic&course=cs10_fa21.html&novideo&noreading&noassignment) Repeat vs Forever
- [The FOR block**](https://cs10.org/bjc-r/cur/programming/loops/for/for.html?1&1&2&2&3&topic=berkeley_bjc%2Fintro_pair%2F2-loops-variables.topic&course=cs10_fa21.html&novideo&noreading&noassignment)
- [Your first custom block](https://cs10.org/bjc-r/cur/programming/functions/intro/tutorial-custom-blocks.html?1&1&2&2&2&3&topic=berkeley_bjc%2Fintro_pair%2F2-loops-variables.topic&course=cs10_fa21.html&novideo&noreading&noassignment) + [Adding an input](https://cs10.org/bjc-r/cur/programming/functions/intro/adding-a-simple-input.html?1&1&2&2&2&3&topic=berkeley_bjc%2Fintro_pair%2F2-loops-variables.topic&course=cs10_fa21.html&novideo&noreading&noassignment)
- [Composition of Blocks](https://cs10.org/bjc-r/cur/programming/functions/intro/composing-blocks.html?1&1&2&2&2&3&3&4&4&4&5&5&topic=berkeley_bjc%2Fintro_pair%2F2-loops-variables.topic&course=cs10_fa21.html&novideo&noreading&noassignment)
- [The RANDOM block](https://cs10.org/bjc-r/cur/programming/random/the-random-block.html?1&1&2&2&2&3&3&4&4&4&5&5&topic=berkeley_bjc%2Fintro_pair%2F2-loops-variables.topic&course=cs10_fa21.html&novideo&noreading&noassignment) + [Randomly moving a character](https://cs10.org/bjc-r/cur/programming/random/randomly-moving-character.html?1&1&2&2&2&3&3&4&4&4&5&5&topic=berkeley_bjc%2Fintro_pair%2F2-loops-variables.topic&course=cs10_fa21.html&novideo&noreading&noassignment)**

## [Block 1:  draw a polygon with (sides) sides of (length) length](https://cs10.org/bjc-r/cur/programming/functions/make-a-draw-polygon-block.html?1&2&2&3&topic=berkeley_bjc%2Fintro_pair%2F2-loops-variables.topic&course=cs10_fa21.html&novideo&noreading&noassignment)

Objective:
- Create a procedure that generalizes any polygon correctly drawing the shape, with the appropriate number of sides AND turning the appropriate angle degrees
- Your code should be able to [draw any polygon](https://cs10.org/bjc-r/cur/programming/loops/repeat-n/draw-regular-polygons-with-repeat.html?1&1&2&2&2&3&3&4&4&4&5&5&topic=berkeley_bjc%2Fintro_pair%2F2-loops-variables.topic&course=cs10_fa21.html&novideo&noreading&noassignment) (square, hexagon, octagon, etc.) on the stage

Inputs: 
- sides = number
    - This variable represents how many sides the polygon has
- length = number
    - This variable represents how long each side is

Outputs: 
- None! It is a procedure / non-pure function, so it only displays a visual effect on the stage and does not output any values
- What type of block did we use for this code? What type of block would report instead? 

Examples:   

![examples of a polygon with 4 sides of 100 length](/su25/assets/images/lab_images/lab2_b1_1.png)   
![examples of a polygon with 6 sides of 100 length](/su25/assets/images/lab_images/lab2_b1_2.png)

## [Block 2: draw a square leaved flower with (leaves) leaves of (size) size](https://cs10.org/bjc-r/cur/programming/functions/intro/composing-blocks.html?1&2&2&3&topic=berkeley_bjc%2Fintro_pair%2F2-loops-variables.topic&course=cs10_fa21.html&novideo&noreading&noassignment) 
Objective: 
- Create a procedure that creates a symmetrical flower with any number of leaves. Each leaf itself is a square. So, a series of square leaves should create a flower.

Inputs: 
- leaves = number
    - A variable that represents how many leaves or petals the flower has. Remember, each leaf is square!
- size = number
    - A variable that represents how large each leaf/square is.

Outputs: 
- None! It is a procedure / non-pure function, so it only displays a visual effect and does not output any values

Examples:  
![example of 'draw a square leaved flower with 6 leaves of 100 size'](/su25/assets/images/lab_images/lab2_b2_1.png)   
![example of 'draw a square leaved flower with 10 leaves of 100 size'](/su25/assets/images/lab_images/lab2_b2_2.png)

## Optional Block: Draw a field of flowers
Objective:  
- Create a procedure that draws a field of flowers using your creativity and artistic flair! You may use blocks you previously coded in this lab as helpers.  
- **DO NOT change the pen hue color** when attempting the flower field block, as this may interfere with the autograder.  
- When finished, take a screenshot of your drawing and upload it to this [folder](https://drive.google.com/drive/u/0/folders/1Seq9Fovej-T3OcWO2K8i_TTKc05bLcfm). All participants will receive a small prize at the next lab! 😉
