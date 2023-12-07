<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
  <title>Getting Started with Linux</title>

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
  <ul>
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

</div>
</body>
</html>