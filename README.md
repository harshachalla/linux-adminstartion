# linux-adminstartion




linux-distributions:

--->distribution is simply a collection of software and applications bundled,together and distributed as a single operating system. For example, one Linux


---.>Distribution shortened to distro. Also, some people refer to the various
distributions as flavors. 

--->What every Linux distribution has in common,
	though, is the Linux kernel. Again, typically when the term Linux is used it refers to the
	Linux Operating System as a whole.

--->However, it can refer to just the Linux Kernel as well. 

--->The Linux kernel is the
	core or the heart of the Operating System. It’s the layer that sits between
	the hardware and applications. 

--->Said another way, it’s the intermediary
	between software and hardware.


*opening terminal in centos

--->click--->applications--->systemtools--->terminal.


--->toexit from the terminal --->just type "exit"





# About SSH

--->If you're going to connect to a Linux system over the network,
	more than likely you're going to use SSH.

## SSH stands for Secure Shell.

### SSH is a network protocol.

It's primary purpose is to allow you to connect,
from one system to another system, 
## "securely over a network".




----> In order to connect to Linux over the network,we're going to need a terminal emulator,that also acts as an SSH 	client.

---->For windows, the most popular SSH client and terminal emulator,
	is a program called, PuTTY.



# Terminal Emulator

------> A terminal emulator allows a host computer to access another computer, including remote ones, through either a command-line interface or a graphical one. The communication is made possible using protocols such as Telnet and SSH.


# 3rd july work



# Linux directory structure

#### The Linux directory structure is like a tree.

----> some of the most common top level directories,that you'll see when using the Linux operating system.

###### The base of the Linux file system hierarchy begins at the root. Directories will start to branch off the root;but everything starts at "root".

### The directory separator in Linux is symbolized by a forward slash, '/'.


------> If you hear someone say look in slash or that file is in slash,they're referring to the root directory.



# some of the most common top level directories

###### 'bin' or '/bin' is where you'll find binary files or executable files.

###### '/etc' or 'etsy' is where you'll find configuration files.

###### '/home' is where user home directories live.


###### 'opt' is where optional or third party software lives.(Opt is for software that is not bundled with the operating system.)

-----> For example Google earth is not part of the standard Linux operating system.So Google earth gets installed in opt.




###### '/tmp' is called temp and it's for temporary space.(Now temp is a great place to store temporary files)




###### '/usr' is called userand this is where user related programs live.Each one of these directories can have subdirectories.


###### '/var', also called, var, is for variable data.Think of things that change often.


--->Some Linux operating systems use /srv
	as a location to place data that is served by the Linux server.

---->For example, web files would be in /srv/www

----->or if it's an FTP server,


------>Let's take this fictitious application called, 'myapp' for example.
Even though the main 'myapp' program
gets installed on /opt/myapp/,
where maybe the binaries live and the libraries live,
you'll also see that you can install files
at /etc/opt/myapp.and that's where you'd find the configuration files.
maybe the files would be located in /srv/ftp.

----->The log files would be in /var/opt/myapp.


------>Sometimes when applications get installed,
they're not given their own directory structure,
they're installed in the shared manner.
So maybe, my app gets installed in /usr/local.
In this case, it would be /usr/local/bin/myapp
and the configuration file could be /usr/local/etc/myapp.com.

----> /usr/local/bin will not only contain my app.


# About Shell

#### The shell is the default user interface to a Linux system.

##### When you log in to a Linux server over the network,the shell is a program that is startedand it acts as your default interface to the system.

###The graphical user interface (log in to a Linux server with out network ) on a Linux system is also called a shell,
 ## "it's a graphical shell".


 ###The shell is really nothing more than an application or program that takes the commands you feed it, and it executes those commands for you.



 ----->In this case, Linux as we are at Linux server.

# At the end of the prompt you'll see a dollar sign.This is an indication that you're using the system,as a "normal user " as opposed to a super user.

# The super user shell prompt ends,typically with a "pound sign (#)".


#The super user on a Linux system, is also called root; it's the root account.

# The Tilde(~) is a shorthand way of representing a home directory.


# Basic Linux Commands

## 'ls' --->  list directories

## 'ls -l' ---> list directory contents.

## 'cd filename' -----> is the change directory command.


## 'cd'  --->take u to home directory

## 'cd -'  --->take u to previous directory

##  'pwd' command displays the present working directory

## 'cat' - concatenate files. Really what cat does is - it displays the contents of files.

## 'echo' displays arguments to the screen.


##  'man -ls' to display the documentation

## To exit or log out of your shell, use the 'exit' command.

## Finally, 'clear' clears the screen.



# Working with directories And commands


## 'cd..' is go to the parent directory.

## 'cd..' is go to the Present directory.


## 'echo $oldpwd' is go to the previous hold directory.

