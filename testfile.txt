# sudo adduser user1
# sudo adduser user1 sudo
# su -l user1 
 <!-- -l : is used for login   -->
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
<!-- ls -1 -->
<!-- ls -l -->
<!-- cd  --> change dierctory 
<!-- cd .. -->
<!-- cd ~ --> for home directory
<!-- mv test docker --> rename test folder to docker //  or we can say move 
mv test /etc : to move the folder
<!-- touch hello.txt --> create a new empty file hello.txt
<!-- rm file.txt -->
<!-- rm -r docker --> 
<!-- cat file.txt--> see content of a file 
<!-- cat file1.txt >file2.txt  --> to combine multiple files
<!-- cp a.txt b.txt -->  it is similar to above , copy the content of a.txt to b.txt
cp -i [Source_file] [Destination_file] 
cp -i a.txt b.txt  # this -i is for interactive 
cp -f a.txt b.txt


<!-- head -n 5 file.txt --> to see the first five line of a file
<!-- tail -n 4 file.txt  --> to see the last 4 line of a file
<!-- nano  --> to write something to a file
redirection 
standard input is keyboard , standard output is screen
<!-- echo hello --> simply show hello 
<!-- echo hello > hello.txt --> write heelo to a new file hello.txt













