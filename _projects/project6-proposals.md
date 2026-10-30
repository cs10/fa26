---
title: Project 5
description: Final Project Proposals
due: "11:59 PM PST on Friday, 11/6"
gradescope_assignment_id: 6577061
submission_files:
    - N/A
---

*Version 2.0. Last Updated: 2026-10-29.*

*We highly recommend reading through this spec in its entirety before you begin.*





## Content

[I. Important logistics](#important-logistics)

[II. Introduction](#introduction)

[III. Required Features](#required-features)

[IV. Proposal Contents](#proposal-contents)

[V. Complexity Guidelines](#complexity-guidelines)

[VI. Submission Guidelines](#submission-guidelines)

[VII. Proposal Review: What to Expect](#proposal-review-what-to-expect)

## Important logistics

**Project Groups**
- You must work in groups of 2. Groups of 3 require TA approval and we will increase their project-complexity requirements. 
- If you want to work alone you must get explicit permission from your lab TA and you will still be graded as a group of 2. This is a complicated project and we very rarely permit students to work solo. 
**Proposal Submission Due Friday 11/6**
- Submit your proposal on Gradescope *before* your meeting.
- The proposal should come to about 1-2 pages, single-spaced. 
- There will be NO extensions available for the proposal
- You can revise and resubmit until your meeting time. Your proposal will be graded based on the content discussed during the meeting.
**Meeting Sign Up Due Friday 11/6**
- Book a 10-minute slot on Google Calendar by Friday, 11/6 at 11:59 PM PST (released soon)
<!-- - To schedule a booking, click here for the booking page: [Proposal Meeting Sign-ups](https://calendar.app.google/wB8NA3KBW1jGhodq9). -->
- If all slots are full or you cannot attend, make a private Ed post by the 11/6 deadline to avoid a 0 score.
**Projetc Proposal Meeting Details (Week 12: Nov 9 -13)**
- Meetings will run during Week 12 (Monday November 9th through Friday November 13th). No meetings on Wednesday November 11 holiday
- You may attend the either in person (location TBD)or via Zoom.
-  The Project Proposal Meeting is worth 5 points of your final grade.
- Only one member of your group needs to attend. Late arrivals receive a '0' score and must sign up for a new time slot.


## Introduction

For the final project, you’ll be building a project that you envision in either Snap! or Python, completely from scratch (how cool is that!) First, you’ll need to submit a project proposal that will be reviewed by a staff member to ensure that your project won’t be too easy or complex. 
This proposal is meant to be just an ideas-focused starting point — the spec for the technical requirements of the final project can be found [here](https://cs10.org/fa26/projects/project6-project/)

You will receive a 0 for Project 5 if you do not submit your proposal and meet with a staff member.

## Technical Requirements

There are certain technical and style requirements that we want you to be able to demonstrate in the implementation of your final project, regardless of what kind of project you’re doing, which are listed below. For some of the rubric items, you can also mix and match (see rubric for more details). Here is a list of some of the technical requirements you must include:

- Non-trivial list: Your project should include at least one non-trivial list, meaning a list whose function could not be simply replaced with another implementation. Often this can be a tracker of high scores, or part of a game board.
- Custom block/function: Your project should include at least TWO functions that you define yourself. There is no restriction on what type of function this should be, whatever suits your project is what you should do!
- Script/local variable: Your project should include at least one <em>non-global</em> variable. 

## Required Features

On top of the technical requirement your project must have required features. Here is a list of approved features. Your 2-3 features MUST be from the following list. If you are proposing to have a feature that does not fit within the guidelines below, you will need to discuss it with your TA, but it is unlikely to be approved. If you use two of the same features they must be distinct and have unique properties. 

- 2D, Nested lists. The nested list can be a representation of the game board, highscores, positions, or some other structure
- Extensive, dynamic visual display
    - Must include: 
        - At least one background
        - At least two sprite costumes
        - At least one sound
        - A help screen or guide to interact with program / instructions
- Organized Text UI in Python
    - Must include:
        - A visual print statement of current state of program
        - A list of functions the user can (such as help, place move, restart, etc.)
- Extensive use of OOP in Python (not Snap!)
    - The main logic of the name would use an OOP structure
    - Most likely, all final projects completed in Snap! will need to use extensive OOP in Snap!, so we are not counting OOP in Snap! as a feature.
- API calls (calls to other programs or websites) - Don’t worry about doing this one; but it’s an option if you’re interested!
- Structures keeping track of important data
    - Examples: Dictionaries, Lists, Trees, Sets
- Complex Algorithm
    - Examples:
        - Merge sort algorithm
        - Determining whether a game is over condition
        - Determining whether a move is valid
        - Determining and displaying the top three (or some number) of high scores
- Extensive use of libraries (in either Python or Snap!)
    - Must use at least three different functions for the library imported
    - Or three different libraries imported, and one function each is used. 
- An AI that runs the program/plays game and tries to optimize for winning moves
- Features that DON’T COUNT:
    - Randomization (it’s completely okay to have randomization, but it doesn’t count as a feature)
    - Helper functions
    - Inputs/Outputs and Response/Prompt
        - Example: Games that simply ask a user for a response/prompt to input
    - Broadcasting messages
    - Pointing and clicking


## Complexity Guidelines

Complexity means “how difficult is it to implement?” and is used as a measurement to ensure that final projects fit a happy medium of not too hard and not too simple.
If your project idea relies heavily on the following, we recommend you consider alternate projects:
- Using any primitive block in Snap! Will not count as a feature
- Mainly being a guess-and-check game: This is considered too easy since it consists primarily of a series of if-then-else statements (ex: number guessing game). This might be a good mini-game in a bigger project.
- Data entry: Projects that rely on data entry get ‘bigger’ by having a bigger database. A fix for this would be having the data component be just one part of a bigger project. 
- Games like Pong, Tic-Tac-Toe, Guess the word, Hangman, dress-up games, point and click games would not be complex enough and are NOT ALLOWED.
- Games like Angry Birds, Balloons Tower Defense, or Need for Speed would likely be too complex. 
- Games previously implemented in Projects are not allowed.
- Use of AI is NOT allowed.

Don’t be worried if you really like a project idea but think it may be too complex, or not complex enough — that’s the purpose of the project proposal, so you can work with a TA to get your project complexity into the right range! 

When considering what your project is, see if you can figure out a solution or a structure for a solution first! A few gauges for complexity are: coming up with logic to check for four-in-a-row in Connect 4 or recreating Flappy Bird in Snap!

Here are some examples of projects in the "accepted proposal" range

- [The Chrome Dinosaur Game:](https://chromedino.com/)
    - Feature 1: TWO DIFFERENT OBSTACLES 
        - Randomly generated shrubs and pterodactyls appear on the screen as obstacles.
        - Obstacles NEED to be traveling at different speeds (otherwise project will not be complex enough)
    - Feature 2: The game ends when the dinosaur runs into an object.
- [Mancala:](https://www.mathplayground.com/mancala.html)
    - Feature 1: When a player chooses a group of marbles, those marbles get distributed around the board, picking up more marbles when the last one falls on a non-empty hole
    - Feature 2: Game over when all marbles are in the two goals, winner is the one with more marbles
- [Doodle Jump:](http://poki.com/en/g/doodle-jump)
    - Feature 1: Doodle jumps continuously, moving higher up in the sky as he lands on bouncing platforms that continuously move downwards
    - Feature 2: Game ends when Doodle falls off the screen
- [Bubble Shooter (Difficult):](http://www.shooter-bubble.com/)
    - Feature 1: Computer will generate randomly colored bubbles that players can shoot
    - Feature 2: If the program detects groups of the same color, it will delete them.

Other projects that fit complexity requirements that students have done in the past include: Frogger, Checkers, Flappy Bird, Snake, Chutes & Ladders, various puzzle games, various board games, data science analysis, Battleship, and chatbots.


## Proposal Contents 

So now that you’ve got a project idea in mind, it’s time to write about it! We recommend you draft your answers out on a Doc before submitting them into Gradescope.

- Who are the group members (name and SID)?
- What language will your project be in? Python or Snap? If you’re doing a graphics-heavy project, we recommend Snap!, as staff will have limited capacity to assist with debugging Python libraries. If you’re not sure, pick whichever you and your group feels more comfortable coding in, and you can check in with your TA/tutor about it later. 
- What is your vision for the project? Describe the specific project and the major 2-3 features (listed above) you’d like to accomplish. Groups of 2 should list 2 features, groups of 3 should list 3. Please go into detail on this one, even if you think your project is well-known! The clearer you are, the better your TA/tutor will be able to help you adjust the project if it falls outside the optimal range of complexity. 
- How will someone interact with your project? Describe the controls that will be used. For Projects 1-2, the answer to this question would be text input via keyboard. For Project 3, the answer would be keyboard controls/arrow keys. 
- What are the technical elements behind your features? Go into more detail about your preliminary thoughts about how you’ll make the 2-3 features happen. What you come up with here doesn’t have to be exactly what you end up doing, but it should convey how you plan on implementing the project in terms of blocks/functions or computing ideas. For example, Pytris utilizes object-oriented programming to build and abstract different elements of the game.

Here is an [example proposal](https://docs.google.com/document/d/1IBLwmPiIa9qJ3p1Jvg6o23CnJNGfK0Jr0xQbZg9nMNM/edit?usp=sharing); it should give a sense of how much detail we want you to go into on the proposal. Feel free to make a copy. 


## Submission Guidelines

By Friday, November 6th 11:59pm, you and your partner will submit your project proposal as a group on Gradescope. Only one person needs to submit, don’t forget to add your partner(s) to the submissions!

![How to add partner to Gradescope](/fa25/assets/images/p6/p6-1.png)


## Proposal Review: What to Expect

You will explain your project and a staff member will review your project proposal, and either approve or disapprove it. Regardless of the status of your project proposal, you must attend the project proposal review meeting with a TA/tutor. 


If your initial project proposal is not approved: 

- It’s okay! This happens to lots of students every semester, and really just means that you’ll have to adapt your idea a bit to ensure it fits our complexity requirements, which the staff member you meet with for your proposal review will help you with. If you decide you’d rather pursue a different project idea, please note that you’ll need to write up another project proposal, and have that approved before you can start working. 
Note: If you choose not to adjust your project as suggested or do not submit a second proposal when your idea changes, you are unlikely to receive full credit for complexity.

If your initial project proposal is approved: 

- Congrats! You can start working on your project. Note any questions (for resources, clarifications, or suggestions/advice on implementation) that you might have for your project TA/tutor, and bring them up during your proposal review session!

As you begin to code, you may feel the need to make adjustments to your project and features (often because of time constraints or unexpected complexity). This is perfectly okay! You don’t have to run the changes by your project TA/tutor to start implementing them, but we do recommend that you check in with any adjustments to ensure that you are still within complexity guidelines.





