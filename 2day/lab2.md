# Vim Basics

. go into insert mode and type a sentence.
1. Command mode commands.
. go into command mode and type one of this hotkeys.
  . use hotkey 'A' to move cursor to the end of the line and write.
  . use hotkey 'I' to move cursor to the beginning of the line and write.
  . use 'o' to move cursor and write below your current sentence.
  . use 'O' to move cursor and write above your current sentence.

2. save current result, but do not quit using 'w'
3. wq or x = save and quit

4. Navigate in vim (command mode)
. L = move cursor to the end of text. or use 'Shift+g' 
. H = move cursor to the beginning of text. or use 'gg' command
. M = move cursor to the mid of text.
. $ = move cursor to the end of line.
. 0 = move cursor to the beginning of line.
. w = jump to the next word. 
. b = jump to previous word.
. replacing cursor keys with  =  h,j,k,l.

5.  to delete.
dd = deletes a whole line.
dw = deletes a word.
db = deletes a word before cursor.

6. to number the lines and change theme. (it wont write to the file,only display)
:set number
:colorscheme + type 'Tab' to list colorschemes.

7.  to search a string in a vim in command mode.
/ = search a string below cursor.
? = search a string above cursor.

8. Undo & redo 
Ctrl+R = Redo 
u      = Undo 

9. cp file /etc/services to your directory and using vim replace all 'tcp' words with the word 'null'.
:g/oldword/s//Newword/g = substitutes the 'oldword' with a new one in the entire file.
:g/oldword/s//newword/  = substitutes the 'oldword' with a new one on every line of the file.

10. Using visual mode in vim copy-paste text,and cut-paste text.
In command mode, type 'v' to enter visual mode and select text after selecting.
y = to copy
x = to cut
p = paste

# less & more

1. Use less command to read the file /etc/protocols file.
2. research which one is better to use 'more' or 'less' command?
3. Jump to the end of file using 'gg' and 'G' hotkey.
4. Search specific string using '/' and '?' in a file. Jump to prev and next found string using 'n or N'

# mv and cp commands

1. create a folder named 'moveit' in home directory and move to /tmp directory.
2. create a file in home dir. and copy to /tmp directory.
3. copy or move several files at once.

# creating hard links and soft links.

1. create a file in a home directory, write something in it,then create hard link of that file in a /tmp folder,
delete the file in home directory and see what will happen to the one in /tmp folder.
2. do the same above, but with symbolic link, then try to read symbolic link.

# tar
1. create a folder that contains three files, and archive it using tar command. 
2. repeat the action above,but with gzip compression and verbose option. (use --help)
3. list the contents of the tar file.
4. extract your compressed archive to /tmp folder.

# basic path structure.
1. what is the difference between '/' and '/root' directory?
2. by default user folders located in which directory?
3. difference between absolute and relative path?

# Using history.
1. List your previous commands and recall one of it.
2. Do the same as above but with using fc command.
3. clear your history.


