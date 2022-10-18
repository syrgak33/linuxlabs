# Useradd & groupadd & usermod
1. Login as root using either sudo or su. 
2. Add a local user to your system named azure, with home directory, with comment and with shell '/bin/sh'.
Check the result in /etc/passwd. Check the password hash in /etc/shadow
3. Add password to your user. You can see the hash of your password in /etc/shadow file.
4. Add a new group named testing with groupID 315.
5. Add your created user to the testing group and the sudoers group(in CentOS its called wheel, in ubuntu sudo)
6. Login to your azure user and temporarily have the testing group as primary group, create a file in the azure's home directory and see to which group does it belong.
7. Delete the azure user, but keep the home directory.
8. Copy the /etc/services file to the /etc/skel directory and create a new user with homedir,list the home directory of that user. After completing delete that user and homedir of it.

# chmod & chown. 
1. change the permission of /home/azure directory so that it can only be read by azure user.  
