# IP configuring.
1. set static ip and change your Virtual machine network options to bridged.(netplan if it's an ubuntu,nmcli or nmtui if centOS)
2. try to ping to a random site. (google.com), to check connectivity.

# Working from different terminal emulator using ssh.
1. Try to ssh into your virtual machine from git-bash after installing it.
2. create ssh-keys using ed25519 type keys, then connect to your linux terminal from windows git-bash,using keys.(commands to use ssh-keygen,ssh-copy-id).
3. From Windows git-bash create ssh-config file in ~/.ssh/ folder and write your ssh configurations to ease the access to your servers.
4. After configuring your ssh connection try to send a file from windows to your Vmachine using scp.
5. Download a file from Vmachine to your windows using scp.
6. Disable password authentication in /etc/ssh/sshd_config file.
7. ssh to your servers using private key.

#  stdin + stdout + stderr. To test it use commands like cat or ls.
1. How to hide error outputs after command execution? 
2. How to redirect both errors and valid output to a file? 
3. Send error outputs only, to a file.
4. What are exit codes? And how to see the previous command's exit code in terminal?

# alias
1. create alias for the command ls with the options you like.
2. list all existing aliases. 
3. create an alias to display your OS details. (/etc/os-release)
4. how to remove alias?

# head & tail
1. Using head & tail display only the 15th line of /etc/passwd file.
2. Display the 5 first lines of the command 'ps aux'
3. Using head options display all lines of /etc/passwd, except the last 10. 
4. Using tail options display all lines of /etc/passwd, except the first 10.


