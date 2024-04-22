# hostname
# lscpu 
cpu architechture

# lsblk
list of storage device disk partition on your linux server

# uname -a
name of operating system and all 
# cat /etc/os-release
details about the operating system


# sudo service nginx start
# sudo service nginx status


# ps -ef 
  sare processs aa jayenge jo running hai


<!-- How to check process java is running or not -->
# ps -ef | grep java
 grep means searching, from all running process we need to search java

<!-- rishura+ 24474   423  0 17:45 pts/5    00:00:00 grep --color=auto java --> java was not running we didn't get any pid but we get a pid for the command which we have executed so the command also become a process here;



<!-- How to get process id of process; -->
# pgrep nginx
it will return the process id 

<!-- HOw to stop a process by processId? -->
# sudo kill -9 24020
-9 is for forcefully

<!-- How to stop a process by it's name -->
# sudo pkill nginx


# sleep 10s 
terminal will sleep for 10s;
 ctrl + Z we stop a process, 
using #jobs we can see which are the process need to done 
<!-- How to see all the active jobs -->
# jobs

<!-- How to resume a job in background -->
# bg
the jobs will start executing in background

<!-- How to resume a job in foreground  -->
# fg

<!-- How to run a script in background -->
# nohup ./script >/dev/null &

# vi myscript.sh
#!/bin/bash
echo "what is your name"
read name

echo "Welcome $name"

# script
it will create a file typescript and save all the command here  
ctrl+D , it will exit and save the command;

