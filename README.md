# Thesis
Altering Linux Bash commands as a defensive measure against attackers
These files here are files that are related to the thesis topic.
The folder bash-master contains modified cd.def file which makes the cd command with comments indicating the changed parts of the code. The changed parts have comments near them that mention thesis so they can be found using "ctrl f" and searching for thesis.
The contents of the bash-master folder can be made into a bash and bashbug file using the make command. Refer to the instructions in Install folder for more details.
The outpupted bash and bashbug files should be copied to /bin after renaming /bin/bash to something else.
The other included files outside of Thesis folder are bashrc file, of which contents can be copied and pasted into ~/.bashrc file overwriting the original code. Other than that there is also the fake_pwd file and the fake chmod file which need to be placed in /bin and given permission to execute after renaming the originals to something else.
The last Lock.txt file should be copied to /lib and granted only read/write permissions with no execute.
A file named Quarantine should be created in Desktop and username "lei906" in cd.def and the fake_pwd files should be changed with the name of the user on the virtual machine.
The Quarantine folder should be granted only read/write permissions using chmod with mode -R after copying a whole root folder from a virtual machine with no important data and of the same type as the original system. That and these files should also be given +X permission using chmod comand which will give execute to directories within the folder. This will insure that they can be accessed by users but no file created inside of them can execute. One should make sure to remove all permissions to execute from all files using -R mode and -x option before changing the directories to execute mode using X option.
The original bash-master folder can be also found in https://github.com/bminor/bash and all code in that folder is taken from there.
