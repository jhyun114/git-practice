# How to use 
## I/O Redirection
#### Standard Output
***Standard output is screen.***
If you make a new file, you can redirect output using “>” after a command to create and save the output in a file.
 If you use this, you have to use ls -lh ">" (Don't use "<" in this situation).
 
If it's a file that already exists, you have to use ">>".

---
#### Standard Input
***Standard input is from keyboard.***
You can redirecct input from a file using “<”.
You can mix “<“ and “>” together in a single line.

If you receive the contents in the file as input and sort it, the input words will output the classified results, which will not be output but will be saved as a file with another name.

---
#### Pipelines "|"
Pipeline feeds output of previous command to input of next command.
ex) command1 | command2 | command3 |...
command 1's output --> command 2's input, command 2's output --> command 3's input

> **ls -lh | less**
> You can check the contents while scrolling directly, and (END) is displayed in the last line.

> **ls | wc -l**
Indicates the number of files currently in the directory. The more files there are, the more effective and useful it is.

---

#### Expansion
Special characters expand its meaning when given to shell commands. 

**echo**
Echo print out the text that follows it.

**echo ~**
Expand the current user's home directory.

#### Backslash ( \ )
Backslah can be used to ignore line change in command (“enter”), to enter a long command in multiple lines.

---
#### Permissions
Linux is a multi-user system.
Files and directories have a permission assigned differently to owner / group / others.
(rwx : read, write, execute)
###### how to use?
$ chmod 000 ABC
(000 : Three-digit numbers representing permissions)
(ABC : Name of the file or directory to which you want to change permissions)

* ex 1) 777 : No restrictions on permissions. Anybody may do anything. Generally not a desirable setting.
* ex 2) 755 : The file's owner may read, write, and execute the file. All others may read and execute the file. This settinf is common for programs that are used by all users.

---
#### Superuser
A superuser has all system administation authority.
Some commands need superuser’s privilleges.
Put “sudo” before the command if you are a superuser. ( Use "sudo" only when you need it. )

---
#### Text editor
* vi, vim : It's a bit difficult to use at first, but once you get used to it, you can use it much faster than other editors.
* nano : It's good for beginners to use. It is a free clone of the text editor supplied with the pine email program. 

---
#### Shell Script
The advantage is that you can use it comfortably if you run the script at any time you want to make the changes.
