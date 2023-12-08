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