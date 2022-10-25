# Vim Basics

. go into INSERT mode and write a sentence.
1. Command mode commands.
. go into command mode by pressing ESC and type one of this hotkeys.
  . A  =  move cursor to the end of the line and start writing.
  . I  =  move cursor to the beginning of the line and start writing.
  . o  =  move cursor and write below your current sentence.
  . O  =  move cursor and write above your current sentence.

2. save current result using :w, but stays in vim. (command mode)

3. :wq or :x = save and quit  (command mode)

4. Navigate in vim (command mode)
. L = move cursor to the end of text. or use 'Shift+g' 
. H = move cursor to the beginning of text. or use 'gg' command
. M = move cursor to the mid of text.
. $ = move cursor to the end of line.
. 0 = move cursor to the beginning of line.
. w = jump to the next word. 
. b = jump to previous word.
. replacing cursor keys with  =  h,j,k,l.

5. Delete lines in command mode.
dd = deletes a whole line.
dw = deletes a word after cursor.
db = deletes a word before cursor.

6. to number the lines type in command mode. (it won't affect the file)
:set number

7. in command mode, change colors of Vim.
:colorscheme + type 'Tab' to list colorschemes.

7. To search a string in a vim in command mode type:
/ = search forward.
? = search backward.

8. Undo & redo in command mode press. 
Ctrl+R = Redo 
u      = Undo 

9. cp file /etc/services to your directory and using vim replace all 'tcp' words with the word 'null'.
:g/oldword/s//Newword/g = substitutes the 'oldword' with a new one in the entire file.
:g/oldword/s//newword/  = substitutes the 'oldword' with a new one once on every line of the file.

10. Using visual mode in vim copy-paste text,and cut-paste text.
In command mode, type 'v' to enter visual mode and select text after selecting.
y = to copy
x = to cut
p = paste

# less 

1. Use less command to read the file /etc/protocols file.
2. Jump to the end of file using 'gg' and 'G' hotkey.
4. Search specific string using '/' and '?' in a file. Jump to prev and next found string using 'n or N'
 
# mv and cp commands

1. create a folder named 'moveit' in your home directory and move to /tmp directory.
2. create a file in home dir. and copy to /tmp directory.
3. copy or move several files at once.
4. rename one of your created files.
5. create a file in ~, then copy to /tmp, then move your created file from ~ directory to /tmp again, but with backup option.
6. create a folder with several files, then copy created folder to /tmp, recursively.

# hard links & soft links & stat.

1. create a file in your home directory, echo something in it,then make hard link of that file in a /tmp folder,
delete the file in home directory and see what will happen to the one in /tmp folder.
2. do the same above, but with symbolic link, then try to open symbolic link.
3. using stat command check the file attributes.

# basic path structure.
1. what is the difference between '/' and '/root' directory?
2. By default user folders located in which directory?
3. difference between absolute and relative path?

# Using history.
1. List your previous commands and recall one of it.
2. Do the same as above but with using fc command.
3. clear your history.
4. (echo $HISTFILE) variable to see the location of your history file.

