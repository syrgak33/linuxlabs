# Deploying FTP server.
1. Upgrade packages on your system. (if it is an Ubuntu update first , then upgrade)
2. Install vsftpd package.
3. Allow service ftp using firewall commands, then reload it ( if it is firewalld)
4. Allow anonymous access to your ftp server. 
5. Restart your vsftpd service.
6. Put text file with some data in it, into /var/ftp (centOS) or into /srv/ftp (ubuntu) directories.
7. Try to connect to your ftp server from Windows web browser. Type in browser ftp://ipaddress
8. From terminal connect to ftp server using ftp command(user: anonymous, no password), and download created file using ftp commands.(use help)
9. Create a user with a password, in home directory create a text file, from Windows try to connect to that user using sftp command, and download that file to your windows.
10. Try to disable newly created user using ftp configuration files.
11. Download into your android phone, 'WiFi FTP server' application from playstore, and using your virtual machine try to connect to your phone and download any picture to your vmachine. 
12. From your phone's web browser(not chrome) you can also access to your virtual machine's ftp server.

# Swap file
1. Check the swap space using free command. 
2. using dd command create a swap file in /var/tmp/swapfile with size 1GB.
3. using mkswap command use created file as a extra swap area.
4. turn on swap using swapon command.
5. Chek swap space again. 

# Swap partition.
1. Create a partition with swap type(hex code).
2. Use your partition as a swap. Using previous commands.

# lsattr & chattr. 
1. As a root using chattr command add options append to the file. Use man chattr.
2. If you use ext4 or xfs filesystem check which chattr options is supported on filesystem.
3. Add immutable attribute to a file. 
4. list added attributes of a file using lsattr command.
5. To avoid extra amount of disk I/O try to disable atime record on a file.
