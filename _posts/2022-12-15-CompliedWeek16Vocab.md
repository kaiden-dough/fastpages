---
toc: true
layout: post
author: Kaiden Do
categories: [markdown, week16]
title: Week 16 Vocab
---
# 3.14
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

- Documentation for the example above: The procedure gradeAverage takes a list of integer values representing the percentages in a certain class, and returns the average of those integers.
- Libraries: A collection of pre-written code or procedures that coders can use to maximize their efficiency

```python
import math
math.sqrt(64)
```

- Application Programming Interface: A type of software through several computers are able to communicate information amongst each other
# 3.15
- Randomization: generates a value between two numbers

```python
import random
answer1 = random.randint(0,3)
print(answer1)
```

# 3.16
- Simulations: an imitation of a situation or process

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

- Experiment: procedure undertaken to make a discovery, test a hypothesis, or demonstrate a known fact
# 3.17
- Algorithm Efficiency: aspect of algorithmic programming that measures the number of steps needed to solve a problem
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

- Heuristic Approach: taking the shortest or easiest possibilities to the result
# 3.18
- Collatz Conjecture: asks whether repeating two simple arithmetic operations will eventually transform every positive integer into 1

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

- Hailstone numbers: sequence of integers generated by Collatz conjecture
- Undecidable problems: should give a "yes" or "no" answer, but yet no algorithm exists that can answer correctly on all inputs
- Unsolvable problems: no algorithm can ever be written to find the solution
