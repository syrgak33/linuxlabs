# Useradd & groupadd & usermod
1. Login as root using either sudo or su. 
2. Create a user named azure, with a home directory,with a comment and with a shell '/bin/sh'.
Check the result in /etc/passwd. Check the password hash in /etc/shadow
3. Add password to your user. You can see the hash of your password in /etc/shadow file.
4. Using usermod change the shell of the user azure to '/bin/bash'. 
5. Add a new group named testing with groupID 315.
6. Add your created user to the testing group and the sudoers group(in CentOS its called wheel, in ubuntu sudo)
7. Login to your azure user and temporarily have the testing group as primary group, create a file in the azure's home directory and see to which group does it belong.
8. Delete the azure user, but keep the home directory.
9. Copy the /etc/services file to the /etc/skel directory and create a new user with homedir,list the home directory of that user. After completing delete that user and homedir of it.
10. See the any user's account aging info. 
11. As a root user LOCK one of your users and try to ssh to that user or login from terminal. Unlock it then.
12. As a root user change the expiration date of one of the users password to 180 day. (use man)
13. Using chage command change the password options of a user, so that he will be forced to change a password on the next login. Try to ssh with that user from a different ssh-session or login from Vbox terminal directly.
14. Set the maximum expiration date for a password = 5 days. 

# chmod & chown. 
1. Recursively change the ownership of deleted user's home directory to a root user and root group. 
2. Create a small script that contains 2 lines.
  #!/bin/bash
  echo 'it works'
give permission 600 and try to run it with './' like = ./scriptname. Add execute permissions and run again.
3. Currently if you don't have ssh-keys in your Vmachine, create them and long list the .ssh directory and it's contents, to see the permissions. REMEMBER: changing default permissions of ssh-key files or folder, will bring errors while using key-based connection.
4. In you home directory as a normal user(not root) create a folder and file in it, change permissions of the folder to 000 and go to directory above,then do these steps.
    a. Try to list created folder. Give read permissions to the created folder and list it again.
    b. Try to create a file in a folder. Give write and execute permissions to the created folder and try to create again.
5. create a file that can be read&write by the user, read by the group, and no permission to others.

