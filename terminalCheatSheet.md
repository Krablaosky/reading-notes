# Terminal Cheat Sheet

Command  | What it Does | Usage 
-------- | ------------ | ---------
dir      | Displays a list of a folder’s files and subfolders | dir (shows current folder) dir myfolder
cd/chdir    | Displays the name of the current directory or changes the current folder | cd filepath<br> chdir filepath<br> cd .. (goes one directory up)
md/mkdir | Creates a folder (directory) | md folder-name<br> mkdir folder-name
rm/rmdir | Deletes a folder (directory) | rm folder-name<br> rmdir folder-name<br> rm /s folder-name<br> rmdir /s folder-name<br> Note: if the folder isn’t empty, you must add the /s.
copy | Copies a file from one location to another | copy filepath-from filepath-to
move | Moves file from one folder to another | move folder1\file.txt folder2\
ren/rename | Changes the name of a file | ren file1 file2
del | Deletes one or more files | del filename
exit | Exits batch script or current command control | exit
echo | Used to display a message or to turn off/on messages in batch scrip | echo message
type | Displays contents of a text file | type myfile.txt
fc | Compares two files and displays the difference between them | fc file1 file2
file | used to find a specific file | file [nick.png]
cls/clear | Clears the screen | cls
ls | Makes a location list | ls [options], [location]
ls -l | Makes a location list with detailed information | ls -l
pwd | Tells you your location | pwd C:\Windows\System32
touch | Creates a new file | touch newfile.md
~(Tilde) | shortcut for your home directory | ~/Documents
.(dot) | reference to your current directory | ./Documents
..(dotdot) | reference to the parent directory | ../../ and this would do a listing of the root directory.
help | Provides more details about DOS/Command Prompt commands | help (lists all commands), help command
