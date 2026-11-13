# My Linux Cheatsheet

- pwd: shows where I am right now
- ls: shows the files in this folder
- cd: to enter
- mkdir: to make a folder
- touch: makes an empty file
- echo: it puts text into a file
- cat: shows what is inside a file
- cp: it makes a second file with the same content
- mv: it gives a file a new name
- rm: it deletes a file forever
- r:mean thet u have permission read
- w:mean thet u have permission to write
- x:mean ther u have permission to execute
- ls  -l: it gives u to the permissions of the files (like -rw-r--r--)
- chmod u+x:file means: give the owner permission to run the file
- In Git Bash on Windows, chmod often does not change the permissions you see with ls -l. That is because Windows stores permissions in a different way than Linux

## grep & piping
- grep:is used to find a pattern or a word in the file
- | (pipe):u put output of the first command it becomes the input for the second command
- grep -i:means ignoring upper/lowercase like APPLE,apple,apple pie
- grep -n:shows the number of each matching line
- grep -v:means inverting the search so u will see different output like banana and cherry
- grep -c:counts how many lines match
- My mistake today:i put ls on one line, and grep thought ls was a file name.

## Finding files
- find WHERE -name "WHAT": WHERE is the folder to search in, WHAT is the file name or pattern to look for
- find ~/day7 -name "notes.txt":with this command u can find a file by name.
- find ~/day7 -name "*.txt":with this command u can find .txt file.
- find ~/day7 -type d: with this command u can only find the folders.
- locate notes.txt:looks in that list and it is very fast.
- with updatedb this command the list get refreshed if the list is too old a new file won't show up.
- whatis locate:the command show one line "command not found" because Git Bash is not a full Linux system.
- my mistakes today: so my first is extra dot after the closing quote.
- and my second mistake is typing space between docs/ report.txt.
- and third mistake typing -name -type d together.
-and my fourth mistake Forgetting -name before "*.txt"

## System & kernel information
-uname -a: this command givs as all informasion so we get evrything in singol line.
-uname -r: this command givs u yuor kernel vrsion.
-uname -s: this command givs u a system name in this case i have MINGW64_NT-10.0-26200.because i use git bash on windows on linux it should be diffrent.
-uname -m: this command show u your computer bits
-cat /etc/os-release: on git bash this command didn't work it shows “No such file or directory” because git bash is not a real linux Git Bash runs on Windows and there is no distribution on real linux it will show u distribution (Ubuntu, Kali, Debian...).
-mistakes today: my first mistake is thet i write uname wrong so i write unmae.
-my second is thet i put sepce between cd day 8.

 ## Bandit Levels 0-2
 -cat ./-: this is used to open a file name dash.
 -Backslash \: this is used to keep space inside a file.
 -my mistake: I typed cat ./-- and it didn't work
 
## Bandit Level 3 - Hidden files
-A hidden file is a file thet starts whit a dot (.) and normal ls dose not show it.
-ls -a show it becouse it means all
-mistakes today: cat inhere so i was already inside the folder but i typed second time and it showed no such file or directory. 

## Bandit Level 4 - Finding the readable file
-file ./* this command is used to find the right file becouse ther will some junk files.
* this means all so if want to see all the files u use this *
-mistake today: I typed done in the terminal, but the terminal only understands commands.


