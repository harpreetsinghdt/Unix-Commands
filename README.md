# Unix Commands (Pipes & Redirection)

### List all files & dirs
```
ls
```
## List all files & dirs in list format
```
ls -l
```
## Change directory 
```
cd <new dir>
```
## Print current directory
```
pwd
```
## Check content of a file
```
cat file1.txt
```
## Word count of a file
```
wc file1.txt -w
```
## count files & dirs
```
ls | wc -w
```
## Count words of a specific file
```
cat file1.txt | wc -w
```
## Count words from two files
```
cat file1.txt file2.txt | wc -w
```
## 