# Class Read 02

## In Tests We Trust — TDD with Python
Unit tests are some pieces of code to exercise the input, the output and the behaviour of your code. You can write them anytime you want.

Test Driven Development (TDD) is a programming practice that instructs developers to write new code only if an automated test has failed. [read more](https://www.guru99.com/test-driven-development.html)

Other thing to care about is the structure. A convention widely used is the AAA: Arrange, Act and Assert.

Arrange: you need to organize the data needed to execute that piece of code (input);

Act: here you will execute the code being tested (exercise the behaviour);

Assert: after executing the code, you will check if the result (output) is the same as you were expecting.

### The Cycle

The cycle is made by three steps:

 Write a unit test and make it fail (it needs to fail because the feature isn’t there, right? If this test passes, call the Ghostbusters, really)
 Write the feature and make the test pass! (you can dance after that)
 Refactor the code — the first version doesn’t need to be the beautiful one (don’t be shy)

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

[see more](https://www.youtube.com/watch?v=Mv9NEXX1VHc)

## Google for Education: Python List

### Python Lists

 List literals are written within square brackets [ ]. Lists work similarly to strings
 
 Assignment with an = 
 
 ### Range 
The range(n) function yields the numbers 0, 1, ... n-1, and range(a, b) returns a, a+1, ... b-1 -- up to but not including the last number.

### While Loop
Python also has the standard while-loop, and the *break* and *continue* statements work as in C++ and Java, altering the course of the innermost loop.

### List Methods
Here are some other common list methods.

list.append(elem) -- adds a single element to the end of the list. Common error: does not return the new list, just modifies the original.

list.insert(index, elem) -- inserts the element at the given index, shifting elements to the right.

list.extend(list2) adds the elements in list2 to the end of the list. Using + or += on a list is similar to using extend().

list.index(elem) -- searches for the given element from the start of the list and returns its index. Throws a ValueError if the element does not appear (use "in" to check without a ValueError).

list.remove(elem) -- searches for the first instance of the given element and removes it (throws ValueError if not present)

list.sort() -- sorts the list in place (does not return it). (The sorted() function shown later is preferred.)

list.reverse() -- reverses the list in place (does not return it)

list.pop(index) -- removes and returns the element at the given index. Returns the rightmost element if index is omitted (roughly the opposite of append()).
 
 ### List Slices
Slices work on lists just as with strings, and can also be used to change sub-parts of the list.

[read more](https://developers.google.com/edu/python/lists)

## Google for Education: Python Strings

### Python Strings

Python has a built-in string class named "str" with many handy features (there is an older module named "string" which you should not use).

String Methods

s.lower(), s.upper() -- returns the lowercase or uppercase version of the string

s.strip() -- returns a string with whitespace removed from the start and end

s.isalpha()/s.isdigit()/s.isspace()... -- tests if all the string chars are in the various character classes

s.startswith('other'), s.endswith('other') -- tests if the string starts or ends with the given other string

s.find('other') -- searches for the given other string (not a regular expression) within s, and returns the first index where it begins or -1 if not found

s.replace('old', 'new') -- returns a string where all occurrences of 'old' have been replaced by 'new'

s.split('delim') -- returns a list of substrings separated by the given delimiter. The delimiter is not a regular expression, it's just text. 'aaa,bbb,ccc'.split(',') -> ['aaa', 'bbb', 'ccc']. As a convenient special case s.split() (with no arguments) splits on all whitespace chars.

s.join(list) -- opposite of split(), joins the elements in the given list together using the string as the delimiter. e.g. '---'.join(['aaa', 'bbb', 'ccc']) -> aaa---bbb---ccc

## Python Modules and Packages

A module is a file containing Python definitions and statements. The file name is the module name with the suffix .py appended. Within a module, the module’s name (as a string) is available as the value of the global variable __name__. 

A module can be written in Python itself.

A module can be written in C and loaded dynamically at run-time, like the re (regular expression) module.

A built-in module is intrinsically contained in the interpreter, like the itertools module.

A python package is a collection of modules. Modules that are related to each other are mainly put in the same package. When a module from an external package is required in a program, that package can be imported and its modules can be put to use.

### Pytest Documentation

The pytest framework makes it easy to write small, readable tests, and can scale to support complex functional testing for applications and libraries.

pytest has never been associated with a security vulnerability, but in any case, to report a security vulnerability please use the Tidelift security contact. Tidelift will coordinate the fix and disclosure.

[read more](https://docs.pytest.org/en/latest/)

## PyTest Tutorial

PyTest is a testing framework that allows users to write test codes using Python programming language. It helps you to write simple and scalable test cases for databases, APIs, or UI. PyTest is mainly used for writing tests for APIs. It helps to write tests from simple unit tests to complex functional tests.

Some of the advantages of pytest are

Very easy to start with because of its simple and easy syntax.

Can run tests in parallel.

Can run a specific test or a subset of tests

Automatically detect tests

Skip tests

Open source

#### How PyTest Identifies the Test Files and Test Methods

Pytest automatically identifies those files as test files

[read more](https://online.ltuc.com/d2l/lms/dropbox/user/folder_submit_files.d2l?db=84771&grpid=0&isprv=False&bp=0&ou=42425)
