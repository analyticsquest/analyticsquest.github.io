Python Style Guide I: Syntax
========================================================


![](http://intro2r.github.io/img/mcqueen.jpg)

*Steve McQueen, your (Python) style guru*


# 1. Why have a code style?

### a. Coding styles help communication

Good coding style is like correct punctuation: 

you can manage without it, 

butitsuremakesthingseasiertoread.


### b. Your code has 1 author; but many readers

you, tomorrow

you, on Friday

you, next week

you, next year

your friend


your friend's friend

your mum

your reviewer

your third reviewer

your revising your manuscript

me

the dog 

...


### c. There are many different styles of writing code

![](http://intro2r.github.io/img/men-style.png)

 - different software or language 
 - different people
 
Try to develop a **consistent** style 


### d. Consistent style is important, because ...

 - **Focus should be what the code does, not how it is written.**
 - Changes in style mid-way through code increases effort and deceases understanding.
 - Especially important when working with others.


### e. Style can be applied to:

1. **Syntax**

2. Files

3. Functions

4. Code documentation



# 2. Syntax Style

## The arrangement of words and phrases

1. Object names.

2. Spacing.

3. Argument names.

4. Indenting.

5. Long lines.

6. Assignment.

7. Semicolons.

8. Quotes.

========

## 1. Object names

Python is case-sensitive ... other software (M$, ...) is not.

### Principles

 - Variable names should be nouns.
 - Function names should be verbs.
 - Concise and meaningful (hard!)
 - Avoid periods (used in indicate classes...more on that later).
 - Avoid writing over common names (e.g., sqrt!)
 
 
 
### Best Practice

 - **Variables:** lowercase, numbers, and underscores.
    ``` 
    x
    my_sqrt
    ```
 - **Functions:** camelCase.
    ``` 
    myNewFunc()
    calcTemp()
    ```
 - All CAPS (constants).
 
 

## 2. Spacing

### Principle

- Ease of reading and understanding code.

 
### Best Practice

Put a space:

 - Before and after all operators (```=, +, -, /, *```, etc...).
    ``` 
    1 + 3
    x / y
    x * y 
    ```
 - Arguments in function calls.
    ```
    seq(from = 1, to = 10)
    ```
 - *Except* around ```:```, ```::```, ```:::```.
    ```
    1:10
    ```
 - Use extra spacing to for readability.
    ```
    new_var = 1:10
    ```
 - No spaces around ```()``` or ```[]```, unless there is a ```,```.
    ```
    seq(1, 10)
    x[1, ]
    ```
 


## 3. Argument names

Two kinds of arguments:

 - Supplies the **data**.
 - **Details** of computation.
 
 
 
### Principle

- Ease of understanding the function.
 
### Best Practice 
 
- Generally omit names of data arguments (they are often the first argument/s).
```
seq(1, 10)
mean(1:10)
```

- If you override the default, use the full argument name.
```
import pandas as pd
data = pd.read_csv("bwq.csv", full argument = XYZ)
data
```


## 4. Indenting

### Principle

- Show hierarchy of code and curly braces or brackets
- Make code easier to read, aligning related lines.



### Best Practice


- Spaces are the preferred indentation method. Tabs should be used solely to remain consistent with code that is already indented with tabs. Python disallows mixing tabs and spaces for indentation.
- Use consistent indenting (2 or 4 spaces, never TABS).
- Always indent after function or loop colon.
```
#an example of a loop (we will do this later in the course)
for i in range(10):
    sum = sum(1+i)
    print sum
```
- Align arguments within a function if line overruns.
```
def demo(name, age):
    # this line is commented out and does not run.
    print(name, age)

demo("Ben", 25)
```

=======

## 5. Long lines

### Principle

- Ease of reading and following code.
- Ease of changing code.

### Best Practice

- Try and limit to 72 characters per line.
- If a function call is too long for one line, use one line each for the function name, each argument, and closing
- Donald Knuth explains the traditional rule in his Computers and Typesetting series: “Although formulas within a paragraph always break after binary operations and relations, displayed formulas always break before binary operations”.
```
# Correct:
# easy to match operators with operands
income = (gross_wages
          + taxable_interest
          + (dividends - qualified_dividends)
          - ira_deduction
          - student_loan_interest)
```


## 6. Assignment

### Principle

- Separation of assignment and arguments.

### Best Practice

- Use ``` = ``` for assignment.

```
#Yes, x assigned value of 10
x = 10

# No, no, no, no, no, nooooooooooo, this is the R language below, not python. 
x <- 1:10
```


## 7. Colons and Semicolons

### Principle

- A colon is required at the beginning of every block of code.
```
if condition:
    code code code
```
- A semicolon in Python is mostly used to separate multiple statements written on a single line.
```
for i in range (4): print ('Hi') ; print('Hello')
output:
  Hi
  Hello
  Hi
  Hello
  Hi
  Hello
  Hi
  Hello
```

## 8. Quotes

### Principle

- Use single-quotes for string literals, e.g. 'my-identifier', but use double-quotes for strings that are likely to contain single-quote characters as part of the string itself (such as error messages, or any strings containing natural language), e.g. "You've got an error!".

### Best Practice

- Double quotes ``` " " ``` and single quotes ``` ' ' ``` are usually **interchangable**.
- Double quotes are **preferred** because of the use of apostrophes in text strings.

```
#single-quotes identifying 'Bob' and assigning to variable called name.
name = 'Bob'
#Double-quotes can be used in Natural language
print("It is easy to get confused with single and double quotes in Python.")
#Double-quotes can be used String interpolation
print(f"{name} said there will be food.")
#Double-quotes can be used to escape a character
print("We're going skiing this winter.")
#Double-quotes can be used for Quotation inside a string
print("My favorite quote from Die Hard is 'Welcome to the party, pal'")
```

[Python Single vs. Double Quotes - Which Should You Use And Why?](https://betterdatascience.com/python-single-vs-double-quotes/)



    
# Links to various Python and Jupyter Notebook style guides

[Guiding Principles - first the style principles](https://explog.in/notes/nbstyle.html) - A good first read for notebook style.

[Jupyter Notebook best practices](https://towardsdatascience.com/jupyter-notebook-best-practices-f430a6ba8c69)

[Coding Standards for your Jupyter Notebooks](https://medium.com/@atma_mani/coding-standards-for-your-jupyter-notebooks-f4e2af7db3a9)

[GCP Jupyter Notebooks Development Manifest](https://cloud.google.com/blog/products/ai-machine-learning/best-practices-that-can-improve-the-life-of-any-developer-using-jupyter-notebooks) Google Cloud Platform Guide

[Clean code in Jupyter Notebooks](https://www.slideshare.net/katenerush/clean-code-in-jupyter-notebooks)

[Style Guide for Python Code](https://peps.python.org/pep-0008/) - A classic.

[Space Telescope Science Institute Jupyter Notebook Style Guide](https://github.com/spacetelescope/style-guides/blob/master/guides/jupyter-notebooks.md)

 
 - - -

Updated: 2022-12-10
