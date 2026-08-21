---
title: "Lab 13"
description: "OOP in Snap!"
due:
gradescope_assignment_id:
submission_files:
---

# Lab 13: OOP in Snap! (Optional)

## Instructions
- There is no workbook for this lab.
- [Here is an optional starter file](https://snap.berkeley.edu/snap/snap.html#present:Username=jedi_force&ProjectName=Lab%2013%3a%20Starter%20%28OOP%20in%20Snap%21%29&editMode&noRun). You are not required to use it, but you can!

## Submitting
There is no submission required for this lab.

## Objectives
In this lab, you will practice Object-Oriented Programming (OOP) concepts through Snap! By the end of the lab, you will:

- Learn to use clones to create interactive objects.
- Use message broadcasting to trigger actions between sprites.
- Create sprite-specific functions and variables.
- Develop your own interactive balloon shooting game.

## Demo Video
[Here's a video demo](https://drive.google.com/file/d/1pnuT4K6nq0uLBIoWTEpNUgrj-OqKie12/view?usp=sharing) of how it should work.

- Feel free to customize it in whatever way you like though!

---

## Sections

### 1. Create Clones to shoot Balloons at the Target

**Objective**  
Create clones of your sprite to shoot balloons at targets. Each clone should be able to independently shoot balloons.

**Steps**
- Create a sprite called "Balloon Shooter."
- Create a sprite called "Balloon"
- Create a script that will generate clones of your Balloon. You can do this by using the "create clone of myself" block.
- When each clone is created, it will shoot balloons toward a target.
- To make the clone move or interact, you will need the "When I start as a clone" block

**Helpful Tips**
- You may find it helpful to check how many clones you're creating and only create more if your sprite has less than a certain number. It's very easy to make a thousand clones in 1 second!
- You may find the following two blocks helpful to get a list of your clones, or ask what the x, y positions are of the clones:
  - ![clone helper blocks]({{ site.baseurl }}/assets/images/lab_images/lab14_1.png)
  - ![clone helper blocks 2]({{ site.baseurl }}/assets/images/lab_images/lab14_2.png)
- Here's an example:
  - ![clone example]({{ site.baseurl }}/assets/images/lab_images/lab14_3.png)

**Fun Tip**  
You can make your clones "laugh" or say funny things like "Take that!" every time they shoot a balloon! You can also delete clones if you have to many or if they reach their "target"

---

### 2. Use Message Broadcasting to Trigger Actions

**Objective**  
Use message broadcasting to trigger actions between sprites. When a balloon hits the target, the target should react.

**Steps**
- Create a new sprite called "Target."
- In the Balloon Shooter sprite, broadcast a message when the balloon hits the target.
- In the Target sprite, add a script to react when it receives the message. For example, change size or play a sound.

**Fun Tip**  
You can add an additional broadcast message so that when the Target sprite receives the message, it then broadcasts a message of its own back to the Balloon Shooter sprite.

---

### 3. Create 1 Function and 1 Global Variable for One Sprite

**Objective**  
Create a custom function and a global variable that is specific to one sprite. For example, you could create a function to check the number of balloons thrown, and a variable to keep track of how many times the sprite has been hit.

**Steps**
- Create a global variable "hit count" to keep track of how many times the sprite has been hit by a balloon.
- Create a custom function "check hits" to check if the sprite has been hit more than three times. If so, make it react in some way (e.g., say something or change size).

**Fun Tip**  
Make the sprite "faint" or make a funny sound after it's been hit too many times!

---

## Additional Challenges (Optional)

- **Add a score system**: Track how many successful hits you have made on the target and display the score on the screen.
- **Add movement**: Make the Water Balloon Shooter sprite move around the screen by adding keyboard controls.
- **Add special effects**: Use sounds, colors, or animations when shooting water balloons or when the target is hit.

---
