# CentOS firewall = firewalld.service. Command = firewall-cmd.
1. Using firewall-cmd command change the default zone from 'public' to 'block' or to 'drop', exit and try to ssh again. From vbox terminal switch to public zone again. You can learn more about zones from the 'man firewalld.zones'
2. List your default zone's allowed services or ports. 
3. Allow two ports (80 and 443), make changes permanent, so after reboot rules will persist. Then type second command to reload firewall rules, after this command you can list opened ports.
4. Allow service ftp and http, make changes permanent.  

# Cron
1. Schedule a backup of all user /home directories at 5am Daily, using tar command.
2. Now reschedule previous cron to 5AM per week.
3. Schedule Cron to execute a command twice a day. 
4. Schedule Cron to execute a job at 3AM daily. Using command apt-get -y update && apt-get -y upgrade.
5. Schedule Cron to Execute a Job at 8PM every week. Using command sudo yum upgrade -y 
6. Backup all cron jobs to plain text file.
7. Restore cron jobs from backup file.
8. If you use CentOS schedule cron to clean all cached files using yum command once in a week.
9. If it is an Ubuntu machine cron to clean unused dependency packages using apt-get autoremove -y. Schedule it weekly.
6. In the end you can remove created crontabs.
