---
toc: true
layout: post
author: Kaiden Do
categories: [markdown, week14]
title: Unit 3 Notes
---
# Extra Vocab
## Unit 2… Binary/Data Terms
- Bits, Bytes, Hexadecimal / Nibbles: pieces of information used in computers and devices
- Binary Numbers: Unsigned Integer, Signed Integer, Floating Point: binary numbers are 1 and 0, used in computers are true and false
- Binary Data Abstractions: Boolean, ASCII, Unicode, RGB: 1 and 0 are true in false in the boolean. ASCII are characters used in code, RGB are a range of colors that can be set with binary
- Data Compression: Lossy, Lossless (note discussed yet): unknown
## Unit 3… Algorithm/Programming Terms
- Variables, Data Types, Assignment Operators: variables hold different data types like string, integer and array
```python
score = 90
name = "Bob"
array = ["Hi", 6, 95]
```
- Managing Complexity with Variables:  Lists, 2D Lists, Dictionaries, Class: Lists, classes and dictionaries decrease redundancy in code and make it easier to view
```python
list = ["apple","oranges","mangos"]
```
- Algorithms, Sequence, Selection, Iteration: a procedure helps reduce the redundancy in the code and helps loops or executes lines of code with certain parameters. They contain all three with sequencing through the code, selection of specific code executing, and iteration with looping until a specific requirement is met
```python
def function(x,y):
  while x > 0:
    print(y+x)
    x+=1
  multiply = x*y
  return multiply
```
- Expressions, Comparison Operators, Booleans Expressions and Selection, Booleans Expressions and Iteration, Truth Tables: +, -, *, /, %. The boolean expressions see if the conditions are true or false. Truth Tables are AND, OR, XOR, NOT
```python
x+y
x-y
x*y
x/y
x%y
x and y
x or y
x ^ y
x not
```
- Characters, Strings, Length, Concatenation, Upper, Lower, Traversing Strings: going through the list and assessing each one
``python
index[x]
sort()
pop()
```
- Python If, Elif, Else conditionals; Nested Selection Statements: Is selection, does code if a requirement or condition is met
```python
if (x==1):
  print(x)
```
- Python For, While loops with Range, with List: while loops loops until a condition is met. For loop does something a number of times
```python
for x in range(5):
  print(x)
while x>0:
  print(x)
```
- Combining loops with conditionals to Break, Continue: loops are combined with  conditionals to reduce code repetition and it only works if the condition is met
- Procedural Abstraction, Python Def procedures, Parameters, Return Values: procedural abstraction is the making of functions to decrease code repetition, parameters are used in functions to have specific values in a procedure to execute, return values is the value returned by the function
```python
def multiply(x,y):
  product = x*y
  return product
products = multiply(5,6)
```
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

# Unit 3 Section 8 & 10
## Lesson 3.8 Iteration
- Iteration: repeating part of an algorithm until a condition is met
- Iteration Statements: changes the flow of the code by repeating statements a number of times and it stops repeating once a condition is met
- Repeat Until: the loop of code loops if the condition is not true
### Section 3.8.1
- Stopping condition is used to stop the iteration when the requirement is already met
### Section 3.8.2
- Iteration Statement: causes statement to be executed 0 or more times, depending on the loop-termination condition
- Starting Value: where the variable starts
- Ending Value: where the variable stops
- Incrementing Value: how the variable increases
### Section 3.8.3
- break would stop the loop
## Section 3.10 Lists
- Traversing Lists: all elements in the list are accessed, for partial traversal, only portion of elements are accessed
### Section 3.10.1
- pop() --> takes element off the list and returns it
- sort() --> permanently changes the order of the list
- sorted() --> temporarily changes the order
- min() --> returns the minimum value of the list
- max() --> returns the maximum value of the list
- sum() --> returns the sum of the values in the list
```python
list.pop()
list.sort()
sorted(list)
min(list)
max(list)
sum(list)
```
### Section 3.10.2
- Traversing a list is process of visiting each element in a list in sequential order; used to access, search for, and modify elements in a list
1. Complete Traversal: all elements are accessed
2. Partial Traversal: only a portion are accessed
3. Iterative Traversal: loops used to iterate through list to access each single element at a time
- insert() --> allows value to be inserted at index i
- append() --> allows value to be added at end of list
- remove() --> allows an element at index i to be removed
- length() --> returns number of elements in the list
```python
list.insert()
list.append()
list.remove()
list.length()
```
## Lesson 3.9
### 3.9.1 Algorithms
- Review: components of an algorithm are selection, sequencing, and iteration
- Algorithms don't always do the same thing because of a small equals sign
```python
70 <= grade
70 < grade
```
These are not the same.
- But there are multiple ways to make an algorithm, so they don't need to be identical to work.
- Can use nested conditionals with booleans while making algorithms
### 3.9.2 Developing Algorithms
- should outline or brainstorm before coding an algorithm to make sure it is sequenced correctly
```python
def multiply(x,y):
    product = x*y
    return product
products = multiply(5,6)
def function(x,y):
    while x > 0:
        print(y+x)
        x+=1
    multiply = x*y
    return multiply
```
  - Use a flowchart or pseudo-code and write it out
  - Helps visualize the algorithm and makes it easier to code it after
- Iteration and selection are used within algorithms
### 3.9.3 Using Pre-existing Algorithms
- You can make new algorithms by branching off old ones
- Collatz Conjecture: can repeating two arithmetic operations make all integer become 1?
## Lesson 3.11 Binary Search
- Binary Search: repeatedly diving search interval in half
  - first put numbers in order from small to big
![](https://cdn.discordapp.com/attachments/806618712056528906/1049218338116620339/IMG_8574.jpg)
  - get middle number, then finds if the number is bigger or small than the middle number
  - then moves to the respective side and repeats past step until finds the desired result
![](https://cdn.discordapp.com/attachments/806618712056528906/1049218809539592212/IMG_1541.jpg)
- Practice:
1. 19
2. 22
# Lesson 3.14-15
## Section 3.14.1 Libraries
- Library contains procedures that can be used in new programs
- Code segments can come from internal or external sources
- Libraries can simplify complex programs
- libraries are included with a "."
```python
import math
math.sqrt(64)
```
## Section 3.15.1
- Randomization generates a random value between two numbers
- Need to do import random at the beginning to use random
```python
import random
answer1 = random.randint(0,3)
answer2 = random.randint(1,8)
answer3 = answer1 + answer2
print(answer3)
```
- The range includes the numbers in the range
- Many methods for random
  - seed()
  - getstate()
  - setstate()
  - getrandbits()
  - randrange()
  - randint()
  - choice()
  - choices()
  - shuffle()
  - sample()
  - random()
  - uniform()
  - betavariate()
  - expovariate()
  - gammavariate()
  - gauss()
  - lognormvariate()
  - normalvariate()
  - vonmisesvariate()
  - paretovariate()
  - weibullvariate()
## 3.15.2 Lesson
- RANDOM (a,b) will provide you with a random integer between the numbers a-b
- Ex. RANDOM (7,18) can provide you with the number 13.
- Using a random generator means each result can come out as different. 
```python
import random
flip = random.randint(1,2)
 
if flip == 1:
    print("Heads")
else:
    print("Tails")
```