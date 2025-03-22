# devalla-jwala--Week-2-Linux-Fundamentals
Sapience Edu Connect Pvt Ltd -Internship task-2
## 1. Create a directory named my_project and navigate into it 
Step1:  
 mkdir my_project  
Step2:  
  cd my_project
##  2. Inside my_project, create an empty file named notes.txt. 
Step1:  
touch notes.txt
## 3. Copy notes.txt to a new file named backup_notes.txt, then move it into a newly created subdirectory called backup. 
Step1:

cp notes.txt backup_notes.txt 
 
Step2: 

mkdir backup
  
Step3: 

mv backup_notes.txt backup/
## 4. Delete the backup directory along with its contents. 
Step1: 

 rm -r backup
## 5. Create a file named script.sh, grant it executable permissions, and change its permissions so it is readable and executable only by the file owner. 

Step1:

 touch script.sh
 
Step2:

 chmod 700 script.sh 
## 6. Update your package manager's repository list, install the htop package, verify its installation, and then uninstall it. 
 
Step1: 

 sudo apt install htop
 
Step2: 

 htop –version  
 
Step3:

sudo apt remove htop
## 7. Check all running processes, identify the PID of a specific process(e.g., sleep if running), and terminate it using the kill command. 
 
Step1: 
 
 Sleep 60s 
 
Step2: 
 
ps aux | grep sleep 
 
 step3: 
 
kill <PID>
## 8. Display your machine's IP address, ping google.com to verifyconnectivity, and list all active network connections. 
Step1: 

 hostname -I  
 
Step2: 

 ping -c 4 google.com 
 
step3: 

 netstat -tuln
## 9. Addanewuser named testuser, switch to this user, and grant them sudo privileges. 
Step1:

 sudo adduser testuser 
 
step2: 

 sudo usermod -aG sudo testuser 
 
step3: 

 su – testuser
## 10. Write a shell script named hello.sh that outputs "Hello, World!" when executed. 
Step1: 

 echo -e '#!/bin/bash\necho "Hello, World!"' > hello.sh 
 
step2: 

 chmod +x hello.sh
## 11. Create a tarball of the my_project directory, extract its contents, and compress the tarball using gzip. 
Step1:

 tar -cvf my_project.tar my_project 
 
step2: 

 tar -xvf my_project.tar
 
step3: 

 gzip my_project.tar
## 12. Check the disk usage, memory usage, and CPU information of your system. 
 Step1:
 
df -h 
 
 step2: 

free -h 

step3: 
 
 lscpu
