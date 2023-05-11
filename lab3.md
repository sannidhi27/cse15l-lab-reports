# Lab Report 3
*** 
## Command: Find.
*** 
1. `find -name`
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
4. `


