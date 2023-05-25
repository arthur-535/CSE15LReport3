# CSE15L LAB 3 REPORT 

For this lab report, I will be researching the "find" command. It's mainly
used to search for files and directories. It searches through files and directories recursivley.

Side note: The general syntax for "find" is
find [options] [path...] [expression]

**Command (-type)**
-type is used to search a specific type of document within a directory. 

EX 1) 

Command
``` 
find ./government -type d
 ``` 

The "-type d" commands allows the user to find all the directories within a directory. 

Output
![Image](typeDlab3.png)

EX 2) 

Command
``` 
find ./Post_Rate_comm -type f
 ``` 

The "-type f" command allows the user to find all of the files within a directory. 

Output
![Image](typeFlab3.png)

Source
ChatGPT

**Command Option 2 (-empty)**

-empty is used to help the user find empty files/directories

Example 1 

Command
``` 
find . -type d -empty

 ```
 Output
![Image](emptyDLab3.png)
 
The ". -type d - empty" command allows the user to find all the empty directories within the CSE15L directory. 



Example 2


Command
``` 
find . -type f -empty

 ```
 Output
![Image](emptyFLab3.png)

The ". -type F - empty" command allows the user to find all the empty files within the CSE15L directory. 

Source
ChatGPT

**Command (-size)**

-size is used to search for files that match a specific size in bytes.

Example 1 

Command
``` 
find ./government -size -500c'

 ``` 

Output
![Image](size--lab3.png)

The "-size -500c" command allowed the user to find the all files what are smaller than 500 bytes. 

Example 2
Command
``` 
find ./government -size +500c'

 ``` 

Output
![Image](size+lab3.png)

The "-size +500c" command allowed the user to find the all files what are larger than 500 bytes. 

Source
ChatGPT
**Command (-name)**

-name -"string"  allows you to search for files and directories based on their names or patterns. 

Example 1 

Command
``` 
find media/* -name 'Annual_fee.txt'

 ``` 
Output
![Image](specNamelab3.png)

The "-name 'Annual_fee.txt'" allowed the user to find exact file within the directory media.


Example 2

Command
``` 
find Post_Rate_Comm/* -name 'Cohenetal_comparison.txt'

 ``` 
Output
![Image](nameComLab3.png)

The "-name 'Cohenetal_comparison.txt'" allowed the user to find exact file within the directory media.

Source
ChatGPT
