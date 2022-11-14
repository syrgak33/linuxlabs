# Systemd & systemctl 
1. List all systemd related manuals in cli using apropos, skim through the list, you might need them for configuring systemd in the future.
2. Perform these steps using systemctl:
    a. ssh into one of your machines from git-bash or cmd.
    b. Check the status of sshd service. 
    c. Stop it and check status again. 
    d. Exit from current shell and ssh again. If you couldn't ssh, connect from vbox terminal(tty1) and start sshd.service.
    e. Check if sshd enabled by default.
    f. Using systemctl list unit files, using 'type' option output only services, look at cron.service from that list, stop cron service,then mask it, try to start it. undo previous steps to make it work again.
    g. What is the difference between systemctl reload and systemctl restart commands?

3. Research about what systemd-analyze command can do, find the subcommand, that helps with troubleshooting boot-up time.

# timedatectl 
1. On your servers, check the status of current time using timedatectl.
2. List available timezones.
3. Set the timezone of our location.
4. Enable ntp synchronization if disabled. true/false
5. if it is Ubuntu, check ntp servers info with the command: timedatectl timesync-status
6. if it is CentOS, check ntp servers info with the command: chronyc sources.
7. On Ubuntu, service name of ntp is systemd-timesyncd.service, check status with systemctl.
8. Check the status of ntp service on CentOS, what service it might be?

# service command (for an older Operating systems using initV, but still usable in systemd OS)
1. try to display status of sshd with 'service' command. (it can also start, restart,stop) 
2. Using top, or 'ps -p 1' you can determine which init process you have, systemd or initV.
