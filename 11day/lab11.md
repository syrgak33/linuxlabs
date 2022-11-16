# CentOS firewall = firewalld.service. Command = firewall-cmd.
1. Using firewall-cmd command change the default zone from 'public' to 'block' or to 'drop', exit and try to ssh again. From vbox terminal switch to public zone again. You can learn more about zones from the 'man firewalld.zones'
2. List your default zone's allowed services or ports. 
3. Allow two ports (80 and 443), make changes permanent, so after reboot rules will persist. Then type second command to reload firewall rules, after this command you can list opened ports.
4. Allow service 
