# Linux Commands Cheatsheet

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
- **`top`**: Displays system resource usage and running processes. Monitor system performance.
- **`htop`**: An enhanced version of `top`, with a more user-friendly interface.
- **`df`**: Displays disk space usage. Monitor available disk space.
- **`du`**: Displays disk usage of files and directories. Check which files are using up disk space.
- **`free`**: Displays memory usage. Monitor available RAM.
- **`uptime`**: Shows how long the system has been running. Useful for monitoring system stability.
- **`ps`**: Displays information about active processes. Monitor and manage running processes.
- **`kill`**: Terminates a process by its ID. Stop unresponsive or unwanted processes.
- **`netstat`**: Displays network connections, routing tables, and interface statistics. Monitor network activity.
- **`ss`**: A more modern replacement for `netstat`, providing similar functionalities with more options.
- **`lsof`**: Lists open files and the processes using them. Troubleshoot open file issues.

## Networking
- **`ssh`**: Connects to a remote machine using SSH protocol. Securely manage remote servers.
- **`scp`**: Securely copies files between hosts over SSH. Transfer files securely between servers.
- **`rsync`**: Efficiently synchronises files and directories between locations over SSH. Backup or replicate files.
- **`wget`**: Downloads files from the web. Fetch files from the internet.
- **`curl`**: Transfers data from or to a server using various protocols. Useful for interacting with APIs.
- **`ping`**: Sends ICMP echo requests to network hosts. Test connectivity to another host.
- **`traceroute`**: Traces the route packets take to a network host. Diagnose network issues.
- **`dig`**: Performs DNS queries. Troubleshoot DNS issues.

## System Administration
- **`sudo`**: Executes a command with root/admin privileges. Temporarily gain elevated permissions.
- **`apt-get`**: Package handling utility for Debian-based distributions. Install, upgrade, and remove packages.
- **`yum`**: Package manager for RPM-based distributions. Manage software packages.
- **`systemctl`**: Controls the systemd system and service manager. Start, stop, and manage system services.
- **`journalctl`**: Views logs collected by systemd. Troubleshoot system issues by examining logs.
- **`service`**: Controls system services. Start, stop, or check the status of services.
- **`crontab`**: Schedules periodic tasks. Automate tasks by setting up cron jobs.
- **`tar`**: Archives files and directories into a single file. Useful for backups and transferring multiple files.
- **`gzip`**: Compresses files using the gzip algorithm. Reduce file size for storage or transfer.
- **`unzip`**: Extracts files from a zip archive. Decompress files for use.
- **`mount`**: Mounts a filesystem. Access additional file systems.
- **`umount`**: Unmounts a filesystem. Safely remove filesystems.
- **`history`**: Displays the list of recently executed commands. Useful for tracking past commands.

## Scripting and Automation
- **`bash`**: Runs a bash script. Useful for automating tasks.
  - `bash script.sh`: Executes the specified bash script.
- **`chmod +x`**: Makes a script executable.
  - `chmod +x script.sh`: Allows the script to be run as `./script.sh`.
- **`./`**: Runs a script in the current directory.
  - `./script.sh`: Runs the script.
- **`sh`**: Runs a shell script.
  - `sh script.sh`: Executes the shell script.
- **`alias`**: Creates an alias for commands to simplify usage.
  - `alias ll='ls -la'`: Shortens the command to list files with details.
- **`echo`**: Prints text or variables to the terminal. Useful in scripts to output information.
  - `echo "Hello, World!"`: Outputs `Hello, World!`.

## Development Tools
- **`git`**: Version control system command-line tool. Manage source code and track changes.
- **`make`**: Builds and manages dependencies for software projects. Automate the build process.
- **`gcc`**: GNU Compiler Collection for compiling C, C++, and other languages. Compile source code into executable files.
- **`docker`**: Manages Docker containers. Run applications in isolated environments.
- **`kubectl`**: Manages Kubernetes clusters. Deploy and manage containerised applications at scale.

## Disk Management
- **`fdisk`**: Manipulates disk partition tables. Create, delete, or modify disk partitions.
- **`parted`**: A more advanced tool for managing disk partitions. Resize, create, and manage partitions.
- **`mkfs`**: Creates a filesystem on a partition. Prepare a partition for use.

## User Management
- **`useradd`**: Creates a new user account. Manage user access to the system.
- **`usermod`**: Modifies user account details. Adjust user privileges or details.
- **`passwd`**: Updates a user’s password. Secure user accounts.
- **`groupadd`**: Creates a new user group. Manage groups of users.
- **`groups`**: Shows the groups a user belongs to. Check user permissions based on group membership.
