---
title: Project 1
description: Wordle™-lite
due: "11:59 PM PST on Wednesday, 2/4"
gradescope_assignment_id: 7495160
submission_files:
    - starter.xml
---

*Version 3.0. Last Updated: 2025-09-09.*

*We highly recommend reading through this spec in its entirety before you begin.*

> Any important updates or clarifications will be made here
>> Project 1 Party on Monday (2/2) from 5–8 PM and Wednesday (2/4) from 6–8 PM.

## To begin, load [this starter project](https://snap.berkeley.edu/snap/snap.html#present:Username=jedi_force&ProjectName=BJC%20CS10%20Project%201%3A%20Wordle%E2%84%A2-lite)


[Project 1 Walkthrough Guide.pdf](https://drive.google.com/file/d/1liTxubkrh5-Vtp5CbQETI9BurAquIVSx/view)

## Content

[I. Introduction](#Introductions)  
[II. Part 1: "game over" Block](#part-1-game-over-guess-secret--score--block)  
[III. Part 2: "matching slots" Block](#part-2-matching-green-slots-between-guess---and-secret--block)  
[IV. Part 3: "update score" Block](#part-3-update-score-based-on-matched-slots--and-score--block)  
[V. Rubric](#rubric)  
[VI. Feedback Form](#feedback-form)

## Submission Guidelines 

- Review the guidelines here to learn how to export your projects and turn them in. 
- Make sure to click “Add Group Member” in the top-right corner of the screen and add your partner!
- Your final score out of 10 on this project is your score on Gradescope.
- Once submitted, finish Project 1 Feedback Form 


## Preface

*Do remember that while you may discuss general ideas with other students, sharing code with anyone but your partner would be academically dishonest.*

The expected timeframe for this project is about 4 hours, with a partner.
- Read instructions - 20 minutes
- Part 1: "game over" Block - 30 minutes
- Part 2: "matching slots" Block - 1 hour
- Part 3: "update score" Block - 1 hr
- Feedback Form - 10 minutes
  
Working on this project assumes you have completed the following:
- Lecture 1
- Lecture 2
- Lecture 3
- Lab 1
- Lab 2
- Lab 3
- Discussion 1

We recommend watching Lecture 4 and completing Lab 4 beforehand too, but this is optional.

**Important: Ensure that you use the starter file we’ve linked below- do NOT create your own Snap! file for this project!**

**Note:** The Project Feedback Form will ask about how long you took at each part of the project. Please keep track of your time frame as you work through the project. For example, if you work for 30 minutes on Thursday, then 40 minutes on Saturday for part 2, you spend 1 hour and 10 minutes total on part 2. 

## Introductions 

In this project, you are required to work with **one (and only one) partner** (and with assistance from course staff as needed) to finish three blocks in an existing program to play Wordle™-lite, a word-guessing game designed for two human players.

In the game, the first player (Player 1) will enter a secret code, and the second player (Player 2) will try to guess that code. Player 2 starts with 100 points, and every wrong guess costs them 10 points, but they earn back the number of letters that match perfectly in the same place in both words (in Wordle™ this would be the green letters). This back-and-forth will continue until Player 2 successfully guesses the secret code or the score is not positive, and the game ends. 

Here is an example of the game being played (make sure to resize HISTORY to see it better):

> `Program: Welcome to Wordle™-lite, a word guessing game.  Ready player one: enter a secret word...`  
`Player 1: love`  
`Program: Ready player two: time to guess the secret word;  you start with a score of 100 (wrong guesses cost you 10 but each matched letter earns back 1); the game ends when you guess the word or the score gets to 0. What is your guess? (hint: it’s a 4-letter word)`  
`Player 2: like`  
`Program: Player two: your guess of “like” matched l--e; your score is now 92. What is your guess? (hint: it’s a 4 letter word)`  
`Player 2: lose`  
`Program: Player two: your guess of “lose” matched lo-e; your score is now 85.  What is your guess? (hint: it’s a 4 letter word)`  
`Player 2: love`  
`Program: “love” is correct, great job! Final score: 85/100`

![Example of Wordlite testcase described above, with person infront of Wheeler hall](/fa24/assets/images/wordlelite.png)

Some notes – nothing in our code prevents either Player 1 or Player 2 from typing a gibberish word. We would hope Player 1 doesn’t do that, since the game is almost impossible if the secret word is a set of random letters. However, one strategy that Player 2 might employ (and this game allows it, making it easier than the actual Wordle™ game) is to type a word (say) of all e’s to see where the e’s are in the word. Also, the guesses Player 2 enters aren’t checked to see if they’re the same length as the secret word. When the guessed word is longer, we only look at the first N slots of the guess (where N is the length of the secret word). When the guessed word is shorter, it just shows the letters that weren’t guessed as missed “-” letters.

If you’re having trouble, please contact the course staff for assistance — Ed, Office Hours, and Labs are all here to help you feel good about the work you’re doing! If you can’t make the times, tell us, and we’ll figure out how you can still get support. But, we won’t know when or how to help unless you let us know.

## **Part 1:** <game over? guess:[] secret: [] score: ()> Block

First, you’ll build a **predicate block** (aka the “game over” block) that will know when the game is over. This should report *True* if the guess equals the secret or if the score is not positive, and *False* otherwise. Here are some examples:

![Testcases for Part 1 Block](/fa24/assets/images/P1-Part1Tests.png)

## **Part 2:** (matching "green" slots between guess: [ ] and secret: []) Block 

Next, you’ll build a **reporter block** (aka the “matching slots” block) that can tell a player how close they are to guessing the secret code by indicating the correct “slots”. Capitalization should not matter (i.e., the game should read r and R as the same), but thanks to the way Snap! implemented its “=” block, you don’t have to worry about making a special case, just using “=” will treat lowercase r and uppercase R the same!

Given two inputs, a guess and a secret code, the matching slots block should report a word of letters or dashes to indicate the matching slots between guess and secret, the same length as secret, in which every matched letter is the letter itself, and any missed letter is a dash. Here are some examples to make this clear:

![Testcases for Part 2 Block](/fa24/assets/images/P1-Part2Tests.png)

## **Part 3:** (update score based on matched slots: [] and score: ()) Block


Finally, you’ll build a reporter block (aka the “update score” block) that will take the result of the matched slots and the old score and report an updated score based on the old score minus 10 (cost for a guess) plus the number of slots that matched (were not “-”). Here are some examples to make this clear:

![Testcases for Part 3 Block](/fa24/assets/images/P1-Part3Tests.png)


## Rubric 
You have three blocks to write and five tests (shown above) for each block, according to the following table. So a perfect score would earn (5 × 0.4) + (5 × 0.8) + (5 × 0.8) = 10 points. Gradescope’s autograder needs the number between 0 and 1, so we divide that score by 10 to send to the autograder. You should continue to work on your code until all test cases pass and the score reported by says: {"score": 1} 
If at any point you’d like to see more details about how we calculate that out-of-10 score, you can run the  block we provide, a, the expected value, the actual value, how many points it is worth, and how many points you’ve earned. The sum of all the earned points is tallied in the bottom-right cell.
Note: correct, working code should handle those test cases, but not have the test cases hardcoded into your solution; they should be able to handle any inputs according to the specifications.

| Block    | Points | Number of Tests |
| -------- | ------- |
| <game over? guess:[] secret: [] score: ()>                 | 0.4    | 5 |
| (matching "green" slots between guess: [ ] and secret: []) | 0.8    | 5 |
| (update score based on matched slots: [] and score: ())    | 0.8    | 5 |

## Feedback Form 
Congratulations on finishing your first project in CS10 🥳. Please spend some time completing this [feedback form](https://forms.gle/URuPr5iCYXcQqQAy9). This will be worth 1 point of your project grade. 






