<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<h1> Goals </h1>
<p> My goal is by the end of the learning to be able to install and manage simple Linux deployment and futher develop my Linux administration skills. <p>
</head>

<body>
<div class="main-paragraph">
<br>
  <h2>Here I will store information about:</h2>
  <ul>
    <li>linux and open source ecosystem</li>
    <li>proper care and feeding of your linux environment</li>
    <li>software package management systems</li>
    <li>server virtualizations</li>
    <li>server application administration</li>
  </ul>
<br>

<h2>Repository Overview:</h2>
<ul>
  <li>Linux installation</li>
  <li>Configure the Linux boot process</li>
  <li>Configure the Linux environment</li>
  <li>Administrating the Linux desktops</li>
  <li>Linux servers</li>
</ul>

<h2> Resources:</h2>
<ul>
  <li>https://bootstrap-it.com/linux-start/</li>
</ul>

<h2> Notes: </h2>

- [The Layers of a Linux Distribution: <a name="firstnote"></a>](#the-layers-of-a-linux-distribution-)
- [Linux Distributions: <a name="secondnote"></a>](#linux-distributions-)
- [Linux Installation: <a name="thirdnote"></a>](#linux-installation-)
- [Configuring the Linux Environment: <a name="fourthnote"></a>](#configuring-the-linux-environment-)
- [Linux Runlevels <a name="fifthnote"></a>](#linux-runlevels-)

## The Layers of a Linux Distribution: <a name="firstnote"></a>

<ol>The Layers of a Linux Distribution:
  <li>The Linux kernel handles system hardware resources on behalf of the OS user</li>
  <li>A Linux desktop is software designed to manage graphic interface features like windows, menus, and application controls</li>
  <li>A Linux distribution will use a specific suite of system tools (like software package managers and process managers)</li>
</ol>

## Linux Distributions: <a name="secondnote"></a>

Because Linux is open source many people have created their version of Linux, also known as Distribution or Distros. They fit special needs.

<ul>Example for such distributions are:
  <li>Android (mobile devices)</li>
  <li>Red Hat Enterprise Linux</li>
  <li>CentOS</li>
  <li>Kali Linux (security)</li>
</ul>

Distributions are build into families. The best know families are Debian (Ubuntu, Mint and Kali Linux), Red Hat Enterprise Linux (CentOS and Fedora), SUSE (OpenSUSE) and Arch Linux (LinHES and Manjaro).

## Linux Installation: <a name="thirdnote"></a>

<p>Backround</p>
<p>Configuration options</p>
<p>Install: PC and Cloud/Docker instances</p>

## Configuring the Linux Environment: <a name="fourthnote"></a>

  * Manage the Linux Environment 
  * Understand the Linux boot process - BIOS/UEFI -> Master Boot Record (MBR) on boot launched -> Bootloader (GRUB) launched -> Linux kernel loaded into memory -> init executes config file targets (runlevels) -> Display manager loaded -> Desktop loaded
  * Understand the Linux Filesystem Hierarchy Standard
  * Manage your locale settings
  * Discover your hardware environment

## Linux Runlevels <a name="fifthnote"></a>

<ul>
  <li>0 - system halt - this means "applying code `0` will shut the machine off"</li>
  <li>1 - single-user (rescue) mode - allows to work through on a problem/issue with the stability that no other user will log on without your knowledge</li>
  <li>3 - multi-user mode without GUI - provides only terminal connections</li>
  <li>5 - multi-user mode with GUI - standard desktop machine. Multi-user means that more than 1 user can login at once</li>
  <li>6 - reboot</li>
</ul>

Notes:

Using Linux Help Resources:
* `man builtins` = starts a list of commands
* `info`


Linux is probably going to be the infrastucture powering things under the hood. It has:
* most web and app servers
* most CI/CD deployments
* Docker virtualizes Linux host kernel resources
* All AWS EC2 instances

LMV = Logical Volume Management

Overview of File System Hierarchy Standard (FHS)

Managing Linux Environments:

Managing System Hardware:

Package managers:
* working with Linux Software Repositories:
Productivity software:
Linux desktop applications: some of the major ones that might come in handy:
- libre office
- Google Docs
- Thunderbird and Firefox
- Apache and Engine X
- MariaDB
- Samba
- Microsoft PowerShell

Understanding Linux Desktops:
Currently there are 3 main classes of desktop:
- Cinnamon/Mate
- Gnome
- Xfce
- KDE

Working with the Linux Server:
server - a computer on which there is at least one process, whose job it is to serve the needs of a remote user, usually called a client

Using Linux Containers:

Working with Server Apps: Apache

A software like APACHE or NGINX is a software that controls the way digital resources like webpages on a server are exposed to clients across a network or across the internet.

Dropbox and Amazon Web Services S3 - document hosting service.

To install manually Nextcloud you need to :
* install a LAMP server;
* configure service connectivity;
* download Nextcloud archive;
* set permissions;
* troubleshoot.

All of this above can be done with a snap. `A snap` is a kind of virtual partition that exists within your file system inside its own isolated environment.

<h2>Linux Command Line:</h2>
<br>
  <ul>
    <li>basics of command syntax patterns</li>
    <li>finding and panipulating data in the Linux file system</li>
    <li>network connectivity</li>
    <li>bash scripting</li>
  </ul>
  <br>
  <ul> Overview of things to learn:
    <li>core command line tools</li>
    <li>help resources</li>
    <li>configure the Linux environment</li>
    <li>command line syntax</li>
    <li>resources are disributed through the Linux file system</li>
  </ul>

<br>
  <ul>Goal:
    <li>use the Linux command line to track down and manage digital resources</li>
    <li>test network connectivity</li>
    <li>build scripts to improve work efficiency</li>
    <li>bash scripting</li>
  </ul>

Linux has its own built-in support systems.

I prefixed apt with the word sudo because on most Linux systems sudo allows privileged users to run single programs with full admin powers without the need to run entire shell sessions as root, something that over the long term carries significant security risks.

You can use the `/` to make searches in Ubuntu, just like you are using `ctrl` + `F`. For example, if I type info, after that `/wget` and hit enter it's going to take me to the place where `wget` has been used. After that you can use the up and down keys to move to a menu that you would like to explore further and hit Enter.

Example of a search using `/`:
1. type `/wget`.
2. after the search is on `wget`, hit Enter.
3. hit again Enter on `examples`.
4. navigate to `simple usage` and hit enter.

The same result can be achieved, if I type:

* `info wget examples simple`

The Linux Terminal: the Linux shell is not quite the same thing as the Linux Terminal. The command `ls -a` lists all the files in the directory. The dot at the beginning of the file name indicates that it's hidden, meaning it won't be displayed when you run a plain old `ls` command without the a argument.

Linux Syntax Patterns and Shortcuts: common usage patters shared by many Linux commands.
  Invoking a command always starts with the command name. In some cases, as with the `ls` command, just the name on its own is enough to return a result. However,
you'll usually need to add some combination of arguments and parameters to get the most out of a tool.

  There are exceptions of course: using the administration `ip` command, for instance, can use the `addr` argument without a dash to show the IP addresses
associated with your system's network interfaces. 

  Keep in mind there is autocomplete for Linux! It will work when there is only one possible matching possibility in the directory.

Navigating the Linux File System:

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

* example of a command: cd home/ubuntu/scripts
* example `nono`: type Hello, press `Ctrl` + `X` to save and then `Y` to exit
* example `globing`: cp file* newdata/
* example `mv ../file`
* example `rmdir newdata/` = remove the newdata directory

Note: Deleted files cannot be restored.

Searching the Linux File System:

* `locate` = quickest and easiest way to find files in Linux. For example you don't remember where the configuration file is and you just type `locate adduser`
* `sudo updatedb` = if you are looking for files that have been added quite recently. This will get you going when you need to find a file

* Rather than just printing just the text directly to the screen, however, it can also search and, if desired, manipulate the contents of a file by sending it through what's called a `pipe`. Multiple text manipulation tools can then be invoked to filter the streaming text.

* example: we will use `cat` to read the group file that contains information about system groups and that lives in the `etc` directory.
$ cat /etc/group | grep ubuntu

* Many files will regularly generate thousands or even millions of text messages that are written to log files so that later you can revisit critical events. To manage the problem of working with all this data, Bash comes with a full set of text manipulation tools for reading.

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

* standard input -> `stdin` -> 0 -> the input comes from the keyboard -> example: `mysql -u root -p < mydatabase.sql` this example will open the database as root user, the right arrow `<` will tell the system where to find the file
* standard output -> `stdout` -> 1 -> example: `echo` Hello -> result: Hello ; `echo "Hello" >> myFile.txt` ; cat myfile.txt
* standard error -> `stderr` -> 2 -> wget pluralsight.comm -> wget pluralsight.comm 2> errorfile.txt -> cat errorfile.txt  Note: the number `2` is a number for designated error.

Working with Archives:

* The most common thing for compresion is `tar` when working with archives. The `.tar` ending tell us that it's an archive and the `.gz` tells us that it's also compresed gzip algorithm.

* `tar xzf "name of the archive"`= to unpack an archive
* `tar czf newarchive.tar.gz[name of the archive] wordpress/[names of the files]` = to repack the files or any set of files we can use the command we perform the previous process in reverse
* `ls -l` = shows us the archive and it tells us that the file size is a little different from the original
* `tar cf largearchive.tar var`
* `gzip largearchive.tar`

To work with zip files, we have to know how to work with unzip.
* `unzip akismet.4.1.zip[name of the zip file]`
* `ls akismet[name of the zip file]`
* `zip newname.zip *` = you can create a new zip archive using the new "zip" command

Linux Kernel Modules and Peripherals:
Troubleshooting Peripherals:
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

The sounds files in Linux end with the `.ko` file extension.

Linux Network Connectivity:

<ul>
  <br>This includes:
  <li>Analyzing network connectivity</li>
  <li>Confirguring DNS</li>
  <li>SSH remote sessions</li>
</ul>

Network Connectivity - building an effective networking system requires some networking skills.
* `ip route show` = to see if you got access to a network router, one sort or another
* `sudo dhclient` = to see, if there is a DHCP server on the network; DHCP = Dynamic Host Configuration Protocol
* `ip addr` = to see my own ip address

The difference between IPv4 and IPv6 addresses is that IPv6 addresses are drawn from a theoretical pool of numbers that exponentially larger than IPv4. The reason is simple: IPv4 addresses are made up 4 IP bit numbers.

<span> **IPv4** </span>
<br> 
example -> 256.256.256.256 = 4 294 967 296 (2^32) available combinations 
example address: 192.168.1.3

<h2> Network Address Translation (NAT) ranges </h2>

* from `10.0.0.0` to `10.255.255.255`
* from `172.16.0.0` to `172.31.255.255`
* from `192.168.0.0` to `192.168.255.255`

<span> **IPv6** </span> <br>
example address: 2001:0db8:85a3:0000:0000:8a2e:0370:7334

* `route` = similar output as `ip route show`
* `ifconfig` = gives the same output as `ip addr`
* `netstat -i` = for more detailed data on network connection and configurations we can use this program
* `netstat -l` = checks and displays all the open and listening ports. This is an easy way to check, if there are any unnecessary and insecure entry points
* `ss -i` = this command can tell you all kinds of good and bad news about your networking interfaces

Domain Name System (DNS) Configuration:
The DNS system was created to map numeric ip addresses like `52.33.197.135` like `Pluralsight.com`. For that to work there have to be databases accessible to every network that contains an up to date index of names. The services that maintain these databases are called DNS servers. You can easily tell, whether your computer has access to a DNS server by pointing a web browser to a DNS name of a website like `bootstrap-it.com`. If you can successfully load the page, than this means that your browser received the correct translation of the name you typed in to it's actual public address.

* `host` = you can also review the status of your DNS server using the command
* `ping 8.8.8.8` = you can try pinging a known ip address. `Ping` is a simple command that repeatedly sends short messages to a network address with the request the message be echoed back, letting us know that the address is live.

If pinging an ip address works, but pinging associated DNS servers doesn't, it means something is wrong with our DNS server. On some distributions you manage your DNS settings from the `cat /etc/resolv.config` file.

* `sudo nano /etc/hosts` = there we can type an ip address with a website name, save the changes and the users of this local machine will be redirected to this ip address every time when they type the name of the site, even if there is a real website out there.

<h2> Remote Connections and SSH: </h2>

<span> The open SSH package was designed to solve two big problems. It is a popular and reliable protocol.</span> 

Remote Is The New Local:
* Accessing headless servers
* Accessing virtual machines
* Accessing workloads on distant servers

Server:
* apt install openssh-server
* or: dnf install openssh-server

Client:
* apt install openssh-client
* or: dnf install openssh-clients

Both the server and client iterations are controlled by configurations by the `/etc/ssh` directory. We will use and edit the `sshd_config` file to manage the system's host behavior and `ssh_config` controls the way your system will log you in as a client on remote hosts.

* cd `/etc/ssh`
* `sudo nano sshd_config`

By default SSH sessions use port 22.

* `ssh ubuntu@10.0.31.131[the name of the user account you want to use]@[the server's remote address]` = to enter a terminal session on the client
* `exit` = to stop the session
* `ssh -p 2222 ubuntu` = to change the port; note: you may need to specify the port using `-p`
* `ssh -i /home/myusername/mykeyfile.pem ubuntu@10.0.31.131` = if I run Linux instances on Amazon's EC2 platform. I can point to the myusername file to the client's local machine using `-i`.
* ` scp update-local.sh[the name of the local file that I want to send] ubuntu@10.0.31.131[username]@[ip address of the remote host]:/home/ubuntu[the location of the saved file]` = this command is used to securely copy files between machines

note: `scp` = secure copy

<h2> Linux Scripting: </h2> 

* `nano myscripts.sh` = create a script file
* `chmod +x myscript.sh` = when using the change mode command, we will make the file executable by adding the value x
* `./myscript.sh` = to run the script in the file

Working with Loops and Flow Controls:

* `fi` = you close an `if` statement with a `fi`
* `esac` = you close an `case` statement with a `esac`

The difference between `builtins` and `external commands`. A `builtin` is a program that's build in to the Bash scripting environment. Calling a builtin from within your script will often use up less system overhead and create fewer subprocesses. Somethimes. the problem you're addressing can be better solved through an external program, so you might choose to reach outside the native Bash environment. Running `man builtins` from the command line will probably get you all the commands you need.

* `man builtins` = starts a list of commands you need to work with `builtins`

<h2> Linux System Administration: </h2>


* System permormance optimization
    * Troubleshooting problems
    * Preventing problems
    * Understanding capacity
    * Searching log data
    * Controlling process lifecycles
* Account authentication - Passwords
* User and groups
* Security
  * Permissions
  * Software updates
  * Network Port Audits
  * Encryption
* Docker containers


<h3> Monitoring System Resources </h3>

We will take a look at `System performance metrics` like `RAM`, `Storage`, `CPU` and `Bandwith`. The 2 main goals here are:
* Understand capacity usage
* Identify (and terminate) rogue processes


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

<h3> Managing System Processes: </h3>

In this section we are going to have the commands for the following events:
* Monitor process event data
* Terminate processes
* Enable/disable processes

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

The difference between the commands `kill` and `killall` is that `kill` will only operate on the process using that specific PID, while `killall` kills all instances of "yes" running on a system.

`sudo systemctl status apache2` = you can check on current state of a process using system ctl using `systemctl status`. This example shows you that the Apache HTTP server software is installed, active and enabled. Enabled means it's set to automatically load each time the computer boots. If we didn't want it to load on boot, I could run `systemctl disable` and after checking the status once again we will make sure it is indeed disabled.
`sudo systemctl start apache` = you can use systemctl to manuall start or stop a process

<h3> Managing Process Priorities: </h3>

To manage a couple of applications and you want them to "play" together and not consume so much memory you can use `nice`.

* `yes > /dev/null &`
* `nice -19 yes > /dev/null &` = we will prefix the command with a value of "19". This means that the process will act very nicely and reduces resource demands in favor of any competing processes.
* `top` = view how the hardware is actually being utilized by the system

A `nice` process might take longer to complete. "19", by the way, is the maximum niceness that's possible, "-20", shown as "--20" is as nasty as it gets and 0 is neutral.
If you would like to change the value of a running process you can use `renice`.

example: `renice 15 -p 80[process ID]`

<h3> Working with Users and Groups: </h3>

* Account data - system files where user and group data is stored
* Access control
* account activity data
* Managing accounts
* Managing groups

Admin Powers: Best Practices
* Avoid using the root account
* Create unique accounts for each user
* Assign only necessary authority to each user
* Use admin power only via sudo

* `less /etc/shadow` = the file contains encrypted versions of all user passwords. With this command the user will be turned back, he doesn't have the authority.
* `sudo less /etc/shadow` = the file is going to be opened
* `less /etc/passwd` = this file holds user data

example: `ubuntu:x:1000:1000:Ubuntu:/home/ubuntu:/bin/bash` . Meaning of every symbol:
ubuntu = this field has the user's name
x = indicates the existance of password in the shadow file
1000:1000 = user ID and group ID numbers
/home/ubuntu: = the file system address is the location of the user's home directory
/bin/bash = default shell

* `less /etc/group` = this performs a similar function for groups containing the group name and group ID
* `id ubuntu` = this command returns my user and group IDs, but also displays the groups of which I'm a member, including sudo
* `who` = this command tells us, which users are currently logged in, when their sessions began and where they came from
* `w` = this command tells us not only who is currently logged in, but what he is also doing as well
* `last | less` = gives you every login since the beginning of the month

How to create and delete users and groups.
* `sudo useradd -m` = to create a new user and the `-m` part tells Linux to create a new directory in the home tree with the user's name
* `ls -a` = so we can see the hidden files
* `/etc/skel` = this is known as a skeleton directory, because it contains files or directories you'd like to form the skeleton or base of the `home` directory of new users as their new accounts are created.
* `sudo passwd pavel.test` = to create a password for a new user
* `sudo mkdir /var/secret` = create a new directory
* `sudo groupadd secter-group` = create a new group
* `sudo chown :secret-group /var/secret/` = change ownership properties of the "/var/secret" directory
* `sudo usermod -a -G secret-gorup[group name] pavel.test[username]` = "-a" means add and "-G" means to an existing group
* `sudo chmod g+w /var/secret/` = edit the permissions for the secret directory to allow group members to edit files; `g+w` means that we will add write permissions for members of the directory's group


<h3> Securing Your Linux Server covers: </h3>

* Permissions
* Software patches
* managing network ports
* Data encryption

Applying Object Permissions:

* `cd /var/secret`
* `ls -l` = `-l` means long version
* `su pavel.test` = `su` means switch user
* `touch data.txt` = create a new file
* `ls -dl` = this will list the attributes not of the contents of the attribute itself
* `chmod` = change an object's attributes using `chmod`
* `sudo chown ubuntu[group name]:secret-group /var/secret` = to change the owner of the group
* `chmod o+x data.txt` = add execute powers for others over data.txt, `o` - stands for others, `+` we are adding a power and `x` to indicate executable

Permissions: Numeric Notation
Read: r - 4
Write: w - 2
Execute: x -1

Full permissions: 4 + 2 + 1 = 7, `7` indicates the highest permissions level possible
Read/execute: 5, `5` indicates someone with read and execite powers, but not write, as would be worth 5
Execute: 1, `1` indicates someone with only execute powers

for example: `-rw-rw-r-x` stands for 665 and a secret directory is worth `775`

`chmod 777 data.txt ` = this would add execute powers to the user and group and write to others

<h3> Extending Object Usability: </h3>

By adding a `sticky bit` value to the directory permissions, group members will only be able to delete their own files within the directory, but not files belonging to others.

* `ls -dl`
* `sudo chmod +t .` = add the sticky bit using this command and then run once again `ls -dl` command

Sometimes you might need access to individual directories or files from more than one location. A very simple solution is to create a symbolic link to the source file in the location where you need it. There's no limit to the number of symlinks you can create, and they behave just like the real thing, because for all intents and purposes they are the real thing.

* `nano /home/ubuntu/scripts/myscript.sh`
* `sudo ln -s /home/ubuntu/scripts/myscript.sh` = `ln` will create a link, while `-s` specifies that the link should be symbolic; the first location is the original script and it's location and the second one is where you'd like the symbolic link created


<h3> Hardening Your Server includes: </h3>

* Reducing vulnerability
* Patching systems
* Understanding network ports
* Managing network ports

Service Access Controls:
* Service hardening
* Port control
* Firewall rules

* `nmap` = powerful and complicated tool
* `nmap -v -sT localhost` = `-v` for verbose and `-sT`, which will scan using the TCP protocol, followed by `localhost` will scan my own computer for open ports
* `systemctl disable apache2` = to simply stop and disable my web server using `systemctl`
* `nmap -v -sT bootstrap-it.com` = using the same command on a remote server


<h3> Data Encryption </h3>

Email Server Elements:
* Mail transport agent (MTA) - Postfix. Sendmail
* Mail delivery agent (MDA) - Dovecot
* Mail user agents (MUA) - Thunderbird

<h3> Working with Docker and Linux Containers: </h3>

Physical Server Model:
* Operating System
* Hardware (CPU, RAM, Disk Drives...)

Hypervisor Virtualization:
* Virtual Client
  * Hypervisor (hardware emulation layer)
  * Linux Kernel
  * Hardware (CPU, RAM, Disk Drives...)

Container Virtualization:
* Ubuntu, SUSE, RHEL, Debian
  * Container Management Platform
  * Linux Kernel
  * Hardware

Linux in a Container World:
* Host Administration
  * Privileges
  * Kernel Access
* Container Administration
  * Application Design
* The Future of Linux
  * Microservices
  * DevOps
  * Development support

<h3> Understanding the Docker Ecosystem: </h3>

Docker Resources:
* Image hosting:
  * Docker Hub
  * Docker Registry - software package
* Storage:
  * Docker Volumes
  * Third-party solutions

* `docker network ls` = docker containers usually are going to be running clusters, they'll need a way to talk to each other and to outside networks.
* `docker network create newnet` = you can define and control networks manually from the command line or through various container orchestation tools like Kubernetes system and Amazon's Elastic Container Service (ECS)

<h3> Installing Docker Engine on Linux </h3>

* `sudo groupadd docker`
* `sudo usermod -aG docker $USER`
* `newgrp docker` = run the following command to activate the changes to groups
* `docker run hello-world` = verify that you can run docker commands without sudo


* `sudo service ssh start`


</div>
</body>
</html>