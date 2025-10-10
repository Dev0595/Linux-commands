# Linux-commands
1.	To create a new User?

  	 `Sudo adduser username`
  	
     Ex: `Sudo adduser "aariz"`
  	
2. 	To change user password?

     `Sudo passwd username`

     Ex: `Sudo passwd aariz`
   	
3.	To change username?

    `Sudo usermod -l newname oldname`

   Ex: `Sudo usermod -l aariz1 aariz`
   
4. 	To delete an existing user?

  `Sudo userdel username`

  Ex: `Sudo userdel aariz`
  
5. 	To lock a useraccount?

  `Sudo passwd -l username`

  Ex: `Sudo passwd -l aariz`
  
6. 	To unlock a user account?	

  `Sudo passwd -u username`

  Ex: `Sudo passwd -u aariz`

7. To create a directory

   `mkdir diretory_name`

   Ex: `mkdir devops`

8. To create a file

   `touch file_name`

   Ex: `touch file1.txt`

9. To create a multiple files using single command?

      `touch script.sh{1..9}`


11. To copy a file from one home directory to another directory?

   `cp /home/source-dir/filename /home/target-dir/`
   

   Ex: `cp /home/aariz/file.txt /home/linuxdev/`
   

11. To move a file

   `Mv /home/source-dir/filename /home/target-dir/`

   
   Ex: `mv /home/aariz/file2.txt /home/linuxdev/`
   

11. To view a file

    `cat file_name`


    Ex: `Cat file.txt`

13. To display first few lines of text in a file?

    `cat head -n file-name`
    
    Ex: `cat head -n 5 file.txt`
    "This will display the first five lines in the textfile without counting spaces

    Ex: `cat head -5 file.txt`
    "This will display the first five lines of the text including spaces.

15. To check users list

    `cat /etc/passwd`
    "You will see the list of users created"


16. To excute a file in Linux

     `./file-name`


!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!**aariz@Areef:/home$**!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
                      
                        
                        ****The above path is explained in detail below****
                  - aariz → This is the username you're logged in as.
                 - Areef → This is the hostname of the computer or virtual machine.
                - /home → This is your current working directory — you're inside the /home folder.
               - $ → This symbol means you're a regular user (not root). If it were #, you'd be root.




**!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!  **File Permission**  !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!**



    *U- User*
    *G- Group*
    *O- Other*



    *r- Read*      *W- Write*   *X- Excute*



__Numeric Values of rwx__


    *r- 4*
    
    *w- 2*
    
    *x- 1*

###Commands


     1. To modify the r(Read) w(write) x(Excute) permission of a file to a *user*?

       `Chmod u=rwx file-name`

       Ex: `chmod u=rwx print.sh`

    2. To modify only r(Read)  W(write) permission of a file to user?

     `chmod u=rw file-name`

     Ex: `Chmod u=rw print.sh`

    3. To modify read(r) write(w) x(excute) permission ofa file to *group*?

    `chmod g=rwx file-name`

    Ex: `chmod g=rwx print.sh`

    4. To modify read(r) write(w) x(excute) permission ofa file to *Other*?

    `chmod o=rwx file-name`

    Ex: `chmod 0=rwx print.sh`

    5. To modify read(r) write(w) x(Excute) permission of a file to User, Group, Other?

    `chmod u=rwx,g=rwx,o=rwx file-name`

    Ex: `chmod u=rwx,g=rwx,o=rwx print.sh`


    6. To modify read,write, and Excute permission of a file to user, group, and Other using numeric values?

    `Chmod 777 file-name`

    Ex: `chmod 777 print.sh`


    7. To modify read permission of a file to user, group, and Other using numeric?

    `chmod 444 file-name`

    Ex: `chmod 444 print.sh`

    8. To modify (read, write) (read) (read) permission of a file to (user) (Group) (Other)?

    `chmod 644 file-name`

    Ex: `chmod 644 print.sh`

    9. To modify only read permission of a file to user and no permissions to group and others?

    `chmod 400 file-name`

    Ex: `chmod 400 print.sh`


    10. To chnage ownership of a file?

    `Chown newuser:new group file-name` -  Note: Ownership can be chnaged from root access only

    Ex: `chown aariz:aariz modify.sh`


To check the List of Process?

 `Ps`

 To check all the process running background?

 
 `ps aux` ---> **This will display with %CPU %Mem utilization**

 `ps -ef`---> **This will not display the %CPU %Mem utilization**

 To check the number of process of running?

`ps aux | nl`

 **The pipe symbol will execute the output of before command**

 To check the count of process running
 
 `ps aux | wc -l`

 Ex: it wil display only the number like "32"

 To check the a process using filter search?

 `ps aux  | grep search-name`

 Ex: ps aux | grep java ( This is command to fetch java process)

 To kill a process?

  `Kill PId`

 Ex: kill 28756

 
 To kill a process forcefully ?

  `kill -9 Pid`

To stop a running process?

  `kill -STOP PID` – Stop a running process

To Resume a stopeed process?

 `kill -CONT PID`

 To check all the service running?

 `systemctl list-units --type=service`

 ----->shows all type of service active,inactive and failed

 To stop a service?

 `systemctl stop service-name`

 To start a serive?

 `systemctl start service-name`

 To enable a service at startup

 `systemctl enable service-name`

##Monitoring Commands !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!

To check real time monitoring?
`top`

To check graphical real time monitoring
`htop`

To check memory usage?
`free -h or free -m`

To check disk space usage
`df -h`  or `du -sh *`



 

 
    




    


