---
title: "Lab 17"
description: "Text Processing in Python"
due: "Thursday, April 16th, 11:59PM"
gradescope_assignment_id:
submission_files:
---

# Lab 17: Text Processing in Python

## Instructions

*Updated 4.15.23*

This worksheet serves as a guide and set of instructions to complete the lab.

- Please go through [the entire workbook](https://cs10.org/bjc-r/cur/programming/python/hug_text_processing/python_text_processing_intro.html?topic=berkeley_bjc%2Fpython%2Fbesides-blocks-text-processing.topic&course&novideo&noreading&noassignment) to complete today's lab
- All material was sourced from the CS10 version of The Beauty and Joy of Computing course.

One of the most interesting and important things we can do as a programmer is manipulate and analyze real world data. Python is a particularly great language for data processing, because of the very powerful open source data manipulation libraries available online.

Installing such libraries is beyond the scope of this course (see CS61A and/or DATA C8 instead), so we'll be working mostly with libraries that are built into Python. In this lab, we'll work with text data.

## Getting Started

Create a new folder called "datalab" on your computer (the name doesn't actually matter, but these instructions assume that's the name you use).

Download the data and [starter code](https://cs10.org/bjc-r/prog/python/lab14starter.zip) for this lab from this link. DO NOT modify/delete comments found in the starter code. To run the sanity tests on all functions, navigate to the directory that contains your starter code file and type `python3 -m doctest word_analyzer.py` in terminal.

Unzip this file into the datalab folder. You can unzip this file through the command line by using the unzip command. Remember if you're working on a Windows machine use dir instead of ls.

![terminal unzip example]({{ site.baseurl }}/assets/images/lab_images/lab18_1.png)

## Objectives

Text processing involves the analysis and manipulation of textual data, transforming raw text into structured information. By leveraging text processing techniques, we can extract meaning, identify patterns, and prepare data for further analysis or AI applications. In today's lab, you will:

- Explore the fundamentals of text processing to manage and analyze text data effectively
- Learn to read and preprocess text from files using Python
- Get more practice with data structures
- Use text processing techniques to extract insights from text data.

## Required Functions

- read_file(filename) [required but code is [given](https://cs10.org/bjc-r/cur/programming/python/hug_text_processing/python_basic_files.html?topic=berkeley_bjc%2Fpython%2Fbesides-blocks-text-processing.topic&course&novideo&noreading&noassignment)]**
- pig_latin(word)
- izzle(word)
- apply_language_game(text, language_game)
- count_words(text)
- top_n_words(counts, n)
- print_top_n_words(counts, n)
- average_word_length(counts)

---

## Important Topics (Workbook)

For better understanding of the lab we highly recommend going through all of the workbook pages for this lab. Topics are best reviewed in order and as you complete the lab.

- [Introduction to Text Processing](https://cs10.org/bjc-r/cur/programming/python/hug_text_processing/python_text_processing_intro.html?topic=berkeley_bjc%2Fpython%2Fbesides-blocks-text-processing.topic&course&novideo&noreading&noassignment)
- [Basic File Input in Python](https://cs10.org/bjc-r/cur/programming/python/hug_text_processing/python_basic_files.html?topic=berkeley_bjc%2Fpython%2Fbesides-blocks-text-processing.topic&course&novideo&noreading&noassignment)
- [Language Games](https://cs10.org/bjc-r/cur/programming/python/hug_text_processing/python_language_games.html?topic=berkeley_bjc%2Fpython%2Fbesides-blocks-text-processing.topic&course&novideo&noreading&noassignment)
- [Counting Words](https://cs10.org/bjc-r/cur/programming/python/hug_text_processing/python_counting_words.html?topic=berkeley_bjc%2Fpython%2Fbesides-blocks-text-processing.topic&course&novideo&noreading&noassignment)
- [Top Words](https://cs10.org/bjc-r/cur/programming/python/hug_text_processing/python_top_words.html?topic=berkeley_bjc%2Fpython%2Fbesides-blocks-text-processing.topic&course&novideo&noreading&noassignment)
- [Word Length](https://cs10.org/bjc-r/cur/programming/python/hug_text_processing/python_word_length.html?topic=berkeley_bjc%2Fpython%2Fbesides-blocks-text-processing.topic&course&novideo&noreading&noassignment)

---

## Exercise 1: pig_latin(word)

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
  `'ellohay'`
- `>>> pig_latin("it")`  
  `'itay'`
- `python3 -m doctest <labfilename>.py` to run autograder
  - Must be in correct parent file

---

## Exercise 2: izzle(word)

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

## Exercise 3: apply_language_game(text, language_game)

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
  `"ethay atcay isay umptygray"`
- Doctests available
  - `python3 -m doctest <labfilename>.py` to run autograder
  - Must be in correct parent file

---

## Exercise 4: count_words(text)

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
  `{'Fruits': 1, "and": 4, "Vegetables": 3, "Cheese": 1}`
- Doctests available
  - `python3 -m doctest <labfilename>.py` to run autograder
  - Must be in correct parent file

---

## Exercise 5: top_n_words(counts, n)

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
- `>>> dict = {'Fruits': 1, "and": 4, "Vegetables": 3, "Cheese": 1}`  
  `>>> top_n_words(dict, 2)`  
  `["and", "Vegetables"]`
- Doctests available
  - `python3 -m doctest <labfilename>.py` to run autograder
  - Must be in correct parent file

---

## Exercise 6: print_top_n_words(counts, n)

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
- `>>> dict = {'Fruits': 1, "and": 4, "Vegetables": 3, "Cheese": 1}`  
  `>>> print_top_n_words(dict, 2)`  
  `And 4`  
  `Vegetables 3`
- Doctests available
  - `python3 -m doctest <labfilename>.py` to run autograder
  - Must be in correct parent file

---

## Exercise 7: average_word_length(counts)

**Objective**  
Create a function that takes in a dictionary and returns the average length of words in the text.

**Notes**
- The average word length can be found by
  - [ (word-length * occurrences) ] / number of total words

**Inputs**
- dict

**Output**
- int

**Examples**
- `>>> dict = {'Fruits': 1, "and": 4, "Vegetables": 3, "Cheese": 1}`  
  `>>> average_word_length(dict)`  
  `6`
- Doctests available
  - `python3 -m doctest <labfilename>.py` to run autograder
  - Must be in correct parent file

---

**You can always check the validity of your solutions by using the local autograder. Remember to submit on Gradescope!**
