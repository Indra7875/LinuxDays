


### day4

### Command Input + Output
* There are two ways to get data into a command and two ways to get data out.
* The ways in are standard input and command-line arguments and the ways out are standard output and error.
* Standard Input, Standard Output, and Standard Error are "Standard Data Streams".
* Every data stream not only has a name like standard output and standard input but also has a number associated with it.
  * Standard Input = 0
  * Standard Output = 1
  * Standard Error = 2
* Data streams can be redirected from their default location to wherever you wish.
* You can redirect the standard output of one command to the standard input of another in a process known as "piping".
### Redirection
```
$ cat
```
-- cat command is used to concatenate all stick together multiple different files.
```
$ cat 1> output.txt
```
-- It will redirect the standard output in the output.txt file. Previous data will erase.
```
$ cat > output.txt
```
-- It will redirect the standard output in the output.txt file. Previous data will erase.
```
$ cat 1>> output.txt
```
-- It will redirect the standard output in the output.txt file. Previous data remain as it is.
```
$ cat >> output.txt
```
-- It will redirect the standard output in the output.txt file. Previous data remain as it is.
```
$ cat input 2> error.txt
```
-- It will redirect the standard error in the error.txt file. Previous data will erase.
```
$ cat input 2>> error.txt
```
-- It will redirect the standard error in the error.txt file. Previous data remain as it is.
```
$ cat 1>> output.txt 2>> errror.txt
```
-- It will redirect the standard output in the output.txt file as well as It will redirect the standard error in the error.txt file. Previous data remain as it is.
```
$ cat >> output.txt 2>> errror.txt
```
-- It will redirect the standard output in the output.txt file as well as It will redirect the standard error in the error.txt file. Previous data remain as it is.
```
$ cat 0< input.txt
```
-- It will redirect the standard input in the input.txt file. Previous data will erase.
```
$ cat < input.txt
```
-- It will redirect the standard input in the input.txt file. Previous data will erase.
```
$ cat >> input.txt
Hii..How are you..?
$ cat < input.txt >> hello.txt
$ cat < hello.txt
Hii..How are you..?
```
-- Here we first redirect the data to input.txt then take the data from the input.txt file and append it in the hello.txt file and at the last read the data from the hello.txt file.
```
$ tty
```
-- It will show us where the terminal is located.
```
$ cat < hello.txt > /dev/pts/1
```
-- It will read the data from hello.txt and append it in the second terminal.
