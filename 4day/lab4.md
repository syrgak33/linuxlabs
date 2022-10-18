# dnf, yum, rpm. (enter Centos machine)
1. List installed packages on your Centos system.
2. list available packages and numerate the output with nl command.
3. Install epel-release package for extra repositories, then update.
4. Upgrade your system's packages. Use assumeyes option.
5. Search for package 'translate-shell' and install it.
6. Find package that provides mkfs command.
7. List available dnf groups.
8. checkout your dnf history, install 'nano' or 'tree' and undo this action using 'dnf history' command.
9. list and download(not install) package from dnf repository.
10. After downloading query information from that package: 
    a. Where config files located.
    b. Detailed information about a package.
    c. Does it contain any scripts in it?
    d. list package contents.
11. Using rpm command query /etc/ssh/sshd_config file to find out which package it came from.
12. Using dnf provides find out where /etc/ssh/sshd_config file came from, add some comments to this file
using # sign, and verify the integrity of that package that you found. Look up man pages of rpm to understand the meaning of output.
> Note: In case of corruption of a package or if its missing some components, dnf reinstall might help.

# apt, apt-get

1. Firstly, update and upgrade the packages.
2. Search for package named as 'ansible-doc'
3. Using apt see the description of 'ansible-doc' package.
4. Using apt list the dependencies of the 'ansible' package.
5. Install nginx, add any comment(using # sign) in the end of the /etc/nginx/nginx.conf file, 
then remove it, check if /etc/nginx/ directory contains any files, if yes, then purge them using apt purge.
6. Add repository named ppa:ansible/ansible to your repo list, then update your apt package info,but do not upgrade, then remove added repository from the /etc/sources.list.d/ directory.

# dpkg
1. Using apt-get command download the 'tree' package.
2. using dpkg command query the contents of the downloaded .deb package.
3. using dpkg query info about that package.

# Process mgmt. 
1. Run 'ls -laR /' command and stop it. 
2. Run vim in the background and list the jobs, bring to the foreground and quit. Make sure job is no longer exist.
3. run 'vim' in the background, open top, find vim process and kill it.
4. Run top and locate the 'bash' command using hotkey.
5. Run top and sort: reversely, by username, CPU usage, Memory usage.
6. run the command 'watch date', find the process in Top and renice it to 15.
7. Use ps command with the current format: ni,pid,comm,user.
8. Use ps command to display parent/child format.
9. Use ps command and sort according to user.
10. Using who command determine the time when you logged in and how long your session exists.
11. Using free command determine how much your swap is used and how your total memory.(use option to see in MB)




