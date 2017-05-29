# Learn command line

Please follow and complete the free online [Command Line Crash Course
tutorial](https://web.archive.org/web/20160708171659/http://cli.learncodethehardway.org/book/) or [Codecademy's Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line). These are helpful tutorials. Each "chapter" focuses on a command. Type the commands you see in the _Do This_ section, and read the _You Learned This_ section. Move on to the next chapter. You should be able to go through these in a couple of hours.

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


1. `pwd` shows the current working directory path.  
2. `mkdir dirname` creates a new directory of title 'dirname'.  
3. `rmdir dirname` deletes the directory of title 'dirname.  
4. `touch filename` creates a files with name 'filename'
5. `rm filename` deletes the file with name 'filename'
6. `mv file1 file2` would rename file1 to file2
7. `ls -a` would show hidden files
8. `mv dir1/file1 dir2/file1` would move file 1 from dir1 to dir2
9. `touch filename` creates a blank file with name 'filename'
10. `man man` opens the manual for help on using the man command

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

> > `ls` lists the director contents.  
`-a` flag forces all files to be displayed (files starting with . are ignored by default).  
`-l` flag gives you a long format list, showing additional information like file size and when it was last modified.  
`-h` flag prints sizes in a human readable format.  
`-t` sorts the files shown in order of modification time.  
`-G` prevents group information from being displayed.  
`-p` appends file type indicator to the entries.  
The commands above are just combinations of these flags.

---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

> > `-R` because showing subdirectories seems useful.  
`-1` because separating each file on its own line without the mess of information from `-l` is useful.  
`-d` because showing only directories is useful.  
`-m` because this seems useful for extracing information.  
`-i` because it looks funny

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> > `xargs` can take a stream of inputs and apply a command to all of them in turn.  This is useful for iterating over multiple files from the command line and can be used in combination with commands like find to filter through different file types or directories. for example the command `find . -name "*.jpg" | xargs tar -czvf jpegs.tgz` to find all the .jpg files in a directory and then zip them into a single file jpegs.tgz

 

