<!-- Video by M prashant -->

# sudo adduser user1
        or
# sudo useradd user1        
# sudo adduser user1 sudo
# su -l user1 
<!-- -l : is used for login   -->

# id user1 
   it will give all the id details of user like: uid, gid 

<!-- How to change password for the user: -->
# passwd user1

<!-- to create a group  -->
# sudo groupadd TESTING
for seeing the group file
# cat /etc/group 

<!-- delete a user  -->
# sudo userdel user1

usermod -G TESTING nick

for playing with password;
chage [option]
-d, -m, -M ,-W,




# at 
to automate the command at given time;
# chrontab
# date
# date +%D
# date +%T:%D
# date +%T:%M
# date +%H:%M

# clear 
# ctrl + l
to clear linux command 




# curl "https://downloads.apache.org/kafka/2.8.2/kafka_2.13-2.8.2.tgz" -o ~/Downloads/kafka.tgz

curl: This is a command-line utility for transferring data from or to a server, using supported protocols such as HTTP, HTTPS, FTP, etc

-o ~/Downloads/kafka.tgz: This part specifies the output file path where the downloaded content should be saved. In this case, it's saving the downloaded file as "kafka.tgz" in the "/Downloads" directory, where "" represents the user's home directory.

# mkdir ~/kafka && cd ~/kafka
# tar -xvzf ~/Downloads/kafka.tgz --strip 1
tar command is used to extract the binary file from given directory
tar: This is a command-line utility used to manipulate archives in the tar format. It can be used to create, list, extract, and modify tar archives.

-xvzf: These are options provided to the tar command:

    x: This option tells tar to extract files from an archive.
    v: This option enables verbose mode, which displays the files being extracted.
    z: This option tells tar to use gzip compression for the archive.
    f: This option indicates that the next argument specifies the name of the archive file to work with.
--strip 1: This option tells tar to strip off the leading directory component when extracting files. In this case, it removes the top-level directory from the archive, so files will be extracted directly into the current directory rather than creating a new directory with the package name.

# nano ~/kafka/config/server.properties   
this will open the file server.properties usign text editor nano
for opening this file we can use  nano command.md 

# sudo nano /etc/systemd/system/zookeeper.service
/etc/systemd/system/zookeeper.service: This is the path to the zookeeper.service file. This file is typically located in the /etc/systemd/system/ directory and is used to define a systemd service for Apache Zookeeper. Editing this file allows you to configure how the Zookeeper service behaves when managed by systemd.


<!-- history  --> to know all comand till now we have executed
# history | grep sort
 it will return all the command used for sort in history
<!-- !2 --> execute that command number 
<!-- apt --> package manager to install package 
<!-- apt install nano -->
Most used commands:
  list - list packages based on package names
  search - search in package descriptions
  show - show package details
  install - install packages
  reinstall - reinstall packages
  remove - remove packages
  autoremove - Remove automatically all unused packages
  update - update list of available packages
  upgrade - upgrade the system by installing/upgrading packages
  full-upgrade - upgrade the system by removing/installing/upgrading packages
  edit-sources - edit the source information file
  satisfy - satisfy dependency strings
  <!-- apt update -->
  <!-- nano --> a text editor
  in linux every thing is a file , bin :(binary) program file, boot for boot files , dev for devices 

<!-- pwd --> present working directory
<!-- ls -->
<!-- ls -lt --> for more details like last modified
<!-- ls x* --> wildcard start with x;
<!-- ls -1 -->
<!-- ls -l -->
<!-- cd  --> change dierctory 
<!-- cd .. -->
<!-- cd ~ --> for home directory
<!-- mv test docker --> rename test folder to docker // 
mv test /etc : to move the folder
<!-- touch hello.txt --> create a new empty 
file hello.txt

# touch file{1..10} 
it will create files file1, file2, file3 .... only in one command

# shuf a.txt
for suffling 

# wc -l test.txt 
it will return number of line

# cmp fileA fileB
return yes or no after compare tow files

# diff -u fileA fileB
return the difference betweem line




<!-- rm file.txt -->
<!-- rm -r docker --> 
<!-- cat file.txt--> see content of a file 
<!-- cat file1.txt >file2.txt  --> to combine multiple files
<!-- cp a.txt b.txt -->  it is similar to above , copy the content of a.txt to b.txt
cp -i [Source_file] [Destination_file] 
cp -i a.txt b.txt  # this -i is for interactive, it will ask to confirm before copying 
cp -f a.txt b.txt  # -f for forceful copy


<!-- head -n 5 file.txt --> to see the first five line of a file
<!-- tail -n 4 file.txt  --> to see the last 4 line of a file
<!-- nano  --> to write something to a file
redirection 
standard input is keyboard , standard output is screen
<!-- echo hello --> simply show hello 
<!-- echo hello > hello.txt --> write heelo to a new file hello.txt


<!-- create a new file and edit and write the file in editor -->
# vi newfile.txt
press i for insert;
after insert press esc ; it will remove the insert and then press :wq it will save and exit;

# nano newfile.txt

# sort a.txt
# sort a.txt | unique
# split -l 4 a.txt




<!-- searching .......................................-->

# less a.txt
for searching , press /keywords 
it will display the keywords and pressing n it will display the next instance of that keyword
searching from bottom: ?keywords
press q to end

# more a.txt
read page by page
grep [options] pattern [files], grep is used for searching the pattern or keyword inside the file
# grep -i "UNix" geekfile.txt
here -i is used as case insensative, there can many type of options based on required output

gzip: Compress or decompress files using gzip compression

# egrep "Wordq | word2" a.txt

# find ./ -name filename
it will search in present directory as well as all inside directory

find: Search for files and directories.
# find /path/to/search -name "filename.txt"

# find /path/to/search -name "*.txt" | xargs rm

# gzip file.txt
# gzip -d file.txt.gz
gunzip: Decompress gzip files.
# gunzip file.txt.gz
     these can only we work with files not with folder

# tar -cvf archive.tar file1.txt file2.txt
    c means compress
# tar -xvf archive.tar 
# tar -cvf archive1.tar folder/
# zip archive.zip file1.txt file2.txt
# unzip archive.zip
# unzip -l a.zip 
it will not unzip the file only give info about how many files are compressed here


vim: A powerful text editor with many features.
# vim filename.txt
emacs: Another powerful text editor with extensive features.
# emacs filename.txt

# file a.txt 
return file type;

# du -h filename.txt
display disc usage by file

# df -h
diplay disc space usage



# which ls, which apt ,which python
we can execute these command to see from where this command are executing 

# man man , it is a manual for linux command;
# man -a passwd , shows the details of passwd command
# man -a ls
file /etc/ssh/sshd_config

# sudo apt install net-tools
it is used to install net tools like , ifconfig, 

rishuraj2401@DESKTOP-41EKJ51:~$ sudo ssh-keygen -A
ssh-keygen: generating new host keys: RSA DSA ECDSA ED25519


# ls --help 
it will show all the option avialable with help

<!-- how to use calculator in linux -->
# bc

# cal 
  calender
# cal 2023

# alias l="ls-ltr"




