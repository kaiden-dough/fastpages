---
toc: true
layout: post
author: Kaiden Do
categories: [markdown, week14]
title: Unit 3 Notes
---

# Unit 3 Section 1-2
## Unit 3, Section 1.1: Data Types and Variables
 - Variable is an abstraction in a program that holds a value, only one value at a time
 - They have good names to organize code and understand what the variables represent
 - Some variables are booleans, numbers, lists and strings; each are used in different instances
 - Variables are seen as "containers" that have a name and value
 - Naming variables certain names are important to prevent confusion
 - Some variables are used for different things

## Unit 3, Section 1.2: Variables
 - Determine the value of variable as a result of an assignment, use assignment operator
 - In python, they use equal sign to assign a value to the variable
 - Recap: learn what is an assignment operator, how to use it, how to store value inside a variable

 ## Unit 3, Section 2.1 : List and Strings Using Variables
 - Strings are a series of characters, both numbers and letters and characters
 - Lists are sequences of elements with each element is a variable
    - In order
    - Can store different types of variables
    - Can be accessed by index (starts at 0)

## Unit 3, Section 2.2 : Data Abstraction with Lists
 - Lists bundle multiple variables under one name, can have different types of variables
 - User doesn't know how the list stores data so it is data abstraction

## Unit 3, Section 2.3 : Managing Complexity with lists
 - Use lists to manage complexity
 - Simplifies code and makes code faster and easier
    - Code is easier to read
 - Many variables are not needed, don't need to edit/add/remove entire variable to change it

# Unit 3 Section 3-4
## Lesson 3.3
 - An algorithm is a finite set of instructions that completes a task
   - Sequencing: the order the code is completed
   - Selection: lets algorithm make a decision based on if a condition is met
   - Iteration: a loop of something until a condition is met
 - Mathematical Expressions
   - Sequential code statements are used in algorithms to specify how signals are assigned
 - Arithmetic Operators: addition, subtraction, multiplication, division, and modulus
   - +, -, *, /, %
   - MOD returns the remainder
## Lesson 3.4
 - String Concatenation
   - Joins two or more strings together to make a new string
      - strings are sequences of characters
      - substring string in python can be found with the string and which range of characters

# Unit 3 Section 5-7
## Lesson 3.5
Boolean
 - Boolean is a true (1) or false (0) --> (binary)
 - Used to tell if something is true or false
 - Ex 1 & Ex 2:
 ```python
 score = 3
 if score == 3:
    print("Score equals 3")
 ```
Relational Operators
 - Mathematical relationship between two variables
 - Determines output even if statement is not true
 - Ex 1
 ```python
 age = 18
 if age >= 16:
    print("Can Drive")
 ```
 - Ex 2
 ```python
 passengers = 3
 cart = 4
 if cart >= passengers:
    print("Not Full")
 ```

 Logical Operators
 - NOT: opposite of the data, usually true/false
 - AND: evaluate 2 conditions together and if both conditions are met
 - OR: determines if one of the conditions is met

## Lesson 3.6
- Selection: specific block of code that will execute if the condition passed
- Algorithm: finite set of code that completes a task
- Conditional statement: affects the sequence of control by executing statements in different order
  - Affects the sequential flow of the code

## Lesson 3.7
- Nested Conditional Statement: conditional statement with more inside of it
- Nested into each other: else if in else if
- Question 1: x = 5 & y = 4
  - x is smaller than y
- Question 2: height = 60 & age = 17 & photo taken
  - The total bill is $10.