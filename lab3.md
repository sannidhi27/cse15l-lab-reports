# Lab Report 3
*** 
## Command: Find.
The command I chose for this lab report was find. 
*** 
1. `find -name`
find -name is used to find any keyword/directory/file within the main directory it is within, which in this case is ./technical.
> Example 1:
> Command Line:
```
>sannidhikrovvidi@Sannidhis-MacBook-Pro technical % find . -name "*plos"   
```
> Output:
```
./plos
```
> Example 2:
> Command Line:
```
sannidhikrovvidi@Sannidhis-MacBook-Pro technical % find . -name "*chapter-1.txt"
```
> Output:
```
./911report/chapter-1.txt
```
***
2. `find "name" type -f`
> Example 1:
> Command Line:
```
sannidhikrovvidi@Sannidhis-MacBook-Pro technical % find . -type f -name "*preface.txt"
```
> Output: 
```
./911report/preface.txt
```
> Example 2:
> Command Line: 
```
sannidhikrovvidi@Sannidhis-MacBook-Pro technical % find . -type f -name "*commission_report.txt"
```
> Output:
```
./government/About_LSC/commission_report.txt
```
***
3. `find -name "name" -and -type d`
> Example 1:
> Command Line:
```
sannidhikrovvidi@Sannidhis-MacBook-Pro technical % find . -type f -name "*Annual_Fee.txt"
```
> Output:
```
./government/Media/Annual_Fee.txt
```
> Example 2: 
> Command Line:
```
sannidhikrovvidi@Sannidhis-MacBook-Pro technical % find . -type f -name "*journal.pbio.0020001.txt"
```
> Output:
```
./plos/journal.pbio.0020001.txt
```
***
4. FIND 
> Example 1:
> Command Line:
```
sannidhikrovvidi@Sannidhis-MacBook-Pro technical % find . -perm -600
```
> Output:
```
...
./biomed/1471-2121-4-4.txt
./biomed/gb-2003-4-4-r28.txt
./biomed/1471-230X-2-17.txt
./biomed/1477-5956-1-1.txt
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
./911report/chapter-11.txt ...
```
> Example 2:
> Command Line:
```
sannidhikrovvidi@Sannidhis-MacBook-Pro technical % find . -perm -700
```
> Output:
```
...
./biomed/1471-2180-2-13.txt
./biomed/1471-2121-4-4.txt
./biomed/gb-2003-4-4-r28.txt
./biomed/1471-230X-2-17.txt
./biomed/1477-5956-1-1.txt
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
***
# Thank you!

