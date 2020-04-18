# ansible-retropie
My Ansible scripts I use to provision a Raspberry Pi with RetroPie installed.
Forked From: adrianmoisey/ansible-retropie by: adrianmoisey  

## Purpose
This project was forked to provide a means of locally testing the playbook changes
using a Debian VM.

### Getting started

#### Linux
Install the following applications
* VirtualBox
* Vagrant

#### Windows (not supported by ansible)
Install the following applications
* Cygwin
* VirtualBox
* Vagrant

To run ansible-playbook with vagrant the following bat file needs to 
be added to your system path this ensures ansible-playbook runs in cygwin

```
@echo off

REM If you used the stand Cygwin installer this will be C:cygwin
set CYGWIN=C:\cygwin64

REM You can switch this to work with bash with %CYGWIN%\bin\bash.exe
set SH=%CYGWIN%\bin\bash.exe

"%SH%" -c "/bin/ansible-playbook %*"
```

## History
Added a Vagrant file (VagrantFile) to provide a Debian VM with the pi user

