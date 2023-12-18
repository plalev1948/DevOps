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

</div>
</body>
</html>