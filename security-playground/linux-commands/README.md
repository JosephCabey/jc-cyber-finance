# Linux Shell Command Cheat Sheet 🐧

This section contains a curated list of essential Linux shell commands for cybersecurity and system administration tasks. These are the tools I’m learning and applying in projects related to system hardening, log inspection, and incident response.

---

## 🔐 Security & Permissions

| Command                      | Description                                |
|-----------------------------|--------------------------------------------|
| `chmod`                     | Change file permissions                    |
| `chown`                     | Change file owner                          |
| `ls -l`                     | List files with permissions                |
| `umask`                     | Set default file permission                |
| `sudo`                      | Execute command as another user (admin)    |

---

## 📁 File & Directory Management

| Command                      | Description                                |
|-----------------------------|--------------------------------------------|
| `ls`, `ls -a`               | List directory contents                    |
| `cd`, `pwd`                 | Navigate directories                       |
| `mkdir`, `rmdir`            | Create/delete directories                  |
| `cp`, `mv`, `rm`            | Copy, move, remove files                   |
| `find / -name filename`     | Search for files                           |

---

## 📄 File Viewing & Editing

| Command                      | Description                                |
|-----------------------------|--------------------------------------------|
| `cat`, `less`, `more`       | View contents of a file                    |
| `head`, `tail -n 100`       | View first/last lines of a file           |
| `nano`, `vim`               | Edit files                                 |
| `touch`                     | Create an empty file                       |

---

## 🔍 System Monitoring

| Command                      | Description                                |
|-----------------------------|--------------------------------------------|
| `top`, `htop`               | View running processes                     |
| `ps aux`                    | Show all running processes                 |
| `df -h`                     | Check disk space usage                     |
| `free -m`                   | View memory usage                          |
| `uptime`, `who`             | Show system info                           |

---

## 🌐 Networking

| Command                      | Description                                |
|-----------------------------|--------------------------------------------|
| `ip a`, `ifconfig`          | Show IP and network interfaces             |
| `ping`, `traceroute`        | Test network connection                    |
| `netstat -tulpn`            | Show active ports                          |
| `ss -tuln`                  | List listening ports                       |
| `curl`, `wget`              | Retrieve web content                       |

---

## 🧰 Log Management

| Command                      | Description                                |
|-----------------------------|--------------------------------------------|
| `tail -f /var/log/syslog`   | Monitor live logs                          |
| `grep "error" /var/log/*`   | Search for errors in logs                  |
| `journalctl -xe`            | View systemd logs                          |

---

## 💡 Other Useful Tips

- Use `man [command]` to learn more about any command.
- Combine commands using `|` (pipes) and `>` (redirects).

---

> “Mastering the command line is like unlocking the hidden powers of the system.”


