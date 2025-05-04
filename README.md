# 🐧 Linux

## 📘 What is Linux?

Linux is a powerful, open-source operating system used on servers, desktops, embedded systems, and more. It gives users fine-grained control over system behavior, security, and performance through the command line interface (CLI).

---

## 🙋‍♂️ Who Should Use Linux?

- **Developers**: For programming, scripting, and tool integration.
- **System Administrators**: To manage servers, users, services, and filesystems.
- **Cybersecurity Enthusiasts**: For ethical hacking and securing systems.
- **Students & Tech Learners**: To understand computing fundamentals.
- **Everyday Users**: Looking for a fast, customizable, and secure OS.

---

## 🎯 Why Use Linux?

- 💡 Open-source and community-driven
- 🔒 Highly secure and privacy-friendly
- ⚡ Fast, lightweight, and customizable
- 💻 Ideal for development, scripting, automation
- 🌍 Widely used in servers, cloud, and mobile (Android)

---

## 💻 Basic File & Directory Commands

| Command | Description |
|---------|-------------|
| `ls` | 📂 List directory contents |
| `cd <dir>` | 🚶 Change directory |
| `pwd` | 📍 Show current directory path |
| `mkdir <dir>` | 🆕 Create new directory |
| `rmdir <dir>` | 🧹 Remove empty directory |
| `rm <file>` | 🗑️ Delete a file |
| `rm -r <dir>` | 🧨 Delete directory and contents |
| `cp <src> <dest>` | 📋 Copy files or directories |
| `mv <src> <dest>` | 🚚 Move or rename files/directories |
| `touch <file>` | 📄 Create empty file |
| `cat <file>` | 📖 Display file content |
| `less <file>` | 📚 View file page by page |
| `file <file>` | 🔍 Detect file type |

---

## 🔍 Searching & Finding Files

| Command | Description |
|---------|-------------|
| `find /path -name "*.txt"` | 🔎 Find files by name |
| `locate <filename>` | 🗺️ Search indexed files |
| `grep "text" <file>` | 🔍 Search text in file |
| `grep -r "text" <dir>` | 🔍 Recursive search in directory |

---

## 📦 Package & Process Management

| Command | Description |
|---------|-------------|
| `top` | 📊 Show real-time system processes |
| `ps aux` | 📋 List all running processes |
| `kill <PID>` | ❌ Kill process by PID |
| `htop` | 🖥️ Interactive process viewer (if installed) |
| `sudo apt update` | 🔄 Update package lists (Debian/Ubuntu) |
| `sudo apt install <pkg>` | 📥 Install package |
| `sudo yum install <pkg>` | 📥 Install package (RHEL/CentOS) |

---

## 🛠️ System Information

| Command | Description |
|---------|-------------|
| `uname -a` | 🧠 Kernel and system info |
| `df -h` | 💽 Disk space usage |
| `du -sh <dir>` | 📦 Size of directory |
| `free -h` | 🧮 Memory usage |
| `uptime` | ⏳ System uptime |
| `whoami` | 🙋 Current username |
| `id` | 🆔 User and group IDs |

---

## 🧰 File Permissions

| Command | Description |
|---------|-------------|
| `chmod +x <file>` | 🛠️ Make file executable |
| `chown user:group <file>` | 👤 Change file owner |
| `ls -l` | 🔐 View permissions |
| `chmod 755 <file>` | 🔧 Set read-write-execute (owner) |

---

## 🌐 Networking

| Command | Description |
|---------|-------------|
| `ip a` | 🌐 Show IP addresses |
| `ping <host>` | 📶 Ping a host |
| `curl <url>` | 🌍 Fetch web data |
| `wget <url>` | ⬇️ Download file from URL |
| `netstat -tulpn` | 📡 List open ports and services |
| `ssh user@host` | 🔐 Remote login |

---

## 🗃️ Archives & Compression

| Command | Description |
|---------|-------------|
| `tar -cvf archive.tar <dir>` | 📦 Create tar archive |
| `tar -xvf archive.tar` | 📂 Extract tar archive |
| `gzip <file>` | 🗜️ Compress file |
| `gunzip <file.gz>` | 🔓 Decompress file |
| `zip <file.zip> <file>` | 🧳 Create zip archive |
| `unzip <file.zip>` | 📂 Extract zip archive |

---

## 🧠 Tip

💡 Use `man <command>` or `<command> --help` to explore more options and usage.

---

> ✅ Save this README as a Linux command reference.  
> ⭐ Star if it helped you become more fluent in the terminal!
