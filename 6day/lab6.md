# locate
1. update the locate database.
2. find 'messages' file.
3. find all files with the name 'readme', using case ignoring option.

# find & nl
1. create two files named: 'TEST and test'.
2. Using find search for files 'test' with case-insensitive option and delete option.
3. Search for a directory named 'log', specifying path '/' and -ls option.
4. find all files bigger than 50 kilobyte in your /etc/ directory.
6. find files in /var/log/ directory less than 1 byte.
5. find all files in /etc directory and use -exec or xargs to check size with 'du -sh' on every single file.
6. find files owned by your user. (specify path /home/)
7. find files owned by your group. 
8. create a user with home directory then delete that user, but keep it's home directory, then serach for files by specifying -nouser option or -nogroup option.
9. find files with exact permission 777 and pipe the output to nl command to count the result.
10. find all executable files add -ls option in the end to see the results with detailed info.
11. find files recently modified, changed or accessed, using atime,amin,ctime,mmin,cmin.
12. find files that don't belong to the root user and bigger than 1 megabyte, use pipe and nl. 
13. find files in /usr/share bigger than 5 megabytes, using '-ok' option, copy them to home directory(to avoid messing up home directory, create a new folder and copy into it.
14. find all symbolic links in /usr/bin directory

# tar 
1. create several files, using tar archive them and compress with gzip compression method, do the same but with bzip2 and xz compression format.
2. using tar command, list the contents of your newly created archive file.
3. unarchive it again to /tmp directory using verbose option.
4. archive and compress /etc and /var directory to a new compressed archive file.
5. Remove files created earlier.


