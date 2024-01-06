<h2> Root-level Directories: </h2>

* `ctrl + alt  + T` = opens a terminal on many Linux systems
* `/bin` - Binary files for single user mode commands
* `/sbin` - Binary files for multi-user commands
* `/boot` - Linux images and boot configuration files
* `/dev` - Pseudo files representing devices
* `/etc` - Configuration files
* `/home` - user files
* `/lib` - software library dependencies
* `/root` - root user files
* `/usr` - additional binaries
* `/var` - updating files (logs, app data, cache)
* Pseudo File Directories: created during system event for example boot
* `/proc` - files representing running system processes
* `/dev` - pseudo files representing devices - hardware devices
* `/sys` - data on system and kernel resources

<h2> Basic Commands: </h2>

* `clear`
* `exit`
* `locale` - refer to my geographic location
* `cd / usr/share/i18n/locales/` - the `locale` setting are stored in
* `localectl status` - to view and edit `locale` settings
* `pwd` - present work directory
* `ehco $PWD` - tells Linux to output the specified value in `pwd`
* `history` - outputs the last 100 commands typed by the user
* `df - ht ext4` - this will display all of the block devices on your system, along with their size and their mount point

<h2> Managing System Hardware: </h2>

* `lsblk | grep sd`
* `dmesg` - this will display messages related to the current ringbuffer. It generates a lot of data
* `dmesg | grep wl`
* `sudo lshw | less` - you get access to all necessary diagnostics
* `yum install lshw`

<h2> Working with Linux Software Repositories and package managers: </h2>

* `apt search business card | less`
* `apt show glabels`
* `sudo apt install glabels`
* `sudo apt-get install glabels`
* `sudo lxc exec (the name of the container) /bin/bash (to specify the type of shell I want to run)` - to open the terminal session within the running container
* `sudo apt install snapd` - command to install locally `snapd`
* `snap install nextcloud` - command to install nextcloud with `snap`
* `cd /var/snap` - enter a directory
* `ls` 
* `cd nextcloud` - enter nextcloud directory

<h2> Linux Command Line - track down and manage digital resources, test network connectivity, build scripts to improve work efficiency and bash scripting: </h2>

* `sudo apt update` - use the following command to update the package lists to get information on the newest versions of packages and their dependencies:
* `sudo apt upgrade` - you can upgrade the installed packages to their latest versions using the following command
* `sudo apt full-upgrade` - you can also perform a full system upgrade, which includes installing new dependencies if required;
* `sudo apt list` --upgradable - you can check if your system is up to date by running this command;
* `sudo apt install info` - install info
* `info` - offers a menu of major topics, including a list of installed programs
* `cd /usr/share/doc/wget` - open the documentation
* `man wget` - this command will display a well-organized reference listing that command`s syntax, usage patters and command line arguments.
* `wget` - a simple program that you run with the address of a web page or file that you would like to download to your current directory
* `wget --help` - displays different commands and helps the user with the usage
* `wget --help | less` - to pipe this output to the less text reader
* `type wget` - this can tell you how a specifiedword would be interpreted by Bash. For example, running type of wget, for instance, tells us that it's a binary command that actually exists in the usr/bin directory.
* `ls -a` - lists all the files in the directory
* `less .bashrc` - shows what the file is consisted of
* `less .profile`
* `less /etc/profile`
* `cat /etc/passwd`
* `ls -a` 
* `ls --all` 
* `man ls` - displays a well-organized reference listing that command`s syntax, usage patters and command line arguments.
* `ip addr` "or" `ip a`
* `ls -lht` "or" `ls -lh` "or" `ls -l`
* `ls -l /etc`
* `nano filel` - create a new directory with the text editor `nano`
* `locate adduser`
* `head /etc/group`
* `tail /etc/group`

<h2> Navigating the Linux File System: </h2>

* `pwd` = present work directory
* `cd` = change directory
* `mkdir` = create a directory
* `ls` = list the contents of the parent directory to show the new subdirectory
* `nono` = text editor
* `touch` = quick way to create empty files with unused names. Note: Using `touch` on an existing file, by the way, will simply update the datetime stamp of the file, which can be useful for some administrative purposes.
* `cp` = create copy. Note: create a copy of the file1 to a new directory
* `globing` = a way of spreading an action across a global target. Add every file that starts with file, no matter the lenght of the name
* `rm file?` = remove all files that start with file and have one digit after the word
* `rm file*` = remove all files
* `mv` = move files from parent directory to current directory
* `rm *` = remove all files from the current directory
* `cd..` = go one directory back
* `rmdir` = remove a directory

