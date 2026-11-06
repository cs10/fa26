---
title: "Lab 17"
description: "Data Structures and Text Processing in Python"
due: "Tuesday, November 17th, 11:59PM"
gradescope_assignment_id:
submission_files:
---

# Lab 17: Data Structures and Text Processing in Python

> **Heads up: this lab is longer than usual!** Lab 17 combines what used to be two separate labs into one, since there is only one lab this week due to the holiday. To give you enough time to finish both parts, it is due **in one week, Tuesday, November 17th, 11:59PM**. We recommend starting early and pacing yourself.

## Instructions
This worksheet serves as a guide and set of instructions to complete the lab. This lab has two parts: **Part 1** covers data structures (lists and dictionaries) and **Part 2** covers text processing. Both parts live in the same starter file and are submitted together.

- You must use the [starter file](https://cs10.org/bjc-r/prog/python/lab17starter.zip), found here, to get credit for the lab. It contains a single file, `lab17starter.py`, with the functions for both parts, plus the text files you need for Part 2.
- Additionally, here are the workbooks that you can read through for further context and additional (non-required) material:
  - [Data Structures workbook](https://cs10.org/bjc-r/cur/programming/python/intro_besides_blocks_data_structs.html?topic=berkeley_bjc%2Fpython%2Fbesides-blocks-data-struct.topic&course&novideo&noreading&noassignment) (Part 1)
  - [Text Processing workbook](https://cs10.org/bjc-r/cur/programming/python/hug_text_processing/python_text_processing_intro.html?topic=berkeley_bjc%2Fpython%2Fbesides-blocks-text-processing.topic&course&novideo&noreading&noassignment) (Part 2)
- All material was sourced from the CS10 version of The Beauty and Joy of Computing course.

## Getting Started

Create a new folder called "datalab" on your computer (the name doesn't actually matter, but these instructions assume that's the name you use).

Download the [starter files](https://cs10.org/bjc-r/prog/python/lab17starter.zip) for this lab and unzip the file into the datalab folder. DO NOT modify/delete comments found in the starter code. You can unzip this file through the command line by using the unzip command. Remember if you're working on a Windows machine use dir instead of ls.

![terminal unzip example]({{ site.baseurl }}/assets/images/lab_images/lab18_1.png)

Part 2 reads text files (such as `gettysburg.txt`), so **run your code and doctests from inside the datalab folder**, where the text files and `lab17starter.py` live together.

## Submitting
You will need to complete **Exercises 1-14** (listed below) and submit `lab17starter.py` to Gradescope.

- To receive full credit, you will need to complete the required functions, and the required functions must pass all tests from the autograder in Gradescope.

Please note, you must use the [starter file](https://cs10.org/bjc-r/prog/python/lab17starter.zip), and you must NOT edit the name of any of the required functions. Failing to do either for these will result in the autograder failing.

## Running Doctests
To run doctests embedded within the docstring of a function, you can use the command:

```
python3 -m doctest -v <filename>.py
```

To run all doctests you can run:

```
python3 -m doctest <filename>.py
```

To run the sanity tests on all functions in this lab, navigate to the directory that contains your starter code file and type `python3 -m doctest lab17starter.py` in terminal. (Functions you haven't written yet will fail their tests until you complete them, and the optional functions in the starter file are not required.)

## Objectives
In this lab, we'll explore data structures in Python and then use them to process real-world text. While Snap! mainly uses lists as its only data structure, Python offers more options, such as lists and dictionaries. You can think of dictionaries as more powerful lists. 

One of the most interesting and important things we can do as a programmer is manipulate and analyze real world data. Python is a particularly great language for data processing, because of the very powerful open source data manipulation libraries available online. Installing such libraries is beyond the scope of this course (see CS61A and/or DATA C8 instead), so we'll be working mostly with libraries that are built into Python.

Text processing involves the analysis and manipulation of textual data, transforming raw text into structured information. By leveraging text processing techniques, we can extract meaning, identify patterns, and prepare data for further analysis or AI applications. 

In today's lab you will:

- Practice writing functions in Python.
- Manipulate simple data structures and their data.
- Learn how to use key-value pairs and determine why they are useful.
- Solve problems with Python lists and dictionaries
- Explore the fundamentals of text processing to manage and analyze text data effectively
- Learn to read and preprocess text from files using Python
- Use text processing techniques to extract insights from text data.

## Required Functions

Functions marked **(OPTIONAL)** are included in the starter file for extra practice but are **not required** and do not count toward credit.

**Part 1: Data Structures**
- Function 1: push_first_odd_back(lst)
- Function 2: flatten(lst)
- (OPTIONAL) Function: flatten_ND(lst)
- Function 3.1: squares_of_evens(lst)
- Function 3.2: nth_power_of_evens(lst, n)
- Function 4: substitute_base(string, old, new)
- Function 5: combine(items)
- Function 6: base_freq(sequence)
- Function 7.1: substitute_chars(string, replacements)
- Function 7.2: invert_dict(original)
- (OPTIONAL) Function: sum_columns(board)
- (OPTIONAL) Function: binary_search(numbers, target)
- (OPTIONAL) Function: count_paths(level)

**Part 2: Text Processing**
- read_file(filename) [required but code is [given](https://cs10.org/bjc-r/cur/programming/python/hug_text_processing/python_basic_files.html?topic=berkeley_bjc%2Fpython%2Fbesides-blocks-text-processing.topic&course&novideo&noreading&noassignment)]
- Function 8: pig_latin(word)
- Function 9: izzle(word)
- Function 10: apply_language_game(text, language_game)
- Function 11: count_words(text)
- Function 12: top_n_words(counts, n)
- Function 13: print_top_n_words(counts, n)
- (OPTIONAL) Function: top_n_words_except(counts, n, boring)
- Function 14: average_word_length(counts)
- (OPTIONAL) Function: word_diversity(counts)
- (OPTIONAL) Function: get_kgram(text, ptr, k)
- (OPTIONAL) Function: process_character(m, text, ptr, k)
- (OPTIONAL) Function: build_markov_model(text, k)

---

# Part 1: Data Structures

## Important Topics (Workbook)
For better understanding of Part 1 we highly recommend going through these workbook pages! Topics that are important but not required for this lab will be indicated with an asterisk (**). These topics are best reviewed in order and as you complete the lab.

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
Create a function that takes in a string and replaces all characters that match (old) with the character(s) (new)

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

# Part 2: Text Processing

Now that you're comfortable with lists and dictionaries, let's put them to work on real text data! Please go through [the entire text processing workbook](https://cs10.org/bjc-r/cur/programming/python/hug_text_processing/python_text_processing_intro.html?topic=berkeley_bjc%2Fpython%2Fbesides-blocks-text-processing.topic&course&novideo&noreading&noassignment) to complete this part of the lab.

## Important Topics (Workbook)

For better understanding of Part 2 we highly recommend going through all of the workbook pages for this part. Topics are best reviewed in order and as you complete the lab.

- [Introduction to Text Processing](https://cs10.org/bjc-r/cur/programming/python/hug_text_processing/python_text_processing_intro.html?topic=berkeley_bjc%2Fpython%2Fbesides-blocks-text-processing.topic&course&novideo&noreading&noassignment)
- [Basic File Input in Python](https://cs10.org/bjc-r/cur/programming/python/hug_text_processing/python_basic_files.html?topic=berkeley_bjc%2Fpython%2Fbesides-blocks-text-processing.topic&course&novideo&noreading&noassignment)
- [Language Games](https://cs10.org/bjc-r/cur/programming/python/hug_text_processing/python_language_games.html?topic=berkeley_bjc%2Fpython%2Fbesides-blocks-text-processing.topic&course&novideo&noreading&noassignment)
- [Counting Words](https://cs10.org/bjc-r/cur/programming/python/hug_text_processing/python_counting_words.html?topic=berkeley_bjc%2Fpython%2Fbesides-blocks-text-processing.topic&course&novideo&noreading&noassignment)
- [Top Words](https://cs10.org/bjc-r/cur/programming/python/hug_text_processing/python_top_words.html?topic=berkeley_bjc%2Fpython%2Fbesides-blocks-text-processing.topic&course&novideo&noreading&noassignment)
- [Word Length](https://cs10.org/bjc-r/cur/programming/python/hug_text_processing/python_word_length.html?topic=berkeley_bjc%2Fpython%2Fbesides-blocks-text-processing.topic&course&novideo&noreading&noassignment)

---

## Setup: read_file(filename)

The code for `read_file` is given in the [Basic File Input in Python](https://cs10.org/bjc-r/cur/programming/python/hug_text_processing/python_basic_files.html?topic=berkeley_bjc%2Fpython%2Fbesides-blocks-text-processing.topic&course&novideo&noreading&noassignment) workbook page. Copy it into `read_file` in the starter file before starting Exercise 8, since later doctests (such as Exercise 10) depend on it.

---

## Exercise 8: pig_latin(word)

**Objective**  
Create a function that takes in a word and returns the pig latin version of that word

**Notes**
- *If the word has vowels, find the FIRST vowel and move ALL the consonants before the vowel to the end of the word and add "ay" to the end. If no vowels OR word starts with a vowel, just add "ay" to the end*

**Inputs**
- str

**Output**
- str

**Examples**
- `>>> x = pig_latin("hello")`  
  `>>> x`  
  `'ellohay'`
- `>>> pig_latin("it")`  
  `'itay'`
- `python3 -m doctest <labfilename>.py` to run autograder
  - Must be in correct parent file

---

## Exercise 9: izzle(word)

**Objective**  
Create a function that takes in a word and outputs the 'izzle' version of that word

**Notes**
- If the word has no vowels, there are two options: append 'izzle' or replace the whole string with 'izzle'. If the word has vowels, replace the string with 'izzle' starting at the LAST vowel.

**Inputs**
- str

**Output**
- str

**Examples**
- `>>> izzle("Merry")`  
  `'Mizzle'`
- `>>> izzle("dentist")`  
  `'dentizzle'`
- Doctests available
  - `python3 -m doctest <labfilename>.py` to run autograder
  - Must be in correct parent file

---

## Exercise 10: apply_language_game(text, language_game)

**Objective**  
Create a function that applies the language game function to each word in the text.

**Inputs**
- text: str
- language_game: function

**Output**
- str

**Examples**
- `>>> text = "the cat is grumpy"`
- `>>> apply_language_game(text, pig_latin)`  
  `'ethay atcay isay umpygray'`
- Doctests available
  - `python3 -m doctest <labfilename>.py` to run autograder
  - Must be in correct parent file

---

## Exercise 11: count_words(text)

**Objective**  
Write a function that counts the occurrences of each word and returns a dictionary where the word is the key and the number of occurrences is the value.

**Notes**
- How do you create a dictionary?

**Inputs**
- str

**Output**
- dict

**Examples**
- `>>> count_words("Fruits and Vegetables and Vegetables and Vegetables and Cheese")`  
  `{'Fruits': 1, 'and': 4, 'Vegetables': 3, 'Cheese': 1}`
- Doctests available
  - `python3 -m doctest <labfilename>.py` to run autograder
  - Must be in correct parent file

---

## Exercise 12: top_n_words(counts, n)

**Objective**  
Create a function that returns a list of the top n words (keys) from the dictionary, ordered by their frequency in descending order.

If two words have the same frequency, their order in the output list depends on their original order in the dictionary

**Notes**
- MUST use the "sorted" function.

**Inputs**
- Counts: dict
- N = int

**Output**
- list

**Examples**
- `>>> dict = {'Fruits': 1, 'and': 4, 'Vegetables': 3, 'Cheese': 1}`  
  `>>> top_n_words(dict, 2)`  
  `['and', 'Vegetables']`
- Doctests available
  - `python3 -m doctest <labfilename>.py` to run autograder
  - Must be in correct parent file

---

## Exercise 13: print_top_n_words(counts, n)

**Objective**  
Prints the top n words (key) along with their counts (value)

**Notes**
- Do not return

**Inputs**
- Counts → dict
- N → int

**Output**
- None
- The function should print

**Examples**
- `>>> dict = {'Fruits': 1, 'and': 4, 'Vegetables': 3, 'Cheese': 1}`  
  `>>> print_top_n_words(dict, 2)`  
  `and 4`  
  `Vegetables 3`
- Doctests available
  - `python3 -m doctest <labfilename>.py` to run autograder
  - Must be in correct parent file

---

## Exercise 14: average_word_length(counts)

**Objective**  
Create a function that takes in a dictionary and returns the average length of words in the text.

**Notes**
- The average word length can be found by
  - [ (word-length * occurrences) ] / number of total words

**Inputs**
- dict

**Output**
- float

**Examples**
- `>>> dict = {'Fruits': 1, 'and': 4, 'Vegetables': 3, 'Cheese': 1}`  
  `>>> average_word_length(dict)`  
  `6.0`
- Doctests available
  - `python3 -m doctest <labfilename>.py` to run autograder
  - Must be in correct parent file

---

**You can always check the validity of your solutions by using the local autograder. Remember to submit on Gradescope!**
