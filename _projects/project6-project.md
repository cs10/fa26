---
title: Project 5
description: Final Project - The Project 
due: "11:59 PM PST on Monday, 12/7"
gradescope_assignment_id: 
submission_files:
    - N/A
---

*Version 2.0. Last Updated: 2026-10-30.*

*We highly recommend reading through this spec in its entirety before you begin.*

- You are required to attend the final project proposal meetings in person. Failure to do so will result in no points awarded for your approved features and meeting attendance, leading to a 50% deduction in your final project score.
- **Oral exams will occur in person during RRR Week (12/7-12/11) and are worth half of your overall Project 5 grade**. All project group members must be present. Time slots for the oral exams will be announced on Ed soon. Please refer to the [Oral Exams](#oral-exams) for more details.

> There are 5 components of the project:
1. Approved Project Proposal
2. The project / code itself
3. README / documentation on your project
4. Video of your group interacting with your project
5. Oral Exam

<!-- >Project 5 Party TBD -->

## Content

[I. Recommended Timeline](#recommended-timeline)

[II. Introduction](#introduction)

[III. Technical Requirements](#technical-requirements)

[IV. Required Features](#required-features)

[V. Style Requirements](#style-requirements)

[VI. README Requirements](#readme-requirements)

[VII. Video Requirements](#video-requirements)

[VIII. Submission Guidelines](#submission-guidelines)

[IX. Oral Exams](#oral-exams)

[X. Rubric & Grading](#rubric--grading)

[XI: Additional Resources](#appendix-i-additional-resources)


## Recommended Timeline

| Group with 2 Features | Group with 3 Features |
| :--------: | :-------: |
| Feature 1: 11/20  |Feature 1: 11/17   |
| Feature 2: 11/30  | Feature 2: 11/26  |
| Full Project Submission Ready: 12/3  | Feature 3: 12/2  |
| README and Submission: By 12/7  | Full Project Submission Ready: 12/4   |
|   | README and Submission: By 12/7   |


## Introduction

For your final project, you'll be turning in both code and a README. The README is a document that describes your project and its features. This project is a chance for you to implement an idea driven by your own interest!

## Technical Requirements
<!-- Here is a list of some of the technical requirements you must be able to demonstrate in the implementation of your final project: -->

- **Non-trivial list**: Your project should include at least one non-trivial list, meaning a list whose function could not be simply replaced with another implementation. This can be a tracker of high scores or part of a game board.
- **Custom block/function**: Your project should include at least TWO functions that you define yourself. 
- **Script/local variable**: Your project should include at least one <em>non-global</em> variable. 

## Required Features

On top of the technical requirement, you must have 2-3 features from the following list. If you want a feature that does not fit within the guidelines below, you will need to discuss it with your TA, but it is unlikely to be approved. If you use two of the same features they must have distinct properties. 

- 2D, Nested lists (representation of the game board, highscores, positions...)
- Extensive, dynamic visual display
    - Must include at least: 1 background, 2 sprite costumes, 1 sound, and a help screen or guide to interact with program / instructions
- Organized Text UI in Python
    - Must include a visual print statement of current state of program and a list of functions the user can (such as help, place move, restart, etc.)
- Extensive use of OOP in Python (not Snap!)
    - Most likely, all final projects completed in Snap! will use extensive OOP in Snap!, so we are not counting OOP in Snap! as a feature.
- API calls (calls to other programs or websites) - Don’t worry about doing this one; but it’s an option if you’re interested!
- Structures keeping track of important data (ex: Dictionaries, Lists, Trees, Sets)
- Complex Algorithm. Examples:
    - Merge sort
    - Determining whether a game is over
    - Determining whether a move is valid
    - Determining and displaying the top three high scores
- Extensive use of libraries (in either Python or Snap!)
    - Must use at least 3 different functions for the library imported
    - Or 3 different libraries imported, and 1 function each is used. 
- Features that DON’T COUNT (but are still okay to have in your code):
    - Randomization
    - Helper functions
    - Inputs/Outputs and Response/Prompt (i.e games that simply ask a user for a response/prompt to input)
    - Broadcasting messages
    - Pointing and clicking
<!-- ## Technical Requirements

There are certain technical and style requirements that we want you to be able to demonstrate in the implementation of your final project, regardless of what kind of project you're doing, which are listed below. For some of the rubric items, you can also mix and match (see rubric for more details). Here is a list of some of the technical requirements you must include:

- Non-trivial list: Your project should include at least one non-trivial list, meaning a list whose function could not be simply replaced with another implementation. Often this can be a tracker of high scores, or part of a game board.
- Custom block/function: Your project should include at least TWO functions that you define yourself. There is no restriction on what type of function this should be, whatever suits your project is what you should do!
- Script/local variable: Your project should include at least one non-global variable.  -->


## Style Requirements

<!-- This is a list of what style markers you should aim for: -->
- **Commenting** -- We require clear and coherent comments for the following purposes:
    - Describing how to start/run the program: Often, this is the green flag for Snap!, and typing a command into the terminal for Python. Make sure to specify what to do, even if it seems obvious! Make sure this is in both your code as a comment and in your README file. 
    - For each function or block you’ve written: An explanation of its inputs + outputs or what data it changes if applicable.
    - Here’s a [guide](https://docs.google.com/document/u/1/d/e/2PACX-1vSrtiqOPprVJ327uvCj9aRGXJYGP9hjOMJyz_vSxK237PNnTCYumvE24QYcbmA_Xy8voUPOqHzXtZOO/pub?embedded=true) for reference!
- **Variables & functions**
    - Variable scope: Make sure you’re only using global variables when absolutely necessary (i.e., when they need to be referenced at multiple points in the program, or by multiple functions). Try to use script/local variables where possible. 
    - Naming convention: Keep function and variable names clear, by specifying what they do or represent. A good rule of thumb is to give things names in a way that would still make sense to you if you needed to explain this project to someone else in a year. For example, a variable could be called “highScore” if it keeps track of the highest score so far. 
- **Abstraction & generalization** — These are key computing ideas for a reason! Do your best to apply these principles as you code. This will look like:
    - Generalizing code: If you can use a for-loop or a HOF or a helper function to prevent copy-pasting similar code, do it!
    - Abstraction: Break down functions/features into smaller, concise pieces. Each function/feature should focus on achieving a specific task. 
        - If you find yourself with repetitive code, consider how you can abstract the part that is repeated. 



## README Requirements

Your README is a project guide and will be used as a reference for grading. The template and instructions can be found [here](https://docs.google.com/document/d/1GiZ6tE-mnezyiry7p_gmEswNRfx7ntNjT3Z-wcfZToA/edit?tab=t.0). Please make a copy of the Google Doc to work on, and make sure to submit it as a **PDF**. 

**[Optional] Bug Writeup**: Sometimes, despite your best efforts, the project deadline rolls around and one or more of your features isn’t working correctly. This happens in industry as well — think about app updates you’ve downloaded! 

Not to fret, you can earn back up to 75% of the points originally lost for a non-functional feature with a thorough write-up. Here’s an [example](https://docs.google.com/document/d/1A6Tzm0UZte8gMnnmE2PV1J9xO__z6SaLkDVA6j3-I5s/edit?tab=t.0) of what we’re looking for in a bug writeup, based on a function you wrote for the OOP lab.
<!-- (Points given will depend on the size of the bug; this is meant to limit the points penalty for not implementing a bug-free project feature.)  -->

## Video Requirements
Your video is a supplement of your README. Please demonstrate exactly how to run your project, the controls, and each of the features. If you are completing a Bug write-up, please demonstrate the bug(s). Your video must be under 3 minutes for full credit.

You may either submit your video via Google Drive or YouTube (unlisted video). If you are submitting through Google Drive please make sure to share your video with staff from the course website. 

*Include the link to your video in your README. If we do not have access to your video you will not get credit for this portion of the assignment.* 

Final Project Demo Examples: [Python](https://www.youtube.com/watch?v=UsjNnCpaTSQ&ab_channel=DorottyaUrmossy) and [Snap!](https://youtu.be/lzp4td5FGzo)

## Submission Guidelines

You should submit 2 things to Gradescope:
1. **README**: Using the template above and an embedded link to your video. Submitted as a PDF, we will not accept .docx files or Drive links, etc.
2. **Project code**:

- *Snap! projects*: 
    - Download the .xml file using File > Export Project.
    - Rename the file to FirstPartner_SecondPartner_FinalProject.xml and upload directly to Gradescope. (Adjust accordingly if you are solo or in a group of 3)

- *Python projects*:
    - Put the .py file(s) containing your project code along with other media (images, sounds, etc.) into a ZIP folder.
    - Rename the ZIP folder FirstPartner_SecondPartner_FinalProject.zip and upload the ZIP file to Gradescope. 
    - Feel free to Google "How to make a .zip file" / ask for help on Ed.

**If you run into any issues submitting, go to a lab or office hours or make a private post on Ed**

## Oral Exams
Staff will be conducting **15-20 minute in-person oral exams during RRR Week (12/7-12/11)** for each group. These exams are an opportunity for you to demonstrate your understanding of your project code.

**All group members are required to attend (NOT Berkeley Time)**. We will announce sign-up details and available time slots on Ed. You may have your code open for reference, but you may not bring any additional notes. 

This is worth **30 points (half of your Project 5 grade)**. Make sure that all group members are familiar with the entire project, even if you divided up the work. All code must be completed by your group members and must follow the course’s [Generative AI and academic honesty policies](https://cs10.org/fa26/syllabus/#academic-integrity). Failure to follow these policies will result in serious consequences, even if the violation involves a portion of the project completed by another group member. 

 
## Rubric & Grading

Project 5 is worth 60 points, graded for style and technical correctness. 
<!-- After you get your grades, you may submit regrade requests via Gradescope. -->

Please don't forget to add your partner(s) to the submissions! [How to add a partner to Gradescope.](/fa25/assets/images/p6/p6-1.png)

| Project Proposal | (5 pts) |
| -------- | ------- |
| +5 | Project Proposal is approved |

| Oral Exam | (30 pts) |
| -------- | ------- |

| README | (5 pts) |
| -------- | ------- |
| +1 | README contains features description |
| +1  | README contains complexity justification |
| +1  | README contains variable justification |
| +1  | README contains blocks/functions table |
| +1  | README or code comments describe program controls  |

| Features  | (7.5 pts) |
| -------- | ------- |
| +3.25 / feature | Groups of 1-2, who implemented two (2) features |
| -3.25 / feature | If the feature implemented was not approved by TA (for groups implementing 2 features). |
| +2.5 / feature  | Groups of 2-3, who implemented three (3) features |
| -2.5 / feature| If the feature implemented was not approved by TA (for groups implementing 3 features). |
| -1.5 / bug | For each major bug (project-breaking/crashing)|
| -0.5 / bug | For each minor bug (errors only on specific input or subpart of feature)|
| +1 / bug | *Optional* Bug writeup for a major bug (see README)|
| +0.5 / bug | *Optional* Bug writeup for a minor bug (see README)|

| Technical Requirements | (7.5 pts) |
| -------- | ------- |
| +2 | Req 1: Custom function |
| +2  | Req 2: Custom function |
| +1.75  | Req 3: Non-trivial list |
| +1.75  | Req 4: 1 or more script or local variable(s) |

| Style Requirements | (2.5 pts) |
| -------- | ------- |
| +1 | Useful and coherent comments |
| -0.5  | Comments are disorganized / incoherent but present |
| +1  | No repetitive code / good use of helper blocks or functions |
| +0.5  | Clear and useful variable and block names |

| Project Demo Video | (2.5 pts) |
| -------- | ------- |
| +1 | Video contains how to run the project |
| +0.75  | Video contains how to use program controls |
| +0.75  | Video contains demonstration for each feature  |
| -0.5  | Video is longer than 3 minutes |


## Appendix I: Additional Resources
- Please Attend OH or Final Project Parties 
- [README Template](https://docs.google.com/document/d/1GiZ6tE-mnezyiry7p_gmEswNRfx7ntNjT3Z-wcfZToA/edit?tab=t.0)
- [Bug Writeup](https://docs.google.com/document/d/1A6Tzm0UZte8gMnnmE2PV1J9xO__z6SaLkDVA6j3-I5s/edit?usp=sharing)
- [Project Proposal Spec](https://cs10.org/fa25/projects/project6-proposals/) 
- [Commenting Guide](https://docs.google.com/document/u/1/d/e/2PACX-1vSrtiqOPprVJ327uvCj9aRGXJYGP9hjOMJyz_vSxK237PNnTCYumvE24QYcbmA_Xy8voUPOqHzXtZOO/pub?embedded=true)