<h2> Searching the Linux File System: </h2>

* `locate` = quickest and easiest way to find files in Linux. For example you don't remember where the configuration file is and you just type `locate adduser`
* `sudo updatedb` = if you are looking for files that have been added quite recently. This will get you going when you need to find a file
* `cat /var/log/syslog`
* `cat /etc/group | grep ubuntu >> newfile` = rather than just printing the output to the screen, we could use this command to populate a file. The information is going to be included in the new file `newfile`.
* `cat /etc/group | grep ubuntu > newfile` = for the same command as above we could use an existing file, instead of creating a new one. This is done by only adding one arrow `>`.
* `head` = this will print by default only the first 10 lines of a file
* example: `head /etc/group`
* `tail` = this will print the last 10 lines of a file
* example: `tail /etc/group`
* `cut -d: -f3` = pull out one field of data from each line and process them all together. `d3` means to use every column as a field limiter or in other words to recognize the beggining and ending of each field. `-f3` is our way of saying that we are insterested of processing the contents of the 3rd field of each line.
* `cut -d: -f3 /etc/group | sort -n` = sort the numbers in a descending order
* `cut -d: -f3 /etc/group | sort -rn` = sort the numbers in a increasing order
* `wc newfile` = to see how much words a file was. `wc` stands for word count

<h2> Working with Archives: </h2>

* `tar xzf "name of the archive"`= to unpack an archive
* `tar czf newarchive.tar.gz[name of the archive] wordpress/[names of the files]` = to repack the files or any set of files we can use the command we perform the previous process in reverse
* `ls -l` = shows us the archive and it tells us that the file size is a little different from the original
* `tar cf largearchive.tar var`
* `gzip largearchive.tar`

<h2> Troubleshooting Peripherals: </h2>

* Step One - `Is the device recognized by the system?`
* Step Two - `Is the appropriate kernel module loaded?`
* `lsusb` = using the command line, with this command we can see what devices does Linux see
* `lspci` = this will show the devices connected through pci slots
* `sudo lshw` = this will gives us the whole hardware range in one output
* `sudo lshw > lshw-output` = the same command but redirected to a text file that can be read and after that type `less lshw-output`
* `ls /lib/modules/` = the software files that make up Kernel modules are usually kept in the `lib/modules/` directory
* `uname -r` = the module you want to use will depend on the Linux Kernel version you are running
* "ls /lib/modules` uname -r`"
* `lsmod | grep sound` = list the modules we are currently using, but this is modified to search only for the sound module
* `modprobe soundcore[module name]` = this is used, if I need to load the module

<h2> Network Address Translation (NAT) ranges </h2>

* `ip route show` = to see if you got access to a network router, one sort or another
* `sudo dhclient` = to see, if there is a DHCP server on the network; DHCP = Dynamic Host Configuration Protocol
* `ip addr` = to see my own ip address
* `route` = similar output as `ip route show`
* `ifconfig` = gives the same output as `ip addr`
* `netstat -i` = for more detailed data on network connection and configurations we can use this program
* `netstat -l` = checks and displays all the open and listening ports. This is an easy way to check, if there are any unnecessary and insecure entry points
* `ss -i` = this command can tell you all kinds of good and bad news about your networking interfaces
* `host` = you can also review the status of your DNS server using the command
* `ping 8.8.8.8` = you can try pinging a known ip address. `Ping` is a simple command that repeatedly sends short messages to a network address with the request the message be echoed back, letting us know that the address is live.
* `sudo nano /etc/hosts` = there we can type an ip address with a website name, save the changes and the users of this local machine will be redirected to this ip address every time when they type the name of the site, even if there is a real website out there.

<h2> Remote Connections and SSH: </h2>

* cd `/etc/ssh`
* `sudo nano sshd_config`
* `ssh ubuntu@10.0.31.131[the name of the user account you want to use]@[the server's remote address]` = to enter a terminal session on the client
* `exit` = to stop the session
* `ssh -p 2222 ubuntu` = to change the port; note: you may need to specify the port using `-p`
* `ssh -i /home/myusername/mykeyfile.pem ubuntu@10.0.31.131` = if I run Linux instances on Amazon's EC2 platform. I can point to the myusername file to the client's local machine using `-i`.
* ` scp update-local.sh[the name of the local file that I want to send] ubuntu@10.0.31.131[username]@[ip address of the remote host]:/home/ubuntu[the location of the saved file]` = this command is used to securely copy files between machines


