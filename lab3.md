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
# Thank you!

