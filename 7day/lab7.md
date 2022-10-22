# cut | sort | uniq | grep | awk | seq
1. cut the fifth field and third field of the /etc/password file.
2. cut the first 5 bytes from /etc/passwd
3. display all fields from /etc/passwd except the second field and sort alphabetically.
4. cut the 3rd field from /etc/group and sort numbers in reverse order.
5. grep all the usernames in /etc/passwd with the /bin/bash shell.
6. run 'ps -ef' command and using awk cut 2nd(PID) field and sort these numbers.
7. using awk display the 2nd field, and then awk again to leave only protocol types field(tcp,udp..), use sort and uniq to count the protocol types number of occurence.
8. run the seq command 'seq 1 100' and grep lines that starts with '5'.
9. run this command: echo {a..z} | sed 's/ /\n/g' , then try to display only vowels using grep.
10. using last command grep only the last column (numbers in parenthesis).
11. grep all files containing the word 'root' in /var/log directory. (use grep options)
12. grep all lines that starts with letters s,m and ends with the letter n in /etc/passwd.
13. echo the line 'Symbol of gold is Au', then using sed replace gold with silver and Au with Ag.
14. echo '192.168.0.20/24' then remove /24 using sed.
15. Open site: https://www.cs.ubbcluj.ro/~rares/course/os/res/practice/gsa/index.html ,
using wget download passwd.fake,ps.fake,last.fake files or just copy them to your Vmachine using vim.
To wget, open one of the files in your browser and copy link, then type in your vmachine:
 wget https://www.cs.ubbcluj.ro/~rares/course/os/res/practice/gsa/passwd.fake 
Try to solve these tasks using downloaded files.

