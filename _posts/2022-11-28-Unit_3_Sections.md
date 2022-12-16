---
toc: true
layout: post
author: Kaiden Do
categories: [markdown, week14]
title: Unit 3 Notes
---
# [Vocab Link]()

# Unit 3 Section 1-2: [Hacks](https://kaiden-dough.github.io/fastpages/jupyter/week14/2022/11/28/Unit_3.1_3.2_HACKS.html)
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

# Unit 3 Section 3-4: [Hacks](https://kaiden-dough.github.io/fastpages/markdown/week14/2022/11/29/Unit_3.3_3.4_HACKS.html)
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

# Unit 3 Section 5-7: [Hacks](https://kaiden-dough.github.io/fastpages/jupyter/week14/2022/12/01/Unit_3.5_3.7_HACKS.html)
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

# Unit 3 Section 8 & 10: [Hacks](https://kaiden-dough.github.io/fastpages/jupyter/week15/2022/12/05/Unit_3.8_3.10_HACKS.html)
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
# Lesson 3.9 & 3.11: [Hacks](https://kaiden-dough.github.io/fastpages/jupyter/week15/2022/12/06/Unit_3.9_3.11_HACKS.html)
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
# Lesson 3.14-15: [Hacks](https://kaiden-dough.github.io/fastpages/jupyter/week16/2022/12/12/Unit_3.14_3.15_HACKS.html)
## Section 3.14.1 Libraries
- Documentation: Text that explains the what, how, or why of your code
```python
def gradeAverage(num):
    sumNums = 0
    for t in num:
        sumNums = sumNums + t

    average = sumNums / len(num)
    return average
print("The average grade is", gradeAverage([65, 70, 72, 75, 80, 73, 61, 84, 81, 83]))
```
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
```python
import random
answer1 = random.randint(0,3)
print(answer1)
```
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
# Lesson 3.16: [Hacks](https://kaiden-dough.github.io/fastpages/jupyter/week16/2022/12/13/Unit_3.16_HACKS.html)
## 3.16 Intro to Simulations
- Simulation: an imitation of situation or process also called a virtual experiment
  - Examples: testing safety of cars, games, testing things
```python
import random
status = "in"
while status != "out":
    chooseCorner = input("What corner do you choose?")
    corner = random.randint(1,4)
    if int(chooseCorner) == corner:
        status = "out"
        print("You chose corner number " + chooseCorner + " and you're OUT")
    else:
        print("You chose corner number " + chooseCorner + " and are still in!")
```
- Experiment: procedure undertaken to make a discovery, test a hypothesis, or to demonstrate a fact
- Simulation Pros and Cons
  - Pros: safer, cheaper, efficient
  - Cons: not as accurate, no outside factors
  - Don't simulate a situation with set results
- Four Corners Example Simulation
```python
import random

status = "in"
while status != "out":
    chooseCorner = input("What corner do you choose?")

    corner = random.randint(1,4)

    if int(chooseCorner) == corner:
        status = "out"
        print("You chose corner number " + chooseCorner + " and you're OUT")
    else:
        print("You chose corner number " + chooseCorner + " and are still in!")
```
- Rolling Dice Simulation
```python
def parse_input(input_string):
    if input_string.strip() in {"1", "2", "3","4", "5", "6"}:
        return int(input_string)
    else:
        print("Please enter a number from 1 to 6.")
        raise SystemExit(1)

import random

def roll_dice(num_dice):
    roll_results = []
    for _ in range(num_dice):
        roll = random.randint(1, 6)
        roll_results.append(roll)
    return roll_results


num_dice_input = input("How many dice do you want to roll? [1-6] ")
num_dice = parse_input(num_dice_input)
roll_results = roll_dice(num_dice)

print("you rolled:", roll_results) 
```
# Lesson 3.17 & 3.18: [Hacks](https://kaiden-dough.github.io/fastpages/jupyter/week16/2022/12/14/Unit_3.17_3.18_HACKS.html)
## Section 3.17
- Sometimes when a problem has too many possibilities, a heuristic approach would be taken
- Algorithmic efficiency: aspect of algorithmic programming that measures the number of steps needed to solve a problem, need code that is more efficient to speed up the code processing.
    - Inefficient:

    ```python
    def inefficientWay(numbers):
        for i in range(len(numbers)):
        min_index = i
        for j in range(i+1, len(numbers)):
            if numbers[j] < numbers[min_index]:
            min_index = j
        numbers[i], numbers[min_index] = numbers[min_index], numbers[i]
        return numbers
    print(inefficientWay([2, 4, 5, 1, 3]))
    ```

    - Efficient:

    ```python
    def efficient_sort(numbers):
        for i in range(len(numbers)):
        min_index = i
        for j in range(i+1, len(numbers)):
            if numbers[j] < numbers[min_index]:
            min_index = j
        numbers[i], numbers[min_index] = numbers[min_index], numbers[i]
        return numbers
    print(efficient_sort([2, 4, 5, 1, 3]))
    ```
## Section 3.18
- Undecidability: you don't know if the problem can be solved or if every number works in the code
  - An undecidable problem is one that should give a "yes" or "no" answer, but yet no algorithm exists that can answer correctly on all inputs.
- Unsolvable: An unsolvable problem is one for which no algorithm can ever be written to find the solution.
- Collatz: The conjecture asks whether repeating two simple arithmetic operations will eventually transform every positive integer into 1
```python
def collatz(i):
    while i != 1:
        if i % 2 > 0:
             i =((3 * i) + 1)
             list_.append(i)
        else:
            i = (i / 2)
            list_.append(i)
    return list_
```
- Hailstone Numbers: The sequence of integers generated by Collatz conjecture are called Hailstone Numbers.