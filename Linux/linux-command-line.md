* ctrl + alt  + T = opens a terminal on many Linux systems

Root-level Directories:

/bin - Binary files for single user mode commands

/sbin - Binary files for multi-user commands

/boot - Linux images and boot configuration files

/dev - Pseudo files representing devices

/etc - Configuration files

/home - user files

/lib - software library dependencies

/root - root user files

/usr - additional binaries

/var - updating files (logs, app data, cache)

Pseudo File Directories: created during system event for example boot

/proc - files representing running system processes

/dev - pseudo files representing devices - hardware devices

/sys - data on system and kernel resources

Commands:

* clear

* exit

* locale - refer to my geographic location

* cd / usr/share/i18n/locales/ - the `locale` setting are stored in

* localectl status - to view and edit `locale` settings

* pwd - present work directory

* ehco $PWD - tells Linux to output the specified value in `pwd`

* history - outputs the last 100 commands typed by the user

* df - ht ext4 - this will display all of the block devices on your system, along with their size and their mount point

Managing System Hardware:

* lsblk | grep sd

* dmesg - this will display messages related to the current ringbuffer. It generates a lot of data

* dmesg | grep wl

* sudo lshw | less - you get access to all necessary diagnostics

* yum install lshw

Working with Linux Software Repositories and package managers:

*  apt search business card | less

*  apt show glabels

*  sudo apt install glabels

*  sudo apt-get install glabels

*  sudo lxc exec (the name of the container) /bin/bash (to specify the type of shell I want to run) - to open the terminal session within the running container

*  sudo apt install snapd - command to install locally snapd

*  snap install nextcloud - command to install nextcloud with `snap`

*  cd /var/snap - enter a directory

*  ls 

*  cd nextcloud - enter nextcloud directory

Linux Command Line - track down and manage digital resources, test network connectivity, build scripts to improve work efficiency and bash scripting:

* sudo apt update - use the following command to update the package lists to get information on the newest versions of packages and their dependencies:
* sudo apt upgrade - you can upgrade the installed packages to their latest versions using the following command
* sudo apt full-upgrade - you can also perform a full system upgrade, which includes installing new dependencies if required;
* sudo apt list --upgradable - you can check if your system is up to date by running this command;
* sudo apt install info - install info
* info - offers a menu of major topics, including a list of installed programs
* cd /usr/share/doc/wget - open the documentation
* man wget - this command will display a well-organized reference listing that command`s syntax, usage patters and command line arguments.
* wget - a simple program that you run with the address of a web page or file that you would like to download to your current directory
* wget --help - displays different commands and helps the user with the usage
* wget --help | less - to pipe this output to the less text reader
* type wget - this can tell you how a specifiedword would be interpreted by Bash. For example, running type of wget, for instance, tells us that it's a binary command that actually exists in the usr/bin directory.
* ls -a - lists all the files in the directory
* less .bashrc - shows what the file is consisted of
* less .profile
* less /etc/profile
* cat /etc/passwd
* ls -a 
* ls --all 
* man ls - displays a well-organized reference listing that command`s syntax, usage patters and command line arguments.
* ip addr `or` ip a
* ls -lht `or` ls -lh `or` ls -l
* ls -l /etc