# Systemd & systemctl 
1. List all systemd related manuals in cli using apropos, skim through the list, you might need them for configuring systemd in the future.
2. Perform these steps using systemctl:
    a. ssh into one of your machines from git-bash or cmd.
    b. Check the status of sshd service. 
    c. Stop it and check status again. 
    d. Exit from current shell and ssh again. If you couldn't ssh, connect from vbox terminal(tty) and start sshd.service.
    e. Check if sshd enabled by default.
    f. Using systemctl list unit files, using 'type' option output only services, look at cron.service from that list, stop cron service,then mask it, try to start it. undo previous steps to make it work again.
    g. What is the difference between systemctl reload and systemctl restart commands?

3. Research about what systemd-analyze command can do, find the subcommand, that helps with troubleshooting boot-up time.

# timedatectl 
 
