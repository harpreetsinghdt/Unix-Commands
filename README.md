# Unix Commands (Pipes & Redirection)

## Pipes
> List all files & dirs
```
ls
```
> List all files & dirs in list format
```
ls -l
```
> Change directory 
```
cd <new dir>
```
> Print current directory
```
pwd
```
> Go to previous dir
```
cd ..
```
> Check content of a file
```
cat file1.txt
```
> Word count of a file
```
wc file1.txt -w
```
> count files & dirs
```
ls | wc -w
```
> Count words of a specific file
```
cat file1.txt | wc -w
```
> Count words from two files
```
cat file1.txt file2.txt | wc -w
```
## Redirection
> Standard Input (stdin - 0) -> Standard Outout (stdout - 1) -> Standard Error (stderr - 2)

> To input content to a file
```
cat > input1.txt
```
> To output content from a file
```
cat < input1.txt
```
> To put output into a file
```
ls -l > output.txt
```
> Check the output
```
less output.txt
```
> To Send error to a file use: 2> error.txt
```
ls -l /bin/usr 2> error.txt
```
> To send error to another file
```
ls -l /bin/usr > error_output.txt 2>&1
less error_output.txt
```

## Grep - Global regular expression print
> Fetch names witch start with Sam from names.txt file
```
grep Sam names.txt
grep sam names.txt
```
> Macth at the middle of string also
```
grep -i Sam names.txt
```
> Match exactly 
```
grep -w Sam names.txt
```
> To match from list within directory files
```
ls /bin
ls /bin | grep zip
```
