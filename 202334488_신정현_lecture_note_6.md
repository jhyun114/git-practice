## Version control
Making copies another name
1. Change
Over the time, record the version.
version1 -> version2 -> version3 -> ... 
Some version has changing file.
2. Snapshot
------
### Local
If I want to share the file, you have to copy local file and send it.
### Centralized
It records multiple versions and sends information centrally when needed by the local computer.
In other words, each local computer gets what it needs from the central computer.
### Distributed
Each local computer has a full copy of information from the central computer (central server). Therefore, when the central server is in trouble, it can be recovered with a copy on the local computer. **(The git adopts a distributed method.)**

--------
### STATE
* Working directory (Modified)
* Staging area (Staged)
* Git directory (Comitted)

### git config
$ git config -- global user.name
$ git config -- global user.email
$ git config -- global init
$ git config -- list
$ git config -- user.name

### git init
implement --> Initialized empty Git repository in /home/user.name/OSS/transformers/.git/

### git add [file_name]
The git adopts a distributed method.
If there is anything you want to change after doing file stacking area, upload it to the staging area once again.

### gitignore
From the git's point of view, the code in this is treated without it at all.

### git commit
'-m' option is recommended.
### git branch
Enter the branch you want to change and add '-m'.