

# Unit 1: Getting Started

In this unit, you will become familiar with the Python in console, Jupyter Notebook, and basic actions and operations in Python.

Follow the links to each lecture, lab, and reading.

Scroll down to download the lessons.


## Lesson 1. What is Python?

Lecture: [Overview of Python](./r-overview.html), demonstration of Python.

Learning Goals:
 - Understand what Python can and cannot do,
 - Install Python and Jupyter Notebook,
 - Know how to navigate within Jupyter Notebook.

Lab: [Unit 1: Lab 1](../unit1/labs.html)

Reading: [NYT article, 2009](http://www.nytimes.com/2009/01/07/technology/business-computing/07program.html?_r=1&pagewanted=all)  | [Quartz article, 2019](https://qz.com/1661487/hadley-wickham-on-the-future-of-r-python-and-the-tidyverse/)

Functions: None.


## Lesson 2. How to use Python as a calculator

Lectures: 

 - [Working with Python and Jupyter Notebooks](./first-look.html)
 
 - [How to use google, stackoverflow, reddit, medium](../swirl.html)

Learning Goals:
 - Perform operations on numbers and integers,
 - Assign numeric and character data to variables,
 - Manipulate variables with operators,
 - Understand and use paths and working directories.

SWIRL: [Basic building blocks](./swirl/basic_building_blocks.html)

Lab: [Unit 1: Lab 2](../unit1/labs.html#lab-2)

Reading: 

 - [How a computer works](./how-computers-work.md)

 - [Working directories](https://support.rstudio.com/hc/en-us/articles/200711843-Working-Directories-and-Workspaces)

Functions: `<-`, `getwd()`, `setwd()`.


## Lesson 3. How to work with vectors

Lecture: [Types of data and data structures](./data-types.html)

Learning Goals:

 - Generate vectors using `c()`, `:`, `seq()`, `rep()`,
 - Assign these vectors to variables and manipulate them,
 - Identify types of vectors (numeric, integer, factor, character, ...)
 - Plot individual vectors with `plot()`.

SWIRL: 

 - [Vectors and Sequences](./swirl/vectors_and_sequences.html)

 - [Subsetting Vectors](./swirl/subsetting_vectors.html)
 
 
Best Practice: [Code style guide](../best/code-style.html)

Labs: 

 - [Unit 1: Lab 3](../unit1/labs.html#lab-3)

 - [Code style lab](../unit1/labs.html#best-practice-lab)

Functions: `c()`, `:`, `seq()`, `rep()`, `plot()`, `is.vector()`, etc


## Lesson 4. How to summarise vectors

Lecture: [Using functions](../unit1/using-functions.html)

Learning Goals:

 - Navigate to and from working directory with `getwd()` and `setwd()`,
 - Subset vectors with logical statements (`>`, `<`, `!=`, `==`),
 - Use functions to perform calculations, with `sum()`, `mean()`, `sd()`, etc.
 - Summarise the distribution of a vector with `boxplot()` and `hist()`.

SWIRL: 

 - [Summarizing Data](./swirl/summarizing_data.html)

 - [Understanding Factors](./swirl/understanding_factors.html)

Lab: [Unit 1: Recap](../unit1/labs.html#unit-1-recap)     

Functions: `getwd()`, `setwd()`, `sum()`, `mean()`, `sd()`, `summary()`, `length()`, `boxplot()`, `hist()`

 - - -
 
# SWIRL

The lessons we will use are available online and you need to download them to your laptop.

1. Open RStudio

2. In the console panel, next to the arrow (>), copy and paste the following: 

```
library(swirl)
install_course_github("intro2r", "swirl_courses", multi = TRUE)
```

This will download the most up-to-date lessons.

To start the lesson, type

```
swirl()
```



- - -

Updated 2018-08-29

