# Bash Notes

## The Command Line

*The command line is a text-based interface used to interact with your computer's operating system. With a command line interface, you can issue specific commands to your computer by typing them in and pressing enter. These commands can range from simple file navigation to complex system configurations.

Git Bash is a command-line interface for Git that runs on Windows. It provides users with a Unix-like terminal environment where they can execute Git commands and use other Unix utilities.

To access a command line interface on Windows, you can use the Git Bash terminal that comes with Git. To get to it, you can follow these steps:

Install Git on your computer if it is not already installed. You can download it from the official website at https://git-scm.com/downloads.

Open the Git Bash terminal by searching for "Git Bash" in the Windows search bar or by running the "git-bash.exe" file located in the Git installation directory.

Once the Git Bash terminal is open, you can start using it to run Git commands and other Unix utilities.

## Basic Navigation

Basic navigation in Bash refers to the process of moving around the Linux directory system using command-line interface. In Linux, directories are organized in a tree-like structure, with the root directory ("/") at the top, and subdirectories branching out from there.

Here are some basic commands you can use to navigate the Linux directory system:

- pwd: This command prints the current working directory, which is the directory you are currently in.

- ls: This command lists the files and directories in the current directory.

- cd: This command is used to change directories. For example, to change to the "Documents" directory, you would type cd Documents.

- mkdir: This command is used to create a new directory. For example, to create a new directory called "NewDirectory", you would type mkdir NewDirectory.

- rmdir: This command is used to remove an empty directory. For example, to remove the directory "OldDirectory", you would type rmdir OldDirectory.

- rm: This command is used to remove a file. For example, to remove a file called "file.txt", you would type rm file.txt.

- cp: This command is used to copy a file or directory. For example, to copy a file called "file.txt" to a new location, you would type cp file.txt /path/to/new/location.

- mv: This command is used to move or rename a file or directory. For example, to rename a file called "oldfile.txt" to "newfile.txt", you would type mv oldfile.txt newfile.txt.



## More about Files

The first concept to understand is that everything in Linux is considered a file, including directories, keyboards, monitors, and text files. This idea helps with understanding Linux's behavior as we manage files and directories.

The second concept is that Linux is an extensionless system, meaning that the system ignores the file extension and looks inside the file to determine what type of file it is. This can sometimes make it difficult to know what type of file a particular file is, but the "file" command can be used to find out.

The third concept is that Linux is case sensitive, which means that files and directories with the same name but letters of different cases are considered distinct and separate files. It is also important to be aware of case sensitivity when dealing with command line options.

The fourth concept is spaces in names. Spaces in file and directory names are valid, but we need to be careful when using them on the command line. One approach is to use quotes around the entire item, while another method is to use an escape character (a backslash) to nullify the special meaning of the next character.

The fifth and final concept is hidden files and directories. If a file or directory's name begins with a . (full stop), then it is considered to be hidden. There is no need for a special command or action to make a file hidden.

## Manual Pages

Manual pages for BASH are a set of pages that explain every command and feature available in the BASH shell, including what they do, how to use them, and what command line arguments they accept. These pages provide detailed information on how to use BASH commands and are an essential resource for anyone using the Linux command line. The BASH manual pages can be accessed by using the `man` command followed by the name of the command or feature you want to look up. They are designed to be easy to navigate, with a consistent structure and clear explanations of each command's purpose and usage. By using the manual pages, users can quickly and easily learn how to use BASH commands and features to accomplish their tasks on the command line.

## File Manipulation

Creating a file: You can create a new file using the touch command. For example, touch myfile.txt will create an empty file called myfile.txt.

Copying a file: You can make a copy of a file using the cp command. For example, cp myfile.txt myfile_copy.txt will create a new file called myfile_copy.txt that is an exact copy of myfile.txt.

Moving a file: You can move a file from one directory to another using the mv command. For example, mv myfile.txt /home/user/documents will move myfile.txt to the documents directory under the user directory.

Renaming a file: You can rename a file using the mv command. For example, mv myfile.txt newfile.txt will rename myfile.txt to newfile.txt.

Deleting a file: You can delete a file using the rm command. For example, rm myfile.txt will delete myfile.txt.

Viewing the contents of a file: You can view the contents of a file using the cat command. For example, cat myfile.txt will display the contents of myfile.txt.

Editing a file: You can edit a file using a text editor such as nano or vim. For example, nano myfile.txt will open myfile.txt in the nano text editor.

Searching for text in a file: You can search for text in a file using the grep command. For example, grep "hello" myfile.txt will search for the word "hello" in myfile.txt.

Sorting the contents of a file: You can sort the contents of a file using the sort command. For example, sort myfile.txt will sort the lines in myfile.txt in alphabetical order.

Counting the number of lines, words, and characters in a file: You can count the number of lines, words, and characters in a file using the wc command. For example, wc myfile.txt will display the number of lines, words, and characters in myfile.txt.

## [Cheat Sheet](https://ryanstutorials.net/linuxtutorial/cheatsheet.php)

## [Back](../401readingNotes.md)