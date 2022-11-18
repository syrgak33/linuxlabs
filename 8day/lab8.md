# Environment variables & aliases.
1. Echo $PATH variable to list it's directories. Create a directory /opt/bin/ as root, and using export command add this directory to the beginning of your PATH variable,(caution! - if you make a mistake while changing default PATH variable, you will break your shell.)  
2. Currently your history command doesn't show commands execution time, add HISTTIMEFORMAT variable to your .bashrc source it(using source command) , check result running history. (Google HISTTIMEFORMAT examples) 
3. Echo env variable named $HISTFILESIZE(number of lines history can save) and try to increase or decrease globally in /etc/profile.d/customvars file. Source it and  check with echo.
4. For extra security, try adding TMOUT variable(auto-logout) specify in seconds, add to your .bashrc to make it permanent.
6. Check if the command 'cdf' exist by typing it(to avoid overwriting existing command), then create short alias for 'cd .. ; pwd' command and add to your .bashrc file. Now you can go directory up with cdf command. 
7. extra: Change your PS1 variable and see the output, examples: PS1='\t[\u@\h]$ '.

# Metacharacters && || ;
1. Try these commands.  To understand conditional expressions use, man bash
and search line named 'CONDITIONAL EXPRESSIONS'.  
  a. [ ! -d test ] && mkdir test  
  b. [ -d test2 ] || mkdir test2
  c. vim script.sh && chmod +x script.sh
  d. [ -f newfile ] || touch file

# Metacharacters * ? []
1. Using ls and [] list the files or folders in /etc/ directory that starts with letters a,s,m.
2. Using ls -ld list files and dirs in /etc/  containing only 5 characters.

# Metacharacters < <<
1. what is the difference between these two commands? Try to google it. 
    a. cat /etc/group
    b. cat < /etc/group

# Metacharacters $() ()
1. Using echo "", $(date +%options), write the text below, substitute the words (Thursday,5,December,2022) with date command options. Use date --help.
   a. Today is Thursday, 5th of December, year 2022.

# SUID GUID sticky bits.
1. find all files in /usr/bin directory with SUID permissions enabled. 
2. find all files in /usr/bin directory with GID permissions enabled. See the groups they belong.
3. what is the difference between simple execution and execution with SUID permissions?