<h2> Linux Scripting: </h2> 

* `nano myscripts.sh` = create a script file
* `chmod +x myscript.sh` = when using the change mode command, we will make the file executable by adding the value x
* `./myscript.sh` = to run the script in the file
* `fi` = you close an `if` statement with a `fi`
* `esac` = you close an `case` statement with a `esac`
* `man builtins` = starts a list of commands you need to work with `builtins`


<h2> Monitoring System Resources </h2>

* `cd /proc` = key system information is kept in the directory here. The files here are not persistent, but are created dynamically with each system boot and in response to system events.
* `less meminfo` = The `meminfo` file, for instance, contains information about the capacity and usage levels of your system memory. The output shows how much physical memory I've got and how much of it is not currently being used.
* `less cpuinfo` = tells me everything about I could want to know about the capacity and specifications of the number of CPU cores. Those files are mostly usefull for understanding the system specs.
* `top` = to view how the hardware is actually being utilized by the system right now, you'll want to run `top`. `Top` provides a single automatically updating screen full of data on those processes using up the highest percentages of CPU and memory resorces.
* `free` = to see how close to the bottom of the barrel you are, run `free`. The key number you are looking for is "available". Adding `-h` to free will display results in megabytes and gigabytes rather than 7 and 8-digit byte counts. 
* example: `free -h`
* `df` = to see the state of all these storage devices currently mounted to your system, run `df`. You can use the `-t` argument to filter for just "ext4" formatted partitions, which is the format they are using.
* example: `df -t ext4` or `df -ht ext4` to get the partition sizes in himan-readable numbers
* `iftop` = a networking version of the command `top`
* `sudo apt install iftop` = command to install the command
* `sudo iftop -i eth0[active interface]` = after running this command you will see source and target addresses associated with requests in the top section of the screen and upload and download statistics below

<h2> Managing System Processes: </h2>

* `ps` = running this command with no arguments will display any processes running with the current shell
* `ps aux` = this will print information on every active process across your entire system
* `ps aux | wc` = piping the command to wc tells us that the number of lines is in the hundreds
* `ps aux | grep sshd` = we may be better off filtering for specific processes using `grep`. I'll `grep` for running instances of the SSH daemon.
* `man sshd`
* `journalctl --since "10 minutes ago"` = you can search through the system logs for any helpful messages. Many Linux distros now use the journald logging system
* `cd /var/log` = if `journald` isn't your thing or you're using a Linux distro that doesn't come with it, then you can always rely on the text-only log files managed by the `syslogd` system
* `dmesg` = tool for keeping track of running processes
* `yes > /dev/null &` = to launch a process called yes that will output a text string to a kind of black hole
* `kill 810[ID of the process]` = terminate the process and after that run ps to see, if the command has been terminated
* `sudo systemctl status apache2` = you can check on current state of a process using system ctl using `systemctl status`. This example shows you that the Apache HTTP server software is installed, active and enabled. Enabled means it's set to automatically load each time the computer boots. If we didn't want it to load on boot, I could run `systemctl disable` and after checking the status once again we will make sure it is indeed disabled.
* `sudo systemctl start apache` = you can use systemctl to manuall start or stop a process

<h2> Managing Process Priorities: </h2>

* `yes > /dev/null &`
* `nice -19 yes > /dev/null &` = we will prefix the command with a value of "19". This means that the process will act very nicely and reduces resource demands in favor of any competing processes.
* `top` = view how the hardware is actually being utilized by the system
* A `nice` process might take longer to complete. "19", by the way, is the maximum niceness that's possible, "-20", shown as "--20" is as nasty as it gets and 0 is neutral. If you would like to change the value of a running process you can use `renice`.

example: `renice 15 -p 80[process ID]`

<h2> Working with Users and Groups: </h2>

* `less /etc/shadow` = the file contains encrypted versions of all user passwords. With this command the user will be turned back, he doesn't have the authority.
* `sudo less /etc/shadow` = the file is going to be opened
* `less /etc/passwd` = this file holds user data
* `less /etc/group` = this performs a similar function for groups containing the group name and group ID
* `id ubuntu` = this command returns my user and group IDs, but also displays the groups of which I'm a member, including sudo
* `who` = this command tells us, which users are currently logged in, when their sessions began and where they came from
* `w` = this command tells us not only who is currently logged in, but what he is also doing as well
* `last | less` = gives you every login since the beginning of the month

