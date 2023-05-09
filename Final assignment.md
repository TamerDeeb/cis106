---
Name: Tamer Deeb
Course: CIS 106
Semester: Spring 23
---

## final assignment 

### Question 1 
for every command in this list, include the following:
1. Description 
2. formula/syntax 
3. 3 examples that you understand well

* awk: Allows users to process and manipulate data to produce formatted reports.
    * Ex1: print a list of all the users in your system `awk ~F '{print $1}' /etc/passwd`
    * Ex2:print a list of all users in your system with their login
      shell: `awk ~F{print $1,$NF}' /etc/passwd`
    * Ex3: Repeat the previous command but make the usernames uppercase: `awk ~F '{print toupper$1,$NF}' /etc/passwd` 
  
  
* cat: reads each file parameter in sequence and writes it to standard output.
  * Ex1: `cat todo. list`
  * Ex2: `cat ~/Documents/todo.list` 
  * Ex3: `cat ~b ~Documents/todo.md`
  
* cp: use the cp command to create a copy of the contents of the file or directory.
  * Ex1: `cp ~/Picturers/Dogs/ ~/Documents/Pets/`
  * Ex2: `cp ~/Documents/cats/ ~/Documents/Tabby/`
  * Ex3: `cp ~/Downloads/file1 ~/Documents/file`
   
* cut: cut out sections of a specified file or piped data and print the result to standard output.
  * Ex1: `cut ~d '"' ~f1 /etc/passwd`
  * Ex2: `cut ~d '"' ~f1,7 /etc/passwd` 
  * Ex3: `cut ~b 1-5 usernames.txt`
  
* grep: search for a sting in groups of files.
  * Ex1:`grep 'Harry potter' ~/Documents/Prisoner0fAzkaban,txt`
  * Ex2:`grep ~v 'Voldemort'  ~/Documents/Prisoner0fAzkaban,txt`
  * Ex3:`grep ~o 'Ron Wesley' ~/Documents/Prisoner0fAzkaban,txt`
  
* head: writes to standard output a specified number of lines or bytes of each of the specified files, or of the standard input.
  * Ex1: `Head ~/Documents/Book/Dracula,txt`
  * Ex2: `Head -5 ~/Documents/Book/Dracula,txt`
  * Ex3: `Head -10 ~/Documents/Book/Dracula,txt`
  
* ls: list the names and features of files and directories0.
  * Ex1: `ls ~/Documents/`
  * Ex2: `ls ~/Documents/Dogs/`
  * Ex3: `ls ~ ~/Weekly Reports/` 
  
* man: display the user manual of any command that we can run on the terminal. 
  * Ex1: `man printf`
  * Ex2: `man 2 intro`
  * Ex3: `man ~f ls`
  
* mkdir: create or make new directories. 
  * Ex1: `mkdir HomeDecor`
  * Ex2: `mkdir {dir1,dir2}`
  * Ex3: `mkdir ~v Pets`
  
* mv: move files and directories from one directories to another or to rename a file or directory.
  * Ex1: `mv sample.txt ~/Documents/`
  * Ex2: `mv dir1 dir2`
  * Ex3: `test.txt ~/TextFiles/`
  
* tac: display the file content in reverse order.
  * Ex1: `tac todo.md`
  * Ex2: `tac ~/Documents/todo.md`
  * Ex3: `tac ~/Final Project/Deliverable 2.pdf`
  
* tail: prints the last few number of line (10 lines by default) of a certain file, then terminates.
  * Ex1: `tail ~/Documents/Book/dracula.txt`
  * Ex2: `tail -5 ~/Documents/Book/dracula.txt`
  * Ex3: `tail -10 ~/Documents/Book/dracula.txt`
  
* touch: creates new files, modifies timestamp, changes access time for any file. 
  * Ex1: `touch cats.txt`
  * Ex2: `touch Project.docx`
  * Ex3: `touch Grocery.lst`

* tr: used to translate a string of text from one language to another.
  * Ex1: `cat file.txt | tr '.' ','`
  * Ex2: `cat program.py | tr "[:space:]" '/t'`
  * Ex3: `cat file.py | tr -5 "[:space:]" ''`
  
* tree: displays directory path and files in each subdirectory.
  * Ex1: `tree cars`
  * Ex2: `tree Lab1`
  * Ex3: `tree Homework`
  
### Question 2
answer each question:
   
* How to work with multiple terminals open?
* You can use applications such as Tilix to open multiple terminals, or if you're using the default terminal press CTRL+Shift+T.
* 
* How to work with manual pages? 
* Open your terminal and use the `man` command in order to open the manual.
* 
* How to parse (search) for specific words in the manual page
* You can parse for specific words in the manual using the `grep` command.
* 
* How to redirect output (> and |)
* You can redirect output using the greater than or pipe symbols.
* Ex: $ echo line 1 > users 
      $ cat users 
      line 1

* How to append the output of a command to a file
   1. open terminal 
   2. Append text to end of file using `echo` command: `echo  'text' >> filename` 
   3. Append command output to end of file: commandname >> filename 
  
   * How to use wildcards
       For copying and moving multiple files at the same time:
       Ex: file1 file2 file3 can be moved all at once using the * wildcard by typing `mv file*` in order to move all files that start with that same first ward.

* How to use brace expansion
    * For creating entire directory structures in a single command
    * Ex: `mkdir ~p subjects/{Math,Art,IT}/{Homework,Projects}`.
