# Linux Commands Cheatsheet

## Table of Contents
- [File and Directory Management](#file-and-directory-management)
- [Navigation and File Viewing](#navigation-and-file-viewing)
- [Text Editors](#text-editors)
- [System Monitoring and Management](#system-monitoring-and-management)
- [Networking](#networking)
- [Log Management](#log-management)
- [System Administration](#system-administration)
- [Disk Management](#disk-management)
- [Scripting and Automation](#scripting-and-automation)
- [Development Tools](#development-tools)
- [Monitoring and Alerts](#monitoring-and-alerts)
- [User Management](#user-management)

---

## File and Directory Management
- **`ls`**: Lists files and directories in the current directory. Useful for quickly viewing contents.
- **`cd`**: Changes the current directory. Navigate through the file system.
- **`mkdir`**: Creates a new directory. Organise files by creating folders.
- **`rm`**: Removes files and directories. Caution: This action is irreversible.
- **`cp`**: Copies files and directories. Keep backups or duplicate files.
- **`mv`**: Moves or renames files and directories. Organise or rename files.
- **`pwd`**: Prints the current working directory. Know where you are in the file system.
- **`find`**: Searches for files and directories based on various criteria. Locate files quickly.
- **`chmod`**: Changes the permissions of files and directories. Control access to files.
- **`chown`**: Changes the ownership of files. Manage file ownership.
- **`ln`**: Creates symbolic links to files or directories. Useful for linking files or directories.
- **`tree`**: Displays the directory structure in a tree format. Useful for visualising directory contents.

## Navigation and File Viewing
- **`cat`**: Concatenates and displays the content of files. Useful for quickly viewing file contents.
- **`less`**: Displays file content one page at a time, with the ability to scroll. More memory efficient than `cat` for large files.
- **`more`**: Similar to `less`, but more basic, displaying file content one page at a time.
- **`head`**: Outputs the first part (usually 10 lines) of a file. Preview file contents.
- **`tail`**: Outputs the last part of a file. Often used with `-f` to monitor log files in real time.
- **`grep`**: Searches for a specified pattern in files. Filter file contents or logs.
- **`wc`**: Counts words, lines, and characters in a file. Useful for statistics on file content.
- **`cut`**: Removes sections from each line of files. Extracts columns or fields from a file or output.

## Text Editors
- **`vim`**: A powerful text editor. Here's how to deal with it:
  - `i`: Enters insert mode to start editing text.
  - `:w`: Saves the file.
  - `:q`: Quits the editor.
  - `:wq`: Saves and quits.
  - `:q!`: Quits without saving changes.
  - Vim is commonly pre-installed on Linux systems and is lightweight but has a steep learning curve.
  
- **`nano`**: A more user-friendly text editor. Common shortcuts:
  - `Ctrl + O`: Saves the file.
  - `Ctrl + X`: Exits the editor.
  - `Ctrl + K`: Cuts the current line.
  - `Ctrl + U`: Pastes the cut line.
  - **Why use it**: Ideal for quick edits without needing to remember complex commands.

## System Monitoring and Management
- **`top`**: Displays system resource usage and running processes.
- **`htop`**: An enhanced version of `top`, with a user-friendly interface.
- **`df`**: Displays disk space usage.
- **`du`**: Displays disk usage of files and directories.
- **`free`**: Displays memory usage.
- **`uptime`**: Shows how long the system has been running.
- **`ps`**: Displays information about active processes.
- **`kill`**: Terminates a process by its ID.
- **`netstat`**: Displays network connections, routing tables, and interface statistics.
- **`ss`**: A more modern replacement for `netstat`, providing more options.
- **`lsof`**: Lists open files and the processes using them.
- **`iostat`**: Reports CPU and I/O statistics.
- **`vmstat`**: Reports virtual memory statistics.
- **`sar`**: Collects and reports system activity (CPU, memory, network).

## Networking
- **`ssh`**: Connects to a remote machine using SSH protocol.
- **`scp`**: Securely copies files between hosts over SSH.
- **`rsync`**: Efficiently synchronises files and directories between locations over SSH.
- **`wget`**: Downloads files from the web.
- **`curl`**: Transfers data from or to a server using various protocols.
- **`ping`**: Sends ICMP echo requests to network hosts.
- **`traceroute`**: Traces the route packets take to a network host.
- **`dig`**: Performs DNS queries.
- **`iptables`**: Configures Linux kernel firewall rules.
- **`ufw`**: Simplifies firewall management using iptables.
- **`nc` (netcat)**: A versatile network tool for debugging and sending raw data over the network.
- **`tcpdump`**: Captures network packets for analysis.

## Log Management
- **`logrotate`**: Manages log rotation, ensuring logs don’t consume too much disk space.

## System Administration
- **`sudo`**: Executes a command with root/admin privileges.
- **`apt-get`**: Package handling utility for Debian-based distributions.
- **`yum`**: Package manager for RPM-based distributions.
- **`systemctl`**: Controls the systemd system and service manager.
- **`journalctl`**: Views logs collected by systemd.
- **`service`**: Controls system services.
- **`crontab`**: Schedules periodic tasks using cron jobs.
- **`tar`**: Archives files and directories.
- **`gzip`**: Compresses files using the gzip algorithm.
- **`unzip`**: Extracts files from a zip archive.
- **`mount`**: Mounts a filesystem.
- **`umount`**: Unmounts a filesystem.
- **`fsck`**: Checks and repairs filesystems.
- **`tune2fs`**: Adjusts filesystem parameters.
- **`history`**: Displays recently executed commands.

## Disk Management
- **`fdisk`**: Manipulates disk partition tables.
- **`parted`**: Advanced tool for managing disk partitions.
- **`mkfs`**: Creates a filesystem on a partition.
- **`iotop`**: Displays I/O usage by processes.
- **`nmon`**: Performance monitoring tool for CPU, memory, disk, and network stats.

## Scripting and Automation
- **`bash`**: Executes bash scripts.
  - `bash script.sh`: Executes the specified bash script.
- **`chmod +x`**: Makes a script executable.
  - `chmod +x script.sh`: Allows the script to be run as `./script.sh`.
- **`./`**: Runs a script in the current directory.
  - `./script.sh`: Executes the script.
- **`alias`**: Creates an alias for commands to simplify usage.
  - `alias ll='ls -la'`: Shortens the command to list files with details.
- **`echo`**: Prints text or variables to the terminal.
  - `echo "Hello, World!"`: Outputs `Hello, World!`.

## Development Tools
- **`git`**: Version control system for managing source code.
- **`make`**: Builds and manages dependencies for software projects.
- **`gcc`**: GNU Compiler Collection for compiling C, C++, and other languages.
- **`docker`**: Manages Docker containers.
- **`kubectl`**: Manages Kubernetes clusters.

## Monitoring and Alerts
- **`dstat`**: Combines `vmstat`, `iostat`, `netstat` into a single tool for monitoring system performance.
- **`watch`**: Repeats a command at regular intervals and displays the output.

## User Management
- **`useradd`**: Creates a new user account.
- **`usermod`**: Modifies user account details.
- **`passwd`**: Updates a user’s password.
- **`groupadd`**: Creates a new user group.
- **`groups`**: Shows the groups a user belongs to.