<h2> How to create and delete users and groups. </h2>

* `sudo useradd -m` = to create a new user and the `-m` part tells Linux to create a new directory in the home tree with the user's name
* `ls -a` = so we can see the hidden files
* `/etc/skel` = this is known as a skeleton directory, because it contains files or directories you'd like to form the skeleton or base of the `home` directory of new users as their new accounts are created.
* `sudo passwd pavel.test` = to create a password for a new user
* `sudo mkdir /var/secret` = create a new directory
* `sudo groupadd secter-group` = create a new group
* `sudo chown :secret-group /var/secret/` = change ownership properties of the "/var/secret" directory
* `sudo usermod -a -G secret-gorup[group name] pavel.test[username]` = "-a" means add and "-G" means to an existing group
* `sudo chmod g+w /var/secret/` = edit the permissions for the secret directory to allow group members to edit files; `g+w` means that we will add write permissions for members of the directory's group

<h2> Applying Object Permissions: </h2>

* `cd /var/secret`
* `ls -l` = `-l` means long version
* `su pavel.test` = `su` means switch user
* `touch data.txt` = create a new file
* `ls -dl` = this will list the attributes not of the contents of the attribute itself
* `chmod` = change an object's attributes using `chmod`
* `sudo chown ubuntu[group name]:secret-group /var/secret` = to change the owner of the group
* `chmod o+x data.txt` = add execute powers for others over data.txt, `o` - stands for others, `+` we are adding a power and `x` to indicate executable
* `chmod 777 data.txt `

<h2> Extending Object Usability: </h2>

* `ls -dl`
* `sudo chmod +t .` = add the sticky bit using this command and then run once again `ls -dl` command
* `nano /home/ubuntu/scripts/myscript.sh`
* `sudo ln -s /home/ubuntu/scripts/myscript.sh` = `ln` will create a link, while `-s` specifies that the link should be symbolic; the first location is the original script and it's location and the second one is where you'd like the symbolic link created
* `sticky bit`

<h2> Hardening The Linux Server: </h2>

* `nmap` = powerful and complicated tool
* `nmap -v -sT localhost` = `-v` for verbose and `-sT`, which will scan using the TCP protocol, followed by `localhost` will scan my own computer for open ports
* `systemctl disable apache2` = to simply stop and disable my web server using `systemctl`
* `nmap -v -sT bootstrap-it.com` = using the same command on a remote server

<h2> Working with Docker and Linux Containers: </h2>

* `docker network ls` = docker containers usually are going to be running clusters, they'll need a way to talk to each other and to outside networks.
* `docker network create newnet` = you can define and control networks manually from the command line or through various container orchestation tools like Kubernetes system and Amazon's Elastic Container Service (ECS)

<h2> Installing Docker Engine on Linux </h2>

* `sudo service ssh start`
* `sudo groupadd docker`
* `sudo usermod -aG docker $USER`
* `newgrp docker` = run the following command to activate the changes to groups
* `sudo service docker start`
* `docker run hello-world` = verify that you can run docker commands without sudo
* `sudo docker run -it ubuntu bash` = once this command is finished, we will find our selves logged in the Ubuntu container as `root`
* `exit` = when I exit, the container will shut down
* `docker ps` = list the currently running containers
* `sudo docker ps -a` = a list of all containers, including those that are stopped

<h2> Building a Customized Docker Image </h2>

* `nano Dockerfile`
* `sudo docker build -t webserver .` = use this command to get things rolling; `-t` will specify the naming tag, `webserver` in this case, we want to attach to this image; `.` dot tells the docker build to look for a Dockerfile in the current directory
* `sudo docker images` = run the command to confirm that our new images are loaded and waiting for us
* `sudo docker run -d -p 80:80 webserver` = fire up a container on the webserver image using the command; `-d` tells Docker to remain detached from the container, meaning we don't want to open a shell session inside; `-p` will permit incoming traffic from my host network on port 80 and through port 80 to the container
* `curl localhost` = run the command from the host machine to confirm everything is operational
* `docker login` = if I want to share the file with the closest people to me, I could push it to a repo in my `Docker Hub` account
* `docker search nextcloud` = search for an image, if you are going to need it
* `docker pull nextcloud` = download an image, if you want
* `docker tag webserver [username]plalev00/webserver`
* `docker push plalev00/webserver`