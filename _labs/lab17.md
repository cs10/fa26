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
This worksheet serves as a guide and set of instructions to complete the lab. This lab has two parts: **Part 1** covers dictionaries (building on the lists you practiced in Lab 16) and **Part 2** covers text processing. Both parts live in the same starter file and are submitted together.

- You must use the [starter file, found here](https://cs10.org/bjc-r/prog/python/cs10-fa26-lab17-starter.py), to get credit for the lab. The starter file, `cs10-fa26-lab17-starter.py`, contains the functions for both parts.
- Additionally, here are the workbooks that you can read through for further context and additional (non-required) material:
  - [Data Structures workbook: Dictionaries](https://cs10.org/bjc-r/cur/programming/python/comparing_dicts_lists.html?topic=berkeley_bjc%2Fpython%2Fbesides-blocks-data-struct.topic&course&novideo&noreading&noassignment) (Part 1)
  - [Text Processing workbook](https://cs10.org/bjc-r/cur/programming/python/hug_text_processing/python_text_processing_intro.html?topic=berkeley_bjc%2Fpython%2Fbesides-blocks-text-processing.topic&course&novideo&noreading&noassignment) (Part 2)
- All material was sourced from the CS10 version of The Beauty and Joy of Computing course.

## Submitting
You will need to complete **Exercises 1-9** plus the `read_file` setup function (listed below) and submit `cs10-fa26-lab17-starter.py` to Gradescope.

- To receive full credit, you will need to complete the required functions, and the required functions must pass all tests from the autograder in Gradescope.

Please note, you must use the [starter file](https://cs10.org/bjc-r/prog/python/cs10-fa26-lab17-starter.py), and you must NOT edit the name of any of the required functions. Failing to do either for these will result in the autograder failing.

## Running Doctests
To run doctests embedded within the docstring of a function, you can use the command:

```
python3 -m doctest -v <filename>.py
```

To run all doctests you can run:

```
python3 -m doctest <filename>.py
```

To run the sanity tests on all functions in this lab, navigate to the directory that contains your starter code file and type `python3 -m doctest cs10-fa26-lab17-starter.py` in terminal. (Functions you haven't written yet will fail their tests until you complete them, and the optional functions in the starter file are not required.)

## Objectives
In this lab, we'll explore data structures in Python and then use them to process real-world text. While Snap! mainly uses lists as its only data structure, Python offers more options. You practiced Python lists in Lab 16; in this lab you'll learn dictionaries, which you can think of as more powerful lists.

One of the most interesting and important things we can do as a programmer is manipulate and analyze real world data. Python is a particularly great language for data processing, because of the very powerful open source data manipulation libraries available online. Installing such libraries is beyond the scope of this course (see CS61A and/or DATA C8 instead), so we'll be working mostly with libraries that are built into Python.

Text processing involves the analysis and manipulation of textual data, transforming raw text into structured information. By leveraging text processing techniques, we can extract meaning, identify patterns, and prepare data for further analysis or AI applications. 

In today's lab you will:

- Practice writing functions in Python.
- Manipulate simple data structures and their data.
- Learn how to use key-value pairs and determine why they are useful.
- Solve problems with Python dictionaries
- Explore the fundamentals of text processing to manage and analyze text data effectively
- Learn to read and preprocess text from files using Python
- Use text processing techniques to extract insights from text data.

## Required Functions

Functions marked **(OPTIONAL)** are included in the starter file for extra practice but are **not required** and do not count toward credit.

**Part 1: Data Structures**
- Function 1: base_freq(sequence)
- Function 2.1: substitute_chars(string, replacements)
- Function 2.2: invert_dict(original)

**Part 2: Text Processing**
- read_file(filename) [required but code is [given](https://cs10.org/bjc-r/cur/programming/python/hug_text_processing/python_basic_files.html?topic=berkeley_bjc%2Fpython%2Fbesides-blocks-text-processing.topic&course&novideo&noreading&noassignment)]
- Function 3: pig_latin(word)
- Function 4: izzle(word)
- Function 5: apply_language_game(text, language_game)
- Function 6: count_words(text)
- Function 7: top_n_words(counts, n)
- Function 8: print_top_n_words(counts, n)
- (OPTIONAL) Function: top_n_words_except(counts, n, boring)
- Function 9: average_word_length(counts)
- (OPTIONAL) Function: word_diversity(counts)
- (OPTIONAL) Function: get_kgram(text, ptr, k)
- (OPTIONAL) Function: process_character(m, text, ptr, k)
- (OPTIONAL) Function: build_markov_model(text, k)

---

# Part 1: Data Structures

## Important Topics (Workbook)
For better understanding of Part 1 we highly recommend going through these workbook pages! These topics are best reviewed in order and as you complete the lab.

- [Lists vs Dictionaries](https://cs10.org/bjc-r/cur/programming/python/comparing_dicts_lists.html?topic=berkeley_bjc%2Fpython%2Fbesides-blocks-data-struct.topic&course&novideo&noreading&noassignment)
- [How To Use Dictionaries](https://cs10.org/bjc-r/cur/programming/python/using_dictionaries.html?topic=berkeley_bjc%2Fpython%2Fbesides-blocks-data-struct.topic&course&novideo&noreading&noassignment)

---

## Exercise 1: base_freq(sequence)

**Objective**  
Create a function that counts how many times each item (each character of a string, or each element of a list) appears in the sequence

**Notes**
- Dictionary keys are unique, so each item should only have 1 counter
- Add to the value stored in a dictionary by using:
  - `dictionary_name[key] += x`

**Inputs**
- sequence = string or list

**Output**
- Reports: Dictionary
- Your output should report a dictionary where the key is a unique item and the value is how many times that item appears in the sequence

**Examples**
- Doctests available
  - `python3 -m doctest <labfilename>.py` to run autograder
  - Must be in correct parent file

---

## Exercise 2.1: substitute_chars(string, replacements)

**Objective**  
Create a function that takes as input a string and a dictionary. The dictionary's keys are single characters and its values are the strings to replace those characters with (a value can be one character or several). This function should return a string with each character substituted with that character's value from the dictionary. If a character doesn't exist as a key in the dictionary, it should be left alone.

**Inputs**
- string = some String
- replacements = a Dictionary with single characters as keys and strings as values

**Output**
- Reports: String
- Your output should be a string with all appropriate characters replaced

**Examples**
- Doctests available
  - `python3 -m doctest <labfilename>.py` to run autograder
  - Must be in correct parent file

---

## Exercise 2.2: invert_dict(original)

**Objective**  
Create a function that takes in a dictionary, and reverses all key value pairs

**Notes**
- Dictionary comprehension is very similar to list comprehension!
- What happens when multiple values across the dictionary are identical?
  - Remember that keys in dictionaries are unique

**Inputs**
- original = some dictionary

**Output**
- Reports: Dictionary
- Your output should report a dictionary where the keys and values are inverted

**Examples**
- Doctests available
  - `python3 -m doctest <labfilename>.py` to run autograder
  - Must be in correct parent file
- **Requires substitute_chars to pass local doctests!**

---

# Part 2: Text Processing

Now that you're comfortable with dictionaries, let's put them to work on real text data! Please go through [the entire text processing workbook](https://cs10.org/bjc-r/cur/programming/python/hug_text_processing/python_text_processing_intro.html?topic=berkeley_bjc%2Fpython%2Fbesides-blocks-text-processing.topic&course&novideo&noreading&noassignment) to complete this part of the lab.

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

The code for `read_file` is given in the [Basic File Input in Python](https://cs10.org/bjc-r/cur/programming/python/hug_text_processing/python_basic_files.html?topic=berkeley_bjc%2Fpython%2Fbesides-blocks-text-processing.topic&course&novideo&noreading&noassignment) workbook page. Copy it into `read_file` in the starter file. The Gradescope autograder tests `read_file` by reading its own text files, so you don't need to download any text files for this lab.

---

## Exercise 3: pig_latin(word)

**Objective**  
Create a function that takes in a word and returns the pig latin version of that word

**Notes**
- *If the word has vowels, find the FIRST vowel and move ALL the consonants before the vowel to the end of the word and add "ay" to the end. If no vowels OR word starts with a vowel, just add "ay" to the end*

**Inputs**
- word = some string

**Output**
- Reports: string

**Examples**
- `>>> x = pig_latin("hello")`  
  `>>> x`  
  `'ellohay'`
- `>>> pig_latin("it")`  
  `'itay'`
- Doctests available
  - `python3 -m doctest <labfilename>.py` to run autograder
  - Must be in correct parent file

---

## Exercise 4: izzle(word)

**Objective**  
Create a function that takes in a word and outputs the 'izzle' version of that word

**Notes**
- If the word has no vowels, there are two options: append 'izzle' or replace the whole string with 'izzle'. If the word has vowels, replace the string with 'izzle' starting at the LAST vowel.

**Inputs**
- word = some string

**Output**
- Reports: string

**Examples**
- `>>> izzle("Merry")`  
  `'Mizzle'`
- `>>> izzle("dentist")`  
  `'dentizzle'`
- Doctests available
  - `python3 -m doctest <labfilename>.py` to run autograder
  - Must be in correct parent file

---

## Exercise 5: apply_language_game(text, language_game)

**Objective**  
Create a function that applies the language game function to each word in the text.

**Inputs**
- text = some string
- language_game = a function that takes in a word and returns a new word

**Output**
- Reports: string

**Examples**
- `>>> text = "the cat is grumpy"`
- `>>> apply_language_game(text, pig_latin)`  
  `'ethay atcay isay umpygray'`
- Doctests available
  - `python3 -m doctest <labfilename>.py` to run autograder
  - Must be in correct parent file
- **Requires pig_latin to pass local doctests!**

---

## Exercise 6: count_words(text)

**Objective**  
Write a function that counts the occurrences of each word and returns a dictionary where the word is the key and the number of occurrences is the value.

**Notes**
- How do you create a dictionary?
- Split the text on whitespace. Do not remove punctuation or change capitalization: `'all'` and `'all!'` count as different words, and so do `'Gotta'` and `'gotta'`.

**Inputs**
- text = some string

**Output**
- Reports: Dictionary

**Examples**
- `>>> count_words("Fruits and Vegetables and Vegetables and Vegetables and Cheese")`  
  `{'Fruits': 1, 'and': 4, 'Vegetables': 3, 'Cheese': 1}`
- Doctests available
  - `python3 -m doctest <labfilename>.py` to run autograder
  - Must be in correct parent file

---

## Exercise 7: top_n_words(counts, n)

**Objective**  
Create a function that returns a list of the top n words (keys) from the dictionary, ordered by their frequency in descending order.

If two words have the same frequency, their order in the output list depends on their original order in the dictionary

**Notes**
- MUST use the "sorted" function.

**Inputs**
- counts = a Dictionary mapping words to their counts
- n = number of top words to return

**Output**
- Reports: List

**Examples**
- `>>> counts = {'Fruits': 1, 'and': 4, 'Vegetables': 3, 'Cheese': 1}`  
  `>>> top_n_words(counts, 2)`  
  `['and', 'Vegetables']`
- Doctests available
  - `python3 -m doctest <labfilename>.py` to run autograder
  - Must be in correct parent file

---

## Exercise 8: print_top_n_words(counts, n)

**Objective**  
Prints the top n words (key) along with their counts (value)

**Notes**
- Do not return
- Your top_n_words function from Exercise 7 may be useful here

**Inputs**
- counts = a Dictionary mapping words to their counts
- n = number of top words to print

**Output**
- Reports: nothing
- *This function should print, not return*

**Examples**
- `>>> counts = {'Fruits': 1, 'and': 4, 'Vegetables': 3, 'Cheese': 1}`  
  `>>> print_top_n_words(counts, 2)`  
  `and 4`  
  `Vegetables 3`
- Doctests available
  - `python3 -m doctest <labfilename>.py` to run autograder
  - Must be in correct parent file

---

## Exercise 9: average_word_length(counts)

**Objective**  
Create a function that takes in a dictionary and returns the average length of words in the text.

**Notes**
- The average word length can be found by
  - (sum of word length × occurrences for every word) / (total number of words)

**Inputs**
- counts = a Dictionary mapping words to their counts

**Output**
- Reports: float

**Examples**
- `>>> counts = {'Fruits': 1, 'and': 4, 'Vegetables': 3, 'Cheese': 1}`  
  `>>> average_word_length(counts)`  
  `6.0`
- Doctests available
  - `python3 -m doctest <labfilename>.py` to run autograder
  - Must be in correct parent file

---

**You can always check the validity of your solutions by using the local autograder. Remember to submit on [Gradescope](https://www.gradescope.com/courses/{{ site.gradescope_course_id }})!**
