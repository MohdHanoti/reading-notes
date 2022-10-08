# Read class 04

### Read & Write Files in Python

What Is a File?

A file is a contiguous set of bytes used to store data. This data is organized in a specific format and can be anything as simple as a text file or as complicated as a program executable. In the end, these byte files are then translated into binary 1 and 0 for easier processing by the computer.

Files on most modern file systems are composed of three main parts:

Header: metadata about the contents of the file (file name, size, type, and so on)

Data: contents of the file as written by the creator or editor

End of file (EOF): special character that indicates the end of the file

File Paths

When you access a file on an operating system, a file path is required. The file path is a string that represents the location of a file. It’s broken up into three major parts:

Folder Path: the file folder location on the file system where subsequent folders are separated by a forward slash / (Unix) or backslash \ (Windows)

File Name: the actual name of the file

Extension: the end of the file path pre-pended with a period (.) used to indicate the file type

Line Endings

One problem often encountered when working with file data is the representation of a new line or line ending. The line ending has its roots from back in the Morse Code era, when a specific pro-sign was used to communicate the end of a transmission or the end of a line.

Reading and Writing Opened Files

Once you’ve opened up a file, you’ll want to read or write to the file. First off, let’s cover reading a file.

so How do I open a Python file in reading and writing?

Also if you open Python tutorial about reading and writing files you will find that: 'r+' opens the file for both reading and writing. On Windows, 'b' appended to the mode opens the file in binary mode, so there are also modes like 'rb', 'wb', and 'r+b'.

[read more](https://realpython.com/read-write-files-python/)

[watch video](https://realpython.com/courses/reading-and-writing-files-python/)

### Python Exceptions: An Introduction

What is an exception?

An exception is an event, which occurs during the execution of a program that disrupts the normal flow of the program's instructions.


Exceptions versus Syntax Errors

Syntax errors occur when the parser detects an incorrect statement.

Raising an Exception

We can use raise to throw an exception if a condition occurs. The statement can be complemented with a custom exception.

The AssertionError Exception

Instead of waiting for a program to crash midway, you can also start by making an assertion in Python. We assert that a certain condition is met. If this condition turns out to be True, then that is excellent! The program can continue. If the condition turns out to be False, you can have the program throw an AssertionError exception.

The try and except Block: Handling Exceptions

The try and except block in Python is used to catch and handle exceptions. Python executes code following the try statement as a “normal” part of the program. The code that follows the except statement is the program’s response to any exceptions in the preceding try clause.

raise allows you to throw an exception at any time.

assert enables you to verify if a certain condition is met and throw an exception if it isn’t.

In the try clause, all statements are executed until an exception is encountered.

except is used to catch and handle the exception(s) that are encountered in the try clause.

else lets you code sections that should run only when no exceptions are encountered in the try clause.

finally enables you to execute sections of code that should always run, with or without any previously encountered exceptions.

[read more](https://realpython.com/python-exceptions/)