## 'slash' is a directory separator.

## 'mkdir' is make a new directory

## 'mkdir [-p]' here -p is refer as parent directory --->example : mkdir -p dirname1/dirname2

## 'rm-rf dir1' If we want to recursively remove them, we can use 'rm-rf dir1'

##'rmdir dir1' to remove directory


# understanding listing 

## 'ls -la , ls -l -a , ls -al , ls -a -l' If we want to see a long listing output that includes hidden files

		--------> You can run '-l' for long listing and '-a' for all files.


## 'ls -F' You can use  to reveal file types. 


#'ls -F' appends a character to a file or directory name that tells you what it is.
### So if it ends in '/' or forward slash, then it's a <u>"directory".</u>
### If it ends in '%', that's a link.
### A star or asterisk (*) means that it's executable.

## 'ls -t'.If you want to list files sorted by time
## 'ls -r'.If you want to list files sorted by reverse

## 'ls -latr' This provides a long listing that includes all files sorted by time in reverse.


## If any file is with spaces 
#### for example u have a file called harsha file.txt then u need to find the file so u will use cmd "ls -l" , as a result u wont get the file in list because in linux spaces are not allowed 
## 	to find these space named files we use cmd as 
# ls -l "harsha file.txt"

# 'ls -d' lists directory names not contents.


# 4th july work

# File and Directory Permissions


1. Here is some output from an 'ls -l' command.And if you look at the permissions string **(-rw-r--r--)**
+ the first character will indicate
 * whether it's a regular **file** by beginning with a **-**,
 * or it will begin with the **'d'** if it's a **directory**,
 * or an **'l'** if it's a **symbolic link.**


2. r, w and x represent the 3 main types of permissions.

 * They are read, which is r,

* write, which is w,

* and execute which is x.

3. `-r--rw-rwx` Observe this First charecter represents **type**  that means in `-r--rw-rwx` **-** is a **file type**
	* Observe this **Second 3 charecter** represents **user**  that means in `-r--rw-rwx` **r--** is a **User Permissions** . Represents with letter **u**
	* Observe this **third 3 charecter** represents **group**  that means in `-r--rw-rwx` **rw-** is a **group Permissions** . Represents with letter **g**
	* Observe this **Final 3 charecter** represents **other**  that means in `-r--rw-rwx` **rwx** is a **other Permissions**. Represents with letter **o**

	4. if a particular permission is not granted, a hyphen will take its place.
	* Permissions are also known as modes.
	* That's why the command you used to change permissions is called `chmod`, which is short for **change mode**

	5. We can change a file permissions by using following commands

	* `chmode u+w harsha.txt`  results `-rw-rw-rwx`
	* ` chmode g+x harsha.txt` results `-rw-rwxrwx`
	* ` chmode o-w harsha.txt` results `-rw-rw-rw-`
	* ` chmode u+wx harsha.txt` results `-rwxrw-rwx`

	**Above commands are based by using symbolic(u,g,o) permissions**

	**Numeric Commands based permissions**


	**Here are the most commonly used permissions.** 

* So 700 ensures that a file can be read, edited and executed by the owner and no one else on the system will have access to that file.
* The 755 permission allows everyone on the system to execute the file but only the user or the owner of the file can edit that file.

* 664 allows a group of people to modify the file and let others read it.

* 660 allows a group of people to modify the file and not let others read it.

* 644 allows everyone on the system to read the file but only the user or the owner of that file can edit that file.



	* ` chmode 700 harsha.txt` results `-rwx-------`
	* ` chmode 755 harsha.txt` results `-rwx-r-x--x`
	* ` chmode 664 harsha.txt` results `-rw-rw-r--`

* similarly so many numeric permissions are there 

# find files and directories.

1. If you don't tell find what to look for, it just returns all the files that are in your current directory.and all the subdirectories below that directory.
  
  * In terminal when u type ` find` results all the files that are in your current directory,and all the subdirectories below that directory.

  * ` find . -name Downloads` here **.** indicates that u r in current directory , and **-name** that indicates what the file/directory name u r searching for, so here i am serching for "Downloads"  
   * ` find . -iname Downloads` here **i** is for to ignore the name case either it may be small or capital letters it will show results

   **You can search for files by modification time by using the '-mtime' option to find.**

   * Let's look for files that are more than 10 days old, but less than 13 days old in the current directory.

   **Command is**   ` find . -mtime +10 -mtime -13` 

   **You can also search for files based on size using '-size'.**
   * Let's look for files that are more than **1kb size**.

   **Command is** ` find . -size +1k`
     * Let's look for files that are more than **1mb size**.

   **Command is** ` find . -size +1M`
     * Let's look for files that are more than **1Gb size**.

   **Command is** ` find . -size +1G`

   
#  about VI editor

