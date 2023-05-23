# Lab Report 3
*** 
## Command: Find.
The command I chose for this lab report was find. All the sources will be references intext throughout the report but the 
links will be at the bottom of the report. 
*** 
1. `find -name`
(Source: adamtheautomator.com)
find -name is used to find any keyword/directory/file within the main directory it is within, which in this case is ./technical.
* Example 1:
This is an example in which I implore the find -name function to find a directory within the directory technical called plos. 
This is useful to check for the existence of specific wanted directories as well as their paths. 
Command Line:
```
>sannidhikrovvidi@Sannidhis-MacBook-Pro technical % find . -name "*plos"   
```
Output:
```
./plos
```
* Example 2:
This is an example where I use the find -name function to find a file within the directory 911report within the technical directory.
This is useful to check for the existence of specific wanted files and their paths.
Command Line:
```
sannidhikrovvidi@Sannidhis-MacBook-Pro technical % find . -name "*chapter-1.txt"
```
Output:
```
./911report/chapter-1.txt
```
***
2. `find "name" type -d/-f`
(Source: adamtheautomator.com)
To specifically find files and directories as well as their paths. 
* Example 1:
Here I used the function to find the all of the directories within technical as well as their paths. This is useful to verify the status and paths of directories. 
directories. 
Command Line:
```
sannidhikrovvidi@Sannidhis-MacBook-Pro technical % find . -type d
```
Output: 
```
.
./government
./government/About_LSC
./government/Env_Prot_Agen
./government/Alcohol_Problems
./government/Gen_Account_Office
./government/Post_Rate_Comm
./government/Media
./plos
./biomed
./911report
```
* Example 2:
Searching for all of the files within technical would produce a very large output so instead I searched for one specific file
while also checking that it was a file and tracing its path. This is useful to verify the status and paths of files.
Command Line: 
```
sannidhikrovvidi@Sannidhis-MacBook-Pro technical % find . -type f -name "*commission_report.txt"
```
Output:
```
./government/About_LSC/commission_report.txt
```
***
3. `find . -name "letter*.filetype"`
(Source: ChatGPT)
This searches for all of the files of a specific filetype such as .txt that start with a given letter.
* Example 1:
Here I am searching for all of the files starting with an a that are .txt files. This is a common starting letter. This is useful to narrow down the search for files of the .txt type starting with an a.
Command Line:
```
sannidhikrovvidi@Sannidhis-MacBook-Pro technical % find . -name "a*.txt"
```
Output:
```
./government/Env_Prot_Agen/atx1-6.txt
./government/Gen_Account_Office/ai00134.txt
./government/Gen_Account_Office/ai9868.txt
./government/Gen_Account_Office/ai2132.txt
./government/Media/agency_expands.txt
./biomed/ar331.txt
./biomed/ar319.txt
./biomed/ar79.txt
./biomed/ar130.txt
./biomed/ar118.txt
./biomed/ar93.txt
./biomed/ar68.txt
./biomed/ar120.txt
./biomed/ar297.txt
./biomed/ar321.txt
./biomed/ar309.txt
./biomed/ar795.txt
./biomed/ar408.txt
./biomed/ar409.txt
./biomed/ar422.txt
./biomed/ar387.txt
./biomed/ar778.txt
./biomed/ar750.txt
./biomed/ar624.txt
./biomed/ar383.txt
./biomed/ar619.txt
./biomed/ar745.txt
./biomed/ar792.txt
./biomed/ar430.txt
./biomed/ar140.txt
./biomed/ar429.txt
./biomed/ar774.txt
./biomed/ar615.txt
./biomed/ar601.txt
./biomed/ar407.txt
./biomed/ar799.txt
./biomed/ar612.txt
./biomed/ar149.txt
./biomed/ar104.txt
./biomed/ar328.txt
```
* Example 2: 
Here I am searching for all of the files starting with an m that are .txt files. This is not as 
common of a starting letter. This is useful to narrow down the search for files of the .txt type starting with an m.
Command Line:
```
sannidhikrovvidi@Sannidhis-MacBook-Pro technical % find . -name "m*.txt"
```
Output:
```
./government/Env_Prot_Agen/multi102902.txt
./government/Media/man_on_national_team.txt
```
***
4. `find . -perm -permissioncode`
(Source: ChatGPT)
This searches for all of the files with the specified permission code (specific permissions).
* Example 1:
Here I explored the outcome of the permission code 600. Many files were found. This is useful to see different specific permissions for different files.
Command Line:
```
sannidhikrovvidi@Sannidhis-MacBook-Pro technical % find . -perm -600
```
Output:
```
...
./biomed/1471-2431-2-12.txt
./biomed/ar328.txt
./biomed/1471-2210-3-1.txt
./biomed/1471-2121-4-5.txt
./biomed/1471-2350-2-8.txt
./biomed/1471-2202-3-17.txt
./biomed/1471-2407-1-13.txt
./biomed/bcr605.txt
./biomed/1476-069X-2-9.txt
./biomed/1478-1336-1-3.txt
./biomed/1471-2164-2-4.txt
./biomed/1471-2210-1-3.txt
./biomed/1476-9433-1-3.txt
./biomed/1471-2334-1-13.txt
./biomed/1471-2407-3-16.txt
./biomed/1471-2164-4-2.txt
./biomed/cvm-2-4-187.txt
./biomed/1471-2105-3-4.txt
./biomed/1471-2121-3-21.txt
./biomed/1471-2202-4-2.txt
./biomed/1471-2172-3-9.txt
./biomed/gb-2001-2-3-research0007.txt
./biomed/1471-2199-2-6.txt
./biomed/bcr567.txt
./biomed/gb-2002-3-10-research0055.txt
./biomed/1471-2121-2-3.txt
./biomed/1471-213X-1-11.txt
./biomed/1472-684X-1-5.txt
./biomed/1476-4598-1-6.txt
./911report
./911report/chapter-13.4.txt
./911report/chapter-13.5.txt
./911report/chapter-13.1.txt
./911report/chapter-13.2.txt
./911report/chapter-13.3.txt
./911report/chapter-3.txt
./911report/chapter-2.txt
./911report/chapter-1.txt
./911report/chapter-5.txt
./911report/chapter-6.txt
./911report/chapter-7.txt
./911report/chapter-9.txt
./911report/chapter-8.txt
./911report/preface.txt
./911report/chapter-12.txt
./911report/chapter-10.txt
./911report/chapter-11.txt ...
```
* Example 2:
Here I explored the outcome of the permission code 700. Many files were found. his is useful to see different specific permissions for different files.
Command Line:
```
sannidhikrovvidi@Sannidhis-MacBook-Pro technical % find . -perm -700
```
Output:
```
...
./biomed/1471-2156-4-9.txt
./biomed/1471-2431-2-12.txt
./biomed/ar328.txt
./biomed/1471-2210-3-1.txt
./biomed/1471-2121-4-5.txt
./biomed/1471-2350-2-8.txt
./biomed/1471-2202-3-17.txt
./biomed/1471-2407-1-13.txt
./biomed/bcr605.txt
./biomed/1476-069X-2-9.txt
./biomed/1478-1336-1-3.txt
./biomed/1471-2164-2-4.txt
./biomed/1471-2210-1-3.txt
./biomed/1476-9433-1-3.txt
./biomed/1471-2334-1-13.txt
./biomed/1471-2407-3-16.txt
./biomed/1471-2164-4-2.txt
./biomed/cvm-2-4-187.txt
./biomed/1471-2105-3-4.txt
./biomed/1471-2121-3-21.txt
./biomed/1471-2202-4-2.txt
./biomed/1471-2172-3-9.txt
./biomed/gb-2001-2-3-research0007.txt
./biomed/1471-2199-2-6.txt
./biomed/bcr567.txt
./biomed/gb-2002-3-10-research0055.txt
./biomed/1471-2121-2-3.txt
./biomed/1471-213X-1-11.txt
./biomed/1472-684X-1-5.txt
./biomed/1476-4598-1-6.txt
./911report
./911report/chapter-13.4.txt
./911report/chapter-13.5.txt
./911report/chapter-13.1.txt
./911report/chapter-13.2.txt
./911report/chapter-13.3.txt
./911report/chapter-3.txt
./911report/chapter-2.txt
./911report/chapter-1.txt
./911report/chapter-5.txt
./911report/chapter-6.txt
./911report/chapter-7.txt
./911report/chapter-9.txt
./911report/chapter-8.txt
./911report/preface.txt
./911report/chapter-12.txt
./911report/chapter-10.txt
./911report/chapter-11.txt ....
```
***
## Sources:
- Website: [Link](https://adamtheautomator.com/bash-find/)
- ChatGPT
    - Questions & Answers:
---

**how to use find -name in a directory.**

---

The find command is a powerful tool for searching for files and directories in a directory hierarchy based on various criteria. The -name option is used to search for files or directories that match a particular name pattern.

To use find -name in a directory, follow these steps:

* Open a terminal window and navigate to the directory where you want to start the search.
* Type the following command:

      find . -name "filename"

* Replace filename with the name of the file or directory that you want to search for. The . indicates the current directory, but you can replace it with the path of the directory you want to search in.
* Press Enter to execute the command.
* The find command will search for all files and directories that match the specified name pattern in the directory hierarchy and print their paths to the terminal.
* For example, to search for all files with the extension .txt in the current directory and its subdirectories, you can use the following command:

      find . -name "*.txt"

> From this information I was able to gain a better understanding of the find function as well as explain the file -name use. I tried
> the function out on my own in VS Code as well which is the code for the use I have put on this lab report. 

***

**how to use find in command line bash different ways.**

---

The find command in Bash is a powerful tool for searching for files and directories in a directory hierarchy based on various criteria. Here are some different ways to use the find command in the command line:

* Find files by name:
To search for files with a specific name, use the -name option followed by the name pattern you want to search for. For example, to search for all files with the name "example.txt" in the current directory and its subdirectories, use the following command:
arduino

    find . -name "example.txt"

* Find files by type:
To search for files of a specific type, use the -type option followed by the type of file you want to search for. For example, to search for all directories in the current directory and its subdirectories, use the following command:

    find . -type d

* Find files by size:
To search for files of a specific size, use the -size option followed by the size of the file you want to search for. For example, to search for all files larger than 1 MB in the current directory and its subdirectories, use the following command:

    find . -size +1M

* Find files by modification time:
To search for files that have been modified within a specific time period, use the -mtime option followed by the number of days. For example, to search for all files modified within the last 7 days in the current directory and its subdirectories, use the following command:

    find . -mtime -7

* Find files by permissions:
To search for files with specific permissions, use the -perm option followed by the permission code. For example, to search for all files that are readable and writable by the owner in the current directory and its subdirectories, use the following command:

    find . -perm -600

* These are just a few examples of how you can use the find command in different ways. The find command has many more options and can be combined with other commands to perform more complex searches and actions.

> From this search result I was able to understand more applications of find, and chose a few to use for this lab report. I tried 
> out various functions on my own VS Code, and then selected a few for this lab report that provided me with interesting results. 
> Thus, the information I used from this search was implemented in this lab report through the application of the functions provided
> in my own VS Code. 

***

**can you give me some more options?**

---

Sure, here are some more options you can use with the find command in Bash:

* Find files by user:
To search for files owned by a specific user, use the -user option followed by the username. For example, to search for all files owned by the user "john" in the current directory and its subdirectories, use the following command:

    find . -user john

* Find files by group:
To search for files owned by a specific group, use the -group option followed by the group name. For example, to search for all files owned by the group "staff" in the current directory and its subdirectories, use the following command:

    find . -group staff

* Find files by file system:
To search for files on a specific file system, use the -xdev option followed by the name of the file system. For example, to search for all files on the file system "/dev/sda1" in the current directory and its subdirectories, use the following command:

    find . -xdev -mount -name "*.*"
The -mount option is used to only search the mounted file systems.

* Find files by inode:
To search for files by inode number, use the -inum option followed by the inode number. For example, to search for a file with an inode number of 1234567 in the current directory and its subdirectories, use the following command:

    find . -inum 1234567

* Find files by depth:
To search for files based on their depth in the directory hierarchy, use the -maxdepth and -mindepth options followed by the maximum and minimum depths, respectively. For example, to search for all files at a depth of 2 in the current directory and its subdirectories, use the following command:

    find . -maxdepth 2 -type f

* This will search for all regular files at a depth of 2 in the directory hierarchy.
These are just a few more examples of the many options you can use with the find command in Bash. The find command is a very powerful tool with many more options that can be combined to perform complex searches and actions.

> I was not able to find enough functions I liked from the previous search, thus I prompted ChatGPT to provide me with more option. 
> From this search result I was able to understand more applications of find, and chose a few to use for this lab report. I tried 
> out various functions on my own VS Code, and then selected a few for this lab report that provided me with interesting results. 
> Thus, the information I used from this search was implemented in this lab report through the application of the functions provided
> in my own VS Code. 

# Thank you!

