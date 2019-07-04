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

