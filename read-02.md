# Class Read 02

## In Tests We Trust — TDD with Python
Unit tests are some pieces of code to exercise the input, the output and the behaviour of your code. You can write them anytime you want.

Test Driven Development (TDD) is a programming practice that instructs developers to write new code only if an automated test has failed. [read more](https://www.guru99.com/test-driven-development.html)

Other thing to care about is the structure. A convention widely used is the AAA: Arrange, Act and Assert.

Arrange: you need to organize the data needed to execute that piece of code (input);

Act: here you will execute the code being tested (exercise the behaviour);

Assert: after executing the code, you will check if the result (output) is the same as you were expecting.

### The Cycle
I hope at this time you didn’t give up of this text because this is an example of an important thing about TDD: the cycle.

The cycle is made by three steps:

🆘 Write a unit test and make it fail (it needs to fail because the feature isn’t there, right? If this test passes, call the Ghostbusters, really)
✅ Write the feature and make the test pass! (you can dance after that)
🔵 Refactor the code — the first version doesn’t need to be the beautiful one (don’t be shy)

[read more](https://code.likeagirl.io/in-tests-we-trust-tdd-with-python-af69f47e6932)


## If name equals main

### What does the if __name__ == “__main__”: do?
Before executing code, Python interpreter reads source file and define few special variables/global variables. 

If the python interpreter is running that module (the source file) as the main program, it sets the special __name__ variable to have a value “__main__”. If this file is being imported from another module, __name__ will be set to the module’s name. Module’s name is available as value to __name__ global variable. 

A module is a file containing Python definitions and statements. The file name is the module name with the suffix .py appended. 

Advantages : 

Every Python module has it’s __name__ defined and if this is ‘__main__’, it implies that the module is being run standalone by the user and we can do corresponding appropriate actions.
If you import this script as a module in another script, the __name__ is set to the name of the script/module.
Python files can act as either reusable modules, or as standalone programs.
if __name__ == “main”: is used to execute some code only if the file was run directly, and not imported.

[read more](https://www.geeksforgeeks.org/what-does-the-if-__name__-__main__-do/)

## Recursion

### Introduction to Recursion – Data Structure and Algorithm Tutorials

What is Recursion? 
The process in which a function calls itself directly or indirectly is called recursion and the corresponding function is called a recursive function. Using a recursive algorithm, certain problems can be solved quite easily. 

Need of Recursion

Recursion is an amazing technique with the help of which we can reduce the length of our code and make it easier to read and write. It has certain advantages over the iteration technique which will be discussed later. A task that can be defined with its similar subtask, recursion is one of the best solutions for it. For example; The Factorial of a number.

Properties of Recursion:

Performing the same operations multiple times with different inputs.

In every step, we try smaller inputs to make the problem smaller.

Base condition is needed to stop the recursion otherwise infinite loop will occur.


A Mathematical Interpretation

Let us consider a problem that a programmer has to determine the sum of first n natural numbers, there are several ways of doing that but the simplest approach is simply to add the numbers starting from 1 to n. 

How are recursive functions stored in memory?

Recursion uses more memory, because the recursive function adds to the stack with each recursive call, and keeps the values there until the call is finished.


There are two types of cases in recursion i.e. recursive case and a base case.

The base case is used to terminate the recursive function when the case turns out to be true.

Each recursive call makes a new copy of that method in the stack memory.

Infinite recursion may lead to running out of stack memory.

Examples of Recursive algorithms: Merge Sort, Quick Sort, Tower of Hanoi, Fibonacci Series, Factorial Problem, etc.

[read more](https://www.geeksforgeeks.org/introduction-to-recursion-data-structure-and-algorithm-tutorials/)

## What on Earth is Recursion?

This article is talks about the recusrsion and why we need it ? Recursion is the process of defining a problem (or the solution to a problem) in terms of (a simpler version of) itself. For example, we can define the operation "find your way home" as: If you are at home, stop moving. Take one step toward home.


Recursion means “solving the problem via the solution of the smaller version of the same problem” or “defining a problem in terms of itself”. It is a widely used idea in programming to solve complex problems by breaking them down into simpler ones.


[see more](https://www.youtube.com/watch?v=Mv9NEXX1VHc)


