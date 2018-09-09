# Learn command line

Please follow and complete the free online [Bash Scripting Tutorial](https://ryanstutorials.net/bash-scripting-tutorial/) or [Codecademy's Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line). These are helpful tutorials. You should be able to go through these in a couple of hours.

**Note:** Bash is not installed on a PC. Rather, PC users must install Cygwin. Once Cygwin has been installed, the command line interface witll _emulate_ bash. You can find all information regarding Cygwin [here](https://www.cygwin.com/).

---

### Q1.  Cheat Sheet of Commands  

Here's a list of items with which you should be familiar:  
* show current working directory path
* creating a directory
* deleting a directory
* creating a file using `touch` command
* deleting a file
* renaming a file
* listing hidden files
* copying a file from one directory to another

Make a cheat sheet for yourself: a list of at least **ten** commands and what they do.  (Use the 8 items above and add a couple of your own.)  

> >
1. pwd: print working directory
2. mkdir: create a directory
3. rmdir: remove/delete empty directories
4. touch <file>:
	-creates file
	-modify time stamp with -t option
	-if trying to modify but do no want to create by mistake use -c option  
5. rm:
	-delete file
	-use -r option to delete directories, especially when they are not empty
	-use -i option in combination with -r to verify each file/subdirectory being deleted in directory
6. mv <file> <desination>: moves files to new destionation
7. mv <file> <new_file_name>: use move command to rename file. Instead of specifying new destination provide new name.
8.ls: list files/directories in current working directory. Files and directory are used synonymously. 
	- -a list all files. Includes hidden files, which are designated with a '.' before the file name (i.e. .file) 
	- -l list files in long version. Includes permissions, users/groups, byte size, and modification timestamp
	- -t list files in order of modification time

9. cp <file> <destination>:
	-Duplicates file to new desination
	-Duplicates file to same directory with different name
10. man <command>: pulls up manual page for command
	- -k <search term> pulls up commands similar to searched term
> >

---

### Q2.  List Files in Unix  
What do the following commands do:  
`ls`  
`ls -a`  
`ls -l`  
`ls -lh`  
`ls -lah`  
`ls -t`  
`ls -Glp`  

> >
ls: 	list nonhidden files/directory in working/specified directory
ls -a: 	list all files/directoies, including those that are hidden
ls -l:	list long format: file or directory, permissions for each user type, number of links, owner then group name, byte size, etc
ls -lh: includes units for the size listed (B for bytes, KB for kilobytes, etc.)
ls -lah: long format with size unites for all files/directories, including those that are hidden
ls -t: list files in descending order(most recent first) based off last modified
ls -Glp: list in colorized long format to include slashes (/) after the name if listing is a directory 
> >

---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

> > 
1. ls -1: lists in single column format
2. ls -m: lists in single row separated by commas
3. ls -r: reverse lexicorgraphical order (prints in opposite order)
4. ls -S: lists by size
5. ls -Tl: lists in long formate with long form of modification timestamp
> >

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> > Xargs builds and executes command line from standard input.
For example, echo '1 2 3' | xargs mkdir , would create three new directories.

