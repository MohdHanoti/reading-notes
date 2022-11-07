# Class read 17

## Python Regular Expressions Tutorial

Regular Expressions, often shortened as regex, are a sequence of characters used to check whether a pattern exists in a given text (string) or not. If you've ever used search engines, search and replace tools of word processors and text editors - you've already seen regular expressions in use. They are used at the server side to validate the format of email addresses or passwords during registration, used for parsing text data files to find, replace, or delete certain string, etc. They help in manipulating textual data, which is often a prerequisite for data science projects involving text mining.

In Python, regular expressions are supported by the re module. That means that if you want to start using them in your Python scripts, you have to import this module with the help of import:

import re

The re library in Python provides several functions that make it a skill worth mastering. You will see some of them closely in this tutorial.

### Basic Patterns: Ordinary Characters

You can easily tackle many basic patterns in Python using ordinary characters. Ordinary characters are the simplest regular expressions. They match themselves exactly and do not have a special meaning in their regular expression syntax.

Examples are 'A', 'a', 'X', '5'.

### Wild Card Characters: Special Characters

Special characters are characters that do not match themselves as seen but have a special meaning when used in a regular expression. For simple understanding, they can be thought of as reserved metacharacters that denote something else and not what they look like.

Back to the special characters now.

. - A period. Matches any single character except the newline character.

^ - A caret. Matches the start of the string.

$ - Matches the end of string.

[abc] - Matches a or b or c.
[a-zA-Z0-9] - Matches any letter from (a to z) or (A to Z) or (0 to 9).

\ - Backslash.

### Repetitions
It becomes quite tedious if you are looking to find long patterns in a sequence. Fortunately, the re module handles repetitions using the following special characters:

+ - Checks if the preceding character appears one or more times starting from that position.

* - Checks if the preceding character appears zero or more times starting from that position.

? - Checks if the preceding character appears exactly zero or one time starting from that position.

[read more](https://www.datacamp.com/tutorial/python-regular-expression-tutorial)

## shutil — High-level File Operations

The shutil module includes high-level file operations such as copying and archiving.

### Copying Files

copyfile() copies the contents of the source to the destination and raises IOError if it does not have permission to write to the destination file.

### Copying File Metadata

By default when a new file is created under Unix, it receives permissions based on the umask of the current user. To copy the permissions from one file to another, use copymode().

### Working With Directory Trees

shutil includes three functions for working with directory trees. To copy a directory from one place to another, use copytree(). It recurses through the source directory tree, copying files to the destination. The destination directory must not exist in advance.

### Finding Files

The which() function scans a search path looking for a named file. The typical use case is to find an executable program on the shell’s search path defined in the environment variable PATH.

### Archives

Python’s standard library includes many modules for managing archive files such as tarfile and zipfile. There are also several higher-level functions for creating and extracting archives in shutil. get_archive_formats() returns a sequence of names and descriptions for formats supported on the current system.

### File System Space

It can be useful to examine the local file system to see how much space is available before performing a long running operation that may exhaust that space. disk_usage() returns a tuple with the total space, the amount currently being used, and the amount remaining free.

[read more](https://pymotw.com/3/shutil/)
