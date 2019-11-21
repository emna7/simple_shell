# Simple Shell

## General info
the shell is a program that takes commands from the keyboard and gives them to the operating system to perform.
In the old days, it was the only user interface available on a Unix-like system such as Linux.
Nowadays, we have graphical user interfaces (GUIs) in addition to command line interfaces (CLIs) such as the shell.

## List of functions and system calls:
* access 
* chdir
* close
* malloc
* strtok
* wait
* getline
* free
* fork
* exit
* env
* perror
* stat
* write

## Compilation
the shell will be compiled this way:
gcc -Wall -Werror -Wextra -pedantic *.c -o hsh

## Testing
### shell should work like this in interactive mode:
$ ./hsh
($) /bin/ls
hsh main.c shell.c
($)
($) exit
$

### But also in non-interactive mode:
$ echo "/bin/ls" | ./hsh
hsh main.c shell.c test_ls_2
$
$ cat test_ls_2
/bin/ls
/bin/ls
$
$ cat test_ls_2 | ./hsh
hsh main.c shell.c test_ls_2
hsh main.c shell.c test_ls_2
$

## Mandatory tasks
* 0. README, man, AUTHORS
* 1. A code that passes the Betty checks
* 2. Simple shell 0.1
 A UNIX command line interpreter.
* 3. Simple shell 0.2
 Handle command lines with arguments
* 4. Simple shell 0.3
 Handle the PATH
* 5. Simple shell 0.4
 Implement the exit built-in, that exits the shell
* 6. Simple shell 1.0
 Implement the env built-in, that prints the current environment
* 7. What happens when you type ls -l in the shell 
a blog post describing step by step what happens when you type ls -l and hit Enter in a shell

## Authors
* Emna Ben Hadj Messaoud
* Iheb Mejri
