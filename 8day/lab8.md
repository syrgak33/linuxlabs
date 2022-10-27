# Environment variables & aliases.
1. Create a directory /opt/bin/ as root, and export this directory to the end of your PATH variable,(caution! - if you make a mistake while changing default PATH variable, you will break your shell.)
2. Currently your history command doesn't show commands execution time, add HISTTIMEFORMAT variable to your .bashrc source it and run history. 
3. Create environment variable COLOR=RED in /etc/profile.d/customvars file. Source it and  check with echo. Open new bash shell(just type 'bash') and try to echo $COLOR again. Do the same steps but with command: export COLOR=RED in that file. 
4. Research about common env variables: SHLVL,RANDOM,SECONDS,HOME,USER,PPID,PS1,SHELL.
5. For extra security, try adding TMOUT variable, if you like it, add to your .bashrc to make it permanent.
6. Check if the command 'cdf' exist by typing, then create short alias for 'cd .. ; pwd' command and add to your .bashrc file. Now you can go directory up with cdf command. 
7. extra: Change your PS1 variable and see the output, examples: PS1='\t[\u@\h]$ '.

# Metacharacters && || ;
1. What will be the output of the commands below.
  a. cat 389473974 && echo 'will echo show the output?' 
  b. ls ~ && echo 'True && True'
  b. cat 384739473 || echo 'why do echo works now?'
  c. ls ~ || echo 'No errors || echo won't Run'
  d. ls ~ ; echo 'always works' ; date

# Metacharacters * ? []
1. Using ls and [] list the files or folders in /etc/ directory that starts with letters a,s,m.
2. Using ls -ld list files and dirs in /etc/  containing only 5 characters.
3. list all .conf files in /etc/ directory.

# Metacharacters < <<
1. what is the difference between these two commands? 
    a. cat /etc/group
    b. cat < /etc/group
2. Write a small text using 'cat', '<<' and '>'  symbols.  

# Metacharacters $() ()
1. Using echo,date and $() characters, write the text below, substitute the words (Thursday,5,December,2022) with date command options.
   a. Today is Thursday, 5th of December, year 2022.
2. using <() and paste command combine columns of two command's output.

 

