Shell Basics
Tips for executing shell scripts

$ chmod u+x ./shell_file
How to see your absolute path of your current directory.
$ pwd
/home/remilekun/Documents/github/alx/alx-system_engineering-devops
how to list all files in a directory.
$ ls
how to navigate to current users home directory.
$ cd ~
$ pwd

# /home/remilekun

Display current directory contents in a long format
$ ls -l
Display current directory contents in a long format, including hidden files
$ ls -l -a
Display current directory contents.
Long format
with user and group IDs displayed numerically and hidden files (starting with .)
$ ls -l -a -n
Create a script that creates a directory named my_first_directory in the /tmp/ directory.
$ mkdir /tmp/my_first_directory
Move the file betty from /tmp/ to /tmp/my_first_directory.
$ mv /tmp/betty /tmp/my_first_directory/betty
Delete the file betty.
The file betty is in /tmp/my_first_directory
$ rm /tmp/my_first_directory/betty
Delete the directory my_first_directory that is in the /tmp directory.
$ rm -r /tmp/my_first_directory
Write a script that changes the working directory to the previous one.
Before the task:

$ pwd

# /home/remilekun

$ ls

# Documents Downloads Pictures Public

cd Documents/github/alx
$ pwd

# /home/remilekun/Documents/github/alx

Main task code

$ cd -

# /home/remilekun

Write a script that lists all files (even ones with names beginning with a period character, which are normally hidden) in the current directory and the parent of the working directory and the /boot directory (in this order), in long format.
ls -la . .. /boot

# total 64

# drwxrwxr-x 2 remilekun remilekun 4096 Mar 3 21:34 .

# drwxrwxr-x 5 remilekun remilekun 4096 Mar 2 20:24 ..

# -rwxrw-r-- 1 remilekun remilekun 16 Mar 2 23:39 0-current_working_directory

Write a script that prints the type of the file named iamafile. The file iamafile will be in the /tmp directory when we will run your script.
file /tmp/iamafile

# /tmp/iamafile: ASCII text

Create a symbolic link to /bin/ls, named ls. The symbolic link should be created in the current working directory.
ln -s /bin/ls **ls**
