# Linux Filesystem

## Overview

Linux uses a single hierarchical filesystem that starts from the root directory (`/`). Every file and directory exists somewhere under this root. Each top-level directory has a specific purpose, such as storing configuration files, logs, user data, programs, or system information.

## Important Directories

### / - root of the Linux filesystems
### /etc - stores the system wide config files
### /var - stores the variable data that are changed during the operation
### /var/log - contains the log files
### /home - contains the directories of the user
### /root - home directories of the root user
### /tmp - stores the temporary files of the system
### /proc - provides the process and kernel info
### /usr - consists of the installed program, resources and libraries 
### /opt - Typically used for optional or third-party software
### /dev - consists of the device files

## Commands I Practiced

- `pwd` – Displays the current working directory.
- `ls` – Lists the files and directories in the current location.
- `cd` – Changes the current directory.
- `cat` – Displays the contents of a file.
- `which` – Shows the location of an executable command.

## Hands-on Lab

Created a practice directory named `linux-lab`.
linux-lab
/configs --- app.conf
/ logs --- application.log
/scripts --- deploy.sh

Practiced:

- Creating directories using `mkdir`
- Creating files using `touch`
- Listing files using `ls`
- Navigating using `cd`
- Viewing the current directory using `pwd`

## What I Learned

- Linux starts from a single root directory (`/`).
- Every directory has a specific purpose.
- `/etc` stores system configuration files.
- `/var/log` stores log files that help troubleshoot issues.
- `/home` contains user home directories.
- `/root` is the home directory of the root user.
- `/proc` is a virtual filesystem that provides system and process information.
- Commands like `pwd`, `ls`, `cd`, `cat`, and `which` help navigate and inspect the Linux system.

## Production Scenario

If an application stops working after a configuration change, I would first check the application's configuration files, which are commonly stored under `/etc`.
After verifying the configuration, I would check the relevant log files (commonly under `/var/log`) to identify any errors or warnings that explain why the application failed.