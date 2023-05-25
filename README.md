# CSE15L LAB 3 REPORT 

For this lab report, I will be researching the "find" command. It's mainly
used to search for files and directories. It searches through files and directories recursivley.

Side note: The general syntax for "find" is
find [options] [path...] [expression]

**Command (-empty)**

EX 1) 

Command
``` 
find ./government -type d
 ``` 

The "-type d" option in the "find" command is useful because it allows you to specifically search for directories. 
By using this option, you can filter the search results to only include directories and exclude any other types of files. 
The command above is used to find all diectories in "./technical".

Output
``` 
``` 

Source
ChatGPT

**Command Option 2 (-find)**

The -size option is used to search for files that match a specific size in bytes. This can be useful when you are looking for files of a specific size, such as very large or very small files.

Example 1 

Command
``` 
find ./technical -size -500c

 ``` 
The find command above is uszed to find all files that are less than 500 bytes in "./technical".
Output



Example 2

Command

``` 
find ./technical -size +500c
``` 
The find command above is uszed to find all files that are more than 500 bytes in "./technical".

Output
``` 

``` 
Source
ChatGPT

**Command (-size)**
The "find" command with the "-name" option allows you to search for files and directories based on their names or patterns. 
It is particularly useful when you want to locate files that match a specific name or pattern within a directory hierarchy. 

Example 1 

Command
``` 
find technical/ -name 'preface.txt'

 ``` 

The find command above used to find a file with the specicic name 'preface.txt'.
This command is useful when trying to find a a specific file.
Output
``` 
preface.txt
``` 


Example 2

Command

``` 
find technical/ -name 'chapter-1.txt'

``` 

The find command above used to find a file with the specicic name 'chapter-1.txt'. 
This is usefull when trying to find a specific name in a directory with many files.


Output
``` 
chapter-1.txt
``` 
Source
ChatGPT
**Command (-name)**

The "find . -type  -empty" command is useful for locating empty directories within a directory hierarchy. 
It helps you efficiently manage disk space, maintain an organized file system, automate cleanup tasks, 
and troubleshoot potential issues related to empty directories.

Example 1 

Command
``` 
find . -type d -empty

 ``` 

The find command above used to find an empty directory.
If you are trying to find an empty direcory to use, this command is a good first step.

Output
``` 
./.git/objects/info
./.git/refs/tags
``` 


Example 2

Command

``` 
find . -type f -empty

``` 
The find command above used to find an empty files.
If you are trying to find an empty file to use or delete this find command could be usefull.

Output
``` 
no ouput
``` 
