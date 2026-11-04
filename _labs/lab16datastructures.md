---
title: "Lab 15"
description: "Data Structures in Python"
due: "Thursday, April 9th, 11:59PM"
gradescope_assignment_id:
submission_files:
---

# Lab 15: Data Structures in Python

## Instructions
This worksheet serves as a guide and set of instructions to complete the lab.

- You must use the [starter file](https://cs10.org/bjc-r/prog/python/lab2starter.py), found here, to get credit for the lab (the file is named lab2starter.py but don't worry about that).
- Additionally, [here is the workbook](https://cs10.org/bjc-r/cur/programming/python/intro_besides_blocks_data_structs.html?topic=berkeley_bjc%2Fpython%2Fbesides-blocks-data-struct.topic&course&novideo&noreading&noassignment) that you can read through for further context and additional (non-required) material.
- All material was sourced from the CS10 version of The Beauty and Joy of Computing course.

## Submitting
You will need to complete **Exercises 1-7.2** and submit this to Gradescope.

- To receive full credit, you will need to complete the required functions, and the required functions must pass all tests from the autograder in Gradescope.

Please note, you must use the [starter file](https://cs10.org/bjc-r/prog/python/lab2starter.py), and you must NOT edit the name of any of the required functions. Failing to do either for these will result in the autograder failing.

## Running Doctests
To run doctests embedded within the docstring of a function, you can use the command:

```
python3 -m doctest -v <filename>.py
```

To run all doctests you can run:

```
python3 -m doctest <filename>.py
```

## Objectives
In this lab, we'll explore data structures in Python. While Snap! mainly uses lists as its only data structure, Python offers more options, such as lists and dictionaries. You can think of dictionaries as more powerful lists. The goal of this lab is to help you become familiar with creating and using these data structures, as well as utilizing Python's built-in functions to solve data-related problems.

In today's lab you will:

- Practice writing functions in Python.
- Manipulate simple data structures and their data.
- Learn how to use key-value pairs and determine why they are useful.
- Solve problems with Python lists and dictionaries

## Required Functions
- Function 1: push_first_odd_back(lst)
- Function 2: flatten(lst)
- Function 3.1: squares_of_evens(lst)
- Function 3.2: nth_power_of_evens(lst, n)
- Function 4: substitute_base(string, old, new)
- Function 5: combine(items)
- Function 6: base_freq(sequence)
- Function 7.1: substitute_chars(string, replacements)
- Function 7.2: invert_dict(original)

---

## Important Topics (Workbook)
For better understanding of the lab we highly recommend going through these workbook pages! Topics that are important but not required for this lab will be indicated with an asterisk (**). These topics are best reviewed in order and as you complete the lab.

- [Basic List Operations](https://cs10.org/bjc-r/cur/programming/python/lists_intro.html?topic=berkeley_bjc%2Fpython%2Fbesides-blocks-data-struct.topic&course&novideo&noreading&noassignment)
- [List Mutability](https://cs10.org/bjc-r/cur/programming/python/list_mutability.html?topic=berkeley_bjc%2Fpython%2Fbesides-blocks-data-struct.topic&course&novideo&noreading&noassignment)
- [List Functions](https://cs10.org/bjc-r/cur/programming/python/list_functions.html?topic=berkeley_bjc%2Fpython%2Fbesides-blocks-data-struct.topic&course&novideo&noreading&noassignment)
- [Iterables](https://cs10.org/bjc-r/cur/programming/python/python_iterables.html?topic=berkeley_bjc%2Fpython%2Fbesides-blocks-data-struct.topic&course&novideo&noreading&noassignment)
- [Lists vs Dictionaries](https://cs10.org/bjc-r/cur/programming/python/comparing_dicts_lists.html?topic=berkeley_bjc%2Fpython%2Fbesides-blocks-data-struct.topic&course&novideo&noreading&noassignment)
- [How To Use Dictionaries](https://cs10.org/bjc-r/cur/programming/python/using_dictionaries.html?topic=berkeley_bjc%2Fpython%2Fbesides-blocks-data-struct.topic&course&novideo&noreading&noassignment)

---

## Exercise 1: push_first_odd_back(lst)

**Objective**  
Create a function that moves the first odd number in the input list to the end of the list

**Notes**
- The pop() function may be useful here
- We are not returning anything, but rather modifying our input list

**Inputs**
- lst = List of numbers

**Output**
- Reports: nothing
- *This function shouldn't return anything*

**Examples**
- Doctests available
  - `python3 -m doctest <labfilename>.py` to run autograder
  - Must be in correct parent file

---

## Exercise 2: flatten(lst)

**Objective**  
Create a function that takes a 2D list (a list of lists) and returns a new 1D list containing all the elements combined together in order, one after the other (i.e., concatenated)

**Notes**
- The append() function could be useful here

**Inputs**
- lst = List of lists

**Output**
- Reports: list
- Your output list should be a 1-D version of the input list

**Examples**
- Doctests available
  - `python3 -m doctest <labfilename>.py` to run autograder
  - Must be in correct parent file

---

## Exercise 3.1: squares_of_evens(lst)

**Objective**  
Create a function that takes in a list of numbers, and returns a list that contains the squares of all even numbers from the input list

**Notes**
- ***You must use list comprehension***
  - Not doing so will result in a failing autograder

**Inputs**
- lst = List of numbers

**Output**
- Reports: List
- Your output should be a list containing the squares of all even numbers found from the input list

**Examples**
- Doctests available
  - `python3 -m doctest <labfilename>.py` to run autograder
  - Must be in correct parent file

---

## Exercise 3.2: nth_power_of_evens(lst, n)

**Objective**  
Create a function that takes an input integer n as well as a list of numbers, and returns a list that contains the nth power of all even numbers found in the input list

**Notes**
- ***You must use list comprehension***
  - Not doing so will result in a failing autograder

**Inputs**
- lst = List of numbers
- n = some integer >= 0

**Output**
- Reports: List
- Your output should be a list containing all even numbers found from the input list to the nth power

**Examples**
- Doctests available
  - `python3 -m doctest <labfilename>.py` to run autograder
  - Must be in correct parent file
- **Requires flatten to pass local doctests!**

---

## Exercise 4: substitute_base(string, old, new)

**Objective**  
Create a function that takes in a string and replaces all characters that match (old) with the the character (new)

**Notes**
- Use of the replace() function is *prohibited*
- Use list comprehension along with "".join() for a clean/efficient solution

**Inputs**
- string = some string
- old = the character to be replaced. A single character
- new = the character(s) to replace the 'old' character with

**Output**
- Reports: string
- Your output should be a string with the proper characters substituted

**Examples**
- Doctests available
  - `python3 -m doctest <labfilename>.py` to run autograder
  - Must be in correct parent file

---

## Exercise 5: combine(items)

**Objective**  
Recreate your own version of combine in Python that takes in a list of numbers OR strings and returns the combined result.

**Notes**
- Use reduce from the functools library is *prohibited*
- Think about what the + operator does for strings and for numbers.
- For the most elegant solution, use **recursion**
  - **The rough equivalent of "all but first of" in Python is list[1:]**

**Inputs**
- items = List of numbers OR strings

**Output**
- Reports: integer, float, or string
- Your output should be the combined result of the items

**Examples**
- Doctests available
  - `python3 -m doctest <labfilename>.py` to run autograder
  - Must be in correct parent file

---

## Exercise 6: base_freq(sequence)

**Objective**  
Create a function that counts how many times each character appears

**Notes**
- Dictionary keys are unique, each character should only have 1 counter
- Add to the value stored in a dictionary by using:
  - `dictionary_name[key] += x`

**Inputs**
- sequence = string or list

**Output**
- Reports: Dictionary
- Your output should report a dictionary where the key is a unique character and the value is how many times that character appears in the sequence

**Examples**
- Doctests available
  - `python3 -m doctest <labfilename>.py` to run autograder
  - Must be in correct parent file

---

## Exercise 7.1: substitute_chars(string, replacements)

**Objective**  
Create a function that takes as input a string and a dictionary. The dictionary will have characters both as keys and values, which represent what to replace certain characters with. This function should return a string with each character substituted with that character's value from the dictionary. If a character doesn't exist as a key in the dictionary, it should be left alone.

**Inputs**
- string = some String
- replacements = a Dictionary with characters both as keys and values

**Output**
- Reports: String
- Your output should be a string with all appropriate characters replaced

**Examples**
- Doctests available
  - `python3 -m doctest <labfilename>.py` to run autograder
  - Must be in correct parent file

---

## Exercise 7.2: invert_dict(original)

**Objective**  
Create a function that takes in a dictionary, and reverses all key value pairs

**Notes**
- Dictionary comprehension is very similar to list comprehension!
- What happens when multiple values across the dictionary are identical?
  - Remember that keys in dictionaries are unique
- Feel free to use *python dictionary comprehension*

**Inputs**
- original = some dictionary

**Output**
- Reports: Dictionary
- Your output should report a dictionary where the keys and values are inverted

**Examples**
- Doctests available
  - `python3 -m doctest <labfilename>.py` to run autograder
  - Must be in correct parent file

---

**You can always check the validity of your solutions by using the local autograder. Remember to submit on Gradescope!**
