# Linux Common Commands Cheat Sheet

## 1. Navigation

| Command | Description |
|---------|-------------|
| `pwd` | Show current working directory |
| `ls` | List files and directories |
| `ls -l` | Detailed list |
| `ls -la` | Show hidden files |
| `cd directory` | Change directory |
| `cd ..` | Go to parent directory |
| `cd ~` | Go to home directory |
| `clear` | Clear terminal |
| `tree` | Display directory tree |

---

## 2. File & Directory Management

| Command | Description |
|---------|-------------|
| `touch file.txt` | Create a new file |
| `mkdir folder` | Create directory |
| `mkdir -p folder/subfolder` | Create nested directories |
| `rm file.txt` | Remove file |
| `rm -r folder` | Remove directory recursively |
| `rm -rf folder` | Force remove directory |
| `cp source destination` | Copy file |
| `cp -r source destination` | Copy directory |
| `mv old new` | Move or rename file |
| `ln -s target shortcut` | Create symbolic link |

---

## 3. Viewing Files

| Command | Description |
|---------|-------------|
| `cat file.txt` | Display file contents |
| `less file.txt` | View file page by page |
| `more file.txt` | View file page by page |
| `head file.txt` | First 10 lines |
| `head -20 file.txt` | First 20 lines |
| `tail file.txt` | Last 10 lines |
| `tail -f logfile.log` | Monitor file in real time |
| `nl file.txt` | Show file with line numbers |

---

## 4. Searching

| Command | Description |
|---------|-------------|
| `find / -name filename` | Search file by name |
| `find . -type f` | Find all files |
| `find . -type d` | Find all directories |
| `locate filename` | Quickly locate file |
| `which command` | Find executable path |
| `whereis command` | Locate binary, source and manual |
| `grep "text" file.txt` | Search text |
| `grep -r "text" .` | Recursive search |

---

## 5. File Permissions

| Command | Description |
|---------|-------------|
| `chmod 755 file` | Change permissions |
| `chmod +x script.sh` | Make executable |
| `chown user file` | Change owner |
| `chown user:group file` | Change owner and group |
| `chgrp group file` | Change group |
| `umask` | Display default permissions |

---

## 6. User Management

| Command | Description |
|---------|-------------|
| `whoami` | Current user |
| `who` | Logged-in users |
| `w` | Show logged-in users and activity |
| `id` | User information |
| `passwd` | Change password |
| `sudo command` | Execute as root |
| `su` | Switch user |

---

## 7. Process Management

| Command | Description |
|---------|-------------|
| `ps` | Running processes |
| `ps aux` | List all processes |
| `top` | Process monitor |
| `htop` | Interactive process monitor |
| `kill PID` | Kill process |
| `kill -9 PID` | Force kill process |
| `pkill process_name` | Kill by process name |
| `jobs` | Show background jobs |
| `bg` | Resume in background |
| `fg` | Bring to foreground |

---

## 8. Disk Usage

| Command | Description |
|---------|-------------|
| `df -h` | Disk usage |
| `du -sh folder` | Directory size |
| `du -ah` | File sizes |
| `lsblk` | Block devices |
| `fdisk -l` | Partition table |
| `mount` | Mount filesystem |
| `umount` | Unmount filesystem |

---

## 9. Memory Information

| Command | Description |
|---------|-------------|
| `free -h` | Memory usage |
| `vmstat` | Virtual memory statistics |
| `swapon --show` | Show swap usage |

---

## 10. Networking

| Command | Description |
|---------|-------------|
| `ip a` | Show IP addresses |
| `ip r` | Routing table |
| `ping google.com` | Test connectivity |
| `traceroute google.com` | Trace route |
| `ss -tuln` | Listening ports |
| `netstat -tulnp` | Network connections |
| `curl https://example.com` | Fetch webpage |
| `wget https://example.com/file` | Download file |
| `dig google.com` | DNS lookup |
| `nslookup google.com` | DNS lookup |

---

## 11. System Information

| Command | Description |
|---------|-------------|
| `uname -a` | Kernel information |
| `hostname` | Hostname |
| `hostnamectl` | Host information |
| `uptime` | System uptime |
| `date` | Current date and time |
| `timedatectl` | Time settings |
| `lscpu` | CPU information |
| `lspci` | PCI devices |
| `lsusb` | USB devices |

---

## 12. Package Management (APT)

| Command | Description |
|---------|-------------|
| `sudo apt update` | Update package list |
| `sudo apt upgrade` | Upgrade packages |
| `sudo apt install package` | Install package |
| `sudo apt remove package` | Remove package |
| `sudo apt autoremove` | Remove unused packages |
| `dpkg -l` | List installed packages |

---

## 13. Compression

| Command | Description |
|---------|-------------|
| `zip archive.zip file` | Create ZIP |
| `unzip archive.zip` | Extract ZIP |
| `tar -cvf archive.tar folder` | Create TAR |
| `tar -xvf archive.tar` | Extract TAR |
| `tar -czvf archive.tar.gz folder` | Create compressed TAR |
| `tar -xzvf archive.tar.gz` | Extract compressed TAR |

---

## 14. Logs

| Command | Description |
|---------|-------------|
| `journalctl` | View system logs |
| `journalctl -xe` | View recent errors |
| `dmesg` | Kernel logs |
| `tail -f /var/log/syslog` | Monitor system log |
| `tail -f /var/log/auth.log` | Monitor authentication log |

---

## 15. Services

| Command | Description |
|---------|-------------|
| `systemctl status service` | Service status |
| `systemctl start service` | Start service |
| `systemctl stop service` | Stop service |
| `systemctl restart service` | Restart service |
| `systemctl enable service` | Enable at boot |
| `systemctl disable service` | Disable at boot |

---

## 16. File Editing

| Command | Description |
|---------|-------------|
| `nano file.txt` | Edit with Nano |
| `vim file.txt` | Edit with Vim |
| `echo "text"` | Print text |
| `echo "Hello" > file.txt` | Overwrite file |
| `echo "Hello" >> file.txt` | Append to file |

---

## 17. Security & Administration

| Command | Description |
|---------|-------------|
| `history` | Command history |
| `sudo -l` | View sudo privileges |
| `groups` | User groups |
| `last` | Login history |
| `lastlog` | Last login |
| `crontab -l` | List cron jobs |
| `crontab -e` | Edit cron jobs |
| `iptables -L` | Firewall rules |
| `ufw status` | Firewall status |
| `fail2ban-client status` | Fail2Ban status |

---

## 18. Checksums

| Command | Description |
|---------|-------------|
| `md5sum file` | MD5 checksum |
| `sha1sum file` | SHA-1 checksum |
| `sha256sum file` | SHA-256 checksum |

---

## 19. Keyboard Shortcuts

| Shortcut | Description |
|----------|-------------|
| `Ctrl + C` | Stop running process |
| `Ctrl + Z` | Suspend process |
| `Ctrl + D` | Exit shell |
| `Ctrl + L` | Clear screen |
| `Ctrl + R` | Search command history |
| `Ctrl + A` | Move to beginning of line |
| `Ctrl + E` | Move to end of line |
| `Tab` | Auto-complete |
| `↑ / ↓` | Previous/Next command |

---

# Useful Tips

- `man <command>` → Open the manual page for a command.
- `<command> --help` → Display command help and options.
- `history` → View previously executed commands.
- `!!` → Re-run the last command.
- `!n` → Run command number `n` from history.
- `sudo !!` → Re-run the previous command with `sudo`.
- `alias ll='ls -la'` → Create a shortcut command.