1.  VI(Visual Instrument), you can even use vi mode for editing shell commands.
	* vi has the concept of modes.
	* You are always working in one of three modes -

	* **command mode**
	* **insert mode** 
	* **line mode.**

	* **k** goes up one line, **j** down.

	* **h** left, '**l** right one character.

	* To move right one word, **w**,

	* **b** moves back one word or left one word.

	* The **^** symbol takes you to the beginning of the line

	* while the **$** symbol takes you to the end of the line.


	* In order to insert text in a file, enter vi's insert mode.

	* Do this by pressing **i**

	* **'I', 'a', or 'A'.**

	* **'i'** inserts text at the current cursor position.

	* **'I'** inserts text at the beginning of the line.

	* **'a'** appends after the cursor position,

	* **'A'** appends to the end of the line.

	* to write the file or save the file, type **:w**, enter.
	* To force a file to be saved, type **:w!**.

	* To quit, **:q**, 
	* to force quit, **:q!**.

	* To save the file and quit, or write and quit, **:wq!**.

	* And **:x** is the same as **:wq**

	* if you want to go to the line 15 in the file, type **:15** enter.

	* To go to the last line of the file, type **:$**.

	* If you want to see line numbers, type **:set nu**.

	* And to turn off line numbering, **:set nonu**.

	* To get help, type **:help** and the command that you're interested in.

	* Again the modes in vi or command mode which you can enter by hitting the **escape key.**

	* While in command mode you can use **x** to delete a character.

	* **dw** to delete a word,

	* **dd** to delete a line

	* and **D** to delete the remaining text on the line.


	* To replace text, type **r** for just one character,

	* **cw** to change an entire word,

	* **cc** to change in entire line,

	* **c$** to change the text from the current position to the end of the line.

	* You can also use **C** for that.

	* The **~** command reverses the case of the character.

	* To yank or copy the current line, type **yy**

	* To yank a position type **y** and a position character.

	* For instance, to yank a word, type **yw**

	* If we want to repeat this, you could yank 3 words with **y3w**.

	* **p** will paste the most recently deleted or yanked text.

	* The undo command in vi is **u**

	* and the redo command is **ctrl-R**.

	* To start a forward search, type **/** and a search pattern and hit enter.

	* To go to the next match, type **n**.

	* To go to the previous match, type **N**.

	* To start a reverse search, use the '**?**
	  
# Delete , Copy , move files
* want to delete some of them.To do that, use the **rm** command.

**rm filename** is the simplest form of this command.

* If you want to remove a directory and its contents recursively, use '**rm -r** and the name of the directory.

* If you want a forced removal, use **rm-f**.

* To copy files, use the **cp** command.

* If you want to create a copy of a file, you just run **cp src_file destination_file**.

* To run cp in interactive mode, use **cp -i**.If the destination file exists, cp will prompt you before it overwrites the file.

* If you use **cp -r source_directory destination**,'cp' will recursively copy source directory into the destination directory.If the destination directory doesn't exist,it will create the destination directory.with the contents of the source directory.

* To move or rename files, use the **mv** command.

* If you were to run **mv source destination**, 'move' will move the source into the destination. Otherwise, source 	will be **renamed destination.**

* If we run **mv file1 file2**,that will rename file1 to file2.It will overwrite file2.

* If you want to do this in interactive mode, use **-i**.In this case it says, 'Hey there's a file that already exist. You want to overwrite it or not'?

* **sort** is used for sorting

* You can use sort with a **sort -k2**(removes the 2nd line,if u provide 3 it removes 3rd line) option and supply a field, so you can sort by a different field than the first field.

* **sort -r** sorts in reverse order

* and **sort -u** removes duplicate lines

* You may want to create a copy or back up of a group of files.You may also have several files that you want to transfer at once or transfer as a set.In these situations, **tar** can help.

* **tar cf what file name u r going to give.tar which file u r going to compress**  Create a tar archive.
* **tar tf  which tar file u want to see** it shows the directory and files 

similarlly.......

* **x** Extract files from the archive.
* **v** Be verbose.
* **z** Use compression.

### Compressing Files To Save Space

* **gzip filename** Compress files.
* **gunzip filename** Uncompress files.
* **gzcat filename** Concatenates compressed files.
* **zcat filename** Concatenates compressed files.


### Disk Usage

* **du** Estimates file usage.
* **du -k** Display sizes in Kilobytes.
* **du -h** Display sizes in human readable format.

# 5th july Work


### Wildcards

**A wildcard is a character or a string that is used to match file and directory names.**

* Here are the 2 main wildcards.They are the **asterisk(*)** and the **question mark(?)**.

* For example, we could use ***.txt** to find all the files that end in '.txt'.

* If you wanted to list all the files that start with the letter **a**, then use **a***.