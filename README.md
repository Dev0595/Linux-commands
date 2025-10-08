# Linux-commands
1.	To create a new User?

  	 Sudo adduser username
  	
     Ex: Sudo adduser "aariz"
  	
2. 	To change user password?

     Sudo passwd username

     Ex: Sudo passwd aariz
   	
3.	To change username?

    Sudo usermod -l newname oldname

   Ex: Sudo usermod -l aariz1 aariz
   
4. 	To delete an existing user?

  Sudo userdel username

  Ex: Sudo userdel aariz
  
5. 	To lock a useraccount?

  Sudo passwd -l username

  Ex: Sudo passwd -l aariz
  
6. 	To unlock a user account?	

  Sudo passwd -u username

  Ex: Sudo passwd -u aariz

7. To create a directory

   mkdir diretory_name

   Ex: mkdir devops

8. To create a file

   touch file_name

   Ex: touch file1.txt

9. To copy a file from one home directory to another directory?

   cp /home/source-dir/filename /home/target-dir/

   Ex: cp /home/aariz/file.txt /home/linuxdev/

10. To move a file

   Mv /home/source-dir/filename /home/target-dir/
   Ex: mv /home/aariz/file2.txt /home/linuxdev/

11. To view a file

    cat file_name
    Ex: Cat file.txt

12. To display first few lines of text in a file?

    cat head -n file-name
    Ex: cat head -n 5 file.txt
    "This will display the first five lines in the textfile without counting spaces

    Ex: cat head -5 file.txt
    "This will display the first five lines of the text including spaces.

13. 


