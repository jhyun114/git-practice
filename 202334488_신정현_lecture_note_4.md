# < How to use the Shell command >
---
## -Basic command- 
### cd : change directory
If you want to get the file name of 'ABC', enter the 'cd ABC/'.
### ls : list files and directories
Can check files where they are.
### pwd : print working directory
Check current location of the files.
### cp
copy files and directories
### mv
move files and directories or rename them
### rm
delete files and directories permantely and irreversevely
But if you use the command 'rm' , you should be careful ! 
**If you use the 'rm', construct your command using 'ls' instead. By doing this, you can see the effect of your wildcards before you delete files. After you have tested your command with ls, recall the command with the up-arrow key and then substitute rm for ls in the command.**
### mkdir
make a new directory

---
## ls's various result
- ls : List the files in the working directory
- ls /bin : List the files in the /bin directory (or any other directory we care to specify)
- ls -l : List the files in the working directory in long format
- ls -l /etc /bin : List the files in the /bin directory and the /etc directory in long format
- ls -la .. : List all files (even ones with names beginning with a period charcter, which are normally hidden) in the parent of the working directory in long format
----
## cp's various result
- cp file1 file2 : Copies the contents of file1 into file2. If file2 doesn't exist, it is created; otherwise, file2 is silently overwritten with the contents of file1.
- xp -i file1 file2 : Like above however, since the "-i" (interactive) option is specified, if file2 exists, the user is promoted before it is overwriiten with the contents of file1.
- cp file1 dir1 : Copy the contents of file1 (into a file named file1) inside of directory dir1.
- cp -R dir1 dir2 : Copy the contents of the directory dir1. If directory dir2 doesn't exist, it is created. Otherwise, it creates a directory named dir1 within directory dir2.
----
## mv's various result
- mv file1 file2 : If file2 doesn't exist, then file1 is renamed file2. If file2 exists, its contents are silently relpaced with the contents of file1.
- mv -i file1 file2 : Like above however, since the "-i" (interactive) option is specified, if file2 exists, the user is prompted before it is overwriiten with the contents of file1.
- mv file1 file2 dir1 : The files file1 and file2 are moved to directory dir1. If dir1 doesn't exist, mv will exit with an error.
- mv dir1 dir2 : If dir2 doesn't exist, the dir1 is renamed dir2. If dir2 exists, the directory dir1 is moved within directory dir2.