## Basic linux commands


### Listing commands
```ls option_flag arguments ```--> list the sub directories and files avaiable in the present directory

Examples:

- ``` ls -l ```--> Lists files and directories in a detailed, long format.
        Ex:$ ls -l
            total 20
            drwxr-xr-x  2 user user 4096 Oct  7 12:30 Documents
            -rw-r--r--  1 user user  123 Oct  7 12:00 file.txt
            -rwxr-xr-x  1 user user  234 Oct  7 11:45 script.sh

- ```ls -a ```--> list all including hidden files and directory
        Ex:$ ls -a
            .  ..  .bashrc  .gitignore  Documents  file.txt

- ```ls *.sh``` --> list all the files having .sh extension.
        Ex:$ ls *.sh
            script1.sh  deploy.sh  backup.sh


- ```ls -i ``` --> list the files and directories with index numbers inodes
        Ex:$ ls -i
            12890123 file.txt  12890124 Documents  12890125 script.sh

- ``` ls -d */``` --> list only directories.(we can also specify a pattern)
        Ex:$ ls -d */
            Documents/  Downloads/  Projects/

### Directoy commands
- ```pwd``` --> print work directory. Gives the present working directory.
        Ex:$ pwd
            /home/user/Documents/Projects

- ```cd path_to_directory``` --> change directory to the provided path
        Ex:$ cd /home/user/Documents
            $ pwd
            /home/user/Documents

- ```cd ~ ``` or just  ```cd ``` --> change directory to the home directory
        Ex:$ cd ~
            $ pwd
            /home/user

- ``` cd - ``` --> Go to the last working directory.
        Ex:$ cd /home/user/Documents
            $ cd /etc
            $ cd -
            /home/user/Documents

- ``` cd ..``` --> change directory to one step back.
        Ex:$ pwd
            /home/user/Documents/Projects
            $ cd ..
            $ pwd
            /home/user/Documents


- ``` cd ../..``` --> Change directory to 2 levels back.
        Ex:$ pwd
            /home/user/Documents/Projects/Code
            $ cd ../..
            $ pwd
            /home/user

- ``` mkdir  directoryName``` --> to make a directory in a specific location

Examples:
```
mkdir newFolder              # make a new folder 'newFolder'

mkdir .NewFolder              # make a hidden directory (also . before a file to make it hidden)

mkdir A B C D                  #make multiple directories at the same time

mkdir /home/user/Mydirectory   # make a new folder in a specific location

mkdir -p  A/B/C/D              # make a nested directory
```
