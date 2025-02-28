# Linux for DevOps

## Overview
This repository documents essential Linux commands and concepts that are crucial for DevOps practices. These commands and topics will help you navigate the Linux environment, manage files, processes, permissions, and automate tasks effectively.

---

## Table of Contents
1. [Why Linux is Important for DevOps](#why-linux-is-important-for-devops)
2. [File and Directory Management](#file-and-directory-management)
3. [File Permissions and Ownership](#file-permissions-and-ownership)
4. [Process Management](#process-management)
5. [Networking Commands](#networking-commands)
6. [System Monitoring](#system-monitoring)
7. [Package Management](#package-management)
8. [User Management](#user-management)
9. [Disk Usage and Storage](#disk-usage-and-storage)
10. [Automation (Cron Jobs)](#automation-cron-jobs)

---

## Why Linux is Important for DevOps
Linux plays a critical role in the DevOps ecosystem due to its flexibility, reliability, and extensive use in modern infrastructure. Here are some key reasons why Linux is essential for DevOps:

### 1. **Linux Powers the Cloud**
- Most cloud platforms like AWS, Google Cloud, and Azure run on Linux-based environments.
- Knowledge of Linux is crucial for managing cloud infrastructure effectively.

### 2. **Server Management**
- DevOps engineers frequently manage Linux servers for deploying and maintaining applications.
- Tasks such as configuring servers, managing processes, and ensuring uptime are easier with Linux.

### 3. **Containerization and Orchestration**
- Tools like Docker and Kubernetes rely on Linux features such as cgroups and namespaces to function.
- Understanding Linux helps in working with containerized applications and orchestrating them at scale.

### 4. **Automation and Scripting**
- Linux provides powerful scripting capabilities (e.g., Bash, Python) to automate repetitive tasks like deployments, backups, and monitoring.
- Many configuration management tools (e.g., Ansible, Puppet) are designed to work seamlessly with Linux.

### 5. **Open Source Ecosystem**
- A vast majority of DevOps tools (e.g., Jenkins, GitLab CI/CD) are open-source and optimized for Linux environments.
- The open-source nature of Linux allows customization to meet specific DevOps requirements.

### 6. **Security and Reliability**
- Linux is known for its robust security features, making it a preferred choice for production systems.
- Its stability ensures high availability of critical applications.

### 7. **Cost Efficiency**
- Being free to use, Linux reduces operational costs compared to proprietary operating systems.

---

## File and Directory Management
| Command | Description |
|---------|-------------|
| `ls`    | Lists files and directories in the current directory. Use `ls -a` to show hidden files and `ls -l` for detailed information. |
| `cd`    | Changes the current working directory. Use `cd /path/to/directory` to navigate to a specific directory. |
| `pwd`   | Prints the current working directory path. |
| `mkdir` | Creates a new directory. Example: `mkdir new_folder`. |
| `rm`    | Deletes files or directories. Use `rm -r` to delete directories recursively. |
| `cp`    | Copies files or directories. Example: `cp file1 file2 /target/directory`. |
| `mv`    | Moves or renames files or directories. Example: `mv file1 /new/path`. |
| `touch` | Creates an empty file. Example: `touch newfile.txt`. |

---

## File Permissions and Ownership
| Command   | Description |
|-----------|-------------|
| `chmod`   | Changes file permissions (read, write, execute). Example: `chmod 755 file`. |
| `chown`   | Changes file ownership (user and group). Example: `chown user:group file`. |
| `umask`   | Sets default permissions for newly created files and directories. |

---

## Process Management
| Command   | Description |
|-----------|-------------|
| `ps`      | Displays information about running processes. Use `ps -aux` for detailed output. |
| `top`     | Shows real-time system processes and resource usage. |
| `kill`    | Terminates a process by its PID (Process ID). Example: `kill 1234`. |
| `jobs`    | Lists background jobs in the current terminal session. |
| `bg`      | Resumes a job in the background. Example: `bg %1`. |
| `fg`      | Brings a background job to the foreground. Example: `fg %1`. |

---

## Networking Commands
| Command    | Description |
|------------|-------------|
| `ping`     | Tests connectivity to another host or IP address. Example: `ping google.com`. |
| `ifconfig` | Displays or configures network interfaces (deprecated, use `ip addr`). |
| `netstat`  | Displays network connections, routing tables, etc. Use alternative: `ss`. |
| `curl`     | Transfers data from or to a server using protocols like HTTP/HTTPS/FTP. |

---

## System Monitoring
| Command     | Description |
|-------------|-------------|
| `df`        | Displays disk space usage of file systems. Example: `df -h`. |
| `du`        | Shows disk usage of files and directories. Example: `du -sh folder_name`. |
| `uptime`    | Displays system uptime and load averages. |
| `free`      | Shows memory usage (RAM). Example: `free -h`. |

---

## Package Management
### Debian-based Systems (Ubuntu):
- **Update package list**:

     sudo apt update
- **Install a package**:
  
     sudo apt install package_name
- **Remove a package**:  

     sudo apt remove package_name
### Red Hat-based Systems (CentOS):
- **Install a package**:  

     sudo yum install package_name
- **Remove a package**:  

     sudo yum remove package_name
  
---

## User Management
| Command      | Description |
|--------------|-------------|
| `adduser`    | Adds a new user to the system. Example: `sudo adduser username`. |
| `passwd`     | Changes the password for a user account. Example: `passwd username`. |
| `whoami`     | Displays the current logged-in user name. |

---

## Disk Usage and Storage
| Command     | Description |
|-------------|-------------|
| `mount`     | Mounts a device to the file system. Example: `mount /dev/sda1 /mnt`. |
| `umount`    | Unmounts a device from the file system. Example: `umount /mnt`. |

---

## Automation (Cron Jobs)
### Cron Syntax:

* * * * * command_to_execute

- First field: Minute (0–59)
- Second field: Hour (0–23)
- Third field: Day of Month (1–31)
- Fourth field: Month (1–12)
- Fifth field: Day of Week (0–6, Sunday = 0)

### Examples:
- Run a script every day at midnight:

0 0 * * * /path/to/script.sh


---

## Resources
- [Linux Commands Handbook](https://www.freecodecamp.org/news/the-linux-commands-handbook/)
- [DigitalOcean Linux Tutorials](https://www.digitalocean.com/community/tutorials/linux-commands)
- [Hostinger Linux Cheat Sheet](https://www.hostinger.com/tutorials/linux-commands)

Feel free to explore the examples in this repository to deepen your understanding of these commands.


