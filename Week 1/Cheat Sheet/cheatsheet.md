# Cheat Sheet – Linux Commands

| Command | What It Does | When to Use |
|---------|--------------|-------------|
| `ls` | List directory contents | Quick view of files
| `cd` | Change directory | Navigate filesystem
| `chmod` | Change file permissions | Adjust security settings
| `chown` | Change file owner/group | Reassign ownership
| `cat` | Concatenate and display file | View file content
| `grep` | Search text using patterns | Find strings in files
| `find` | Search for files/directories | Locate files by name/size
| `ps` | Display running processes | Check process status
| `ss -tulpn` | List listening sockets with programs | Identify open ports
| `cron` | Schedule recurring tasks | Automate scripts
| `tar` | Archive/compress files | Backup directories
| `apt-get` / `apt` | Package manager (Debian/Ubuntu) | Install/remove software
| `systemctl` | Manage system services | Start/stop services
| `ssh` | Secure remote login | Access remote machines
| `scp` | Secure copy files over SSH | Transfer files securely
| `wget` | Download files from web | Fetch resources
| `dig` | DNS lookup utility | Query DNS records
| `ip a` | Show network interfaces | Inspect IP configuration
| `iptables` | Manage firewall rules | Control traffic filtering
| `df -h` | Disk space usage | Monitor storage
| `du -sh` | Directory size summary | Check folder size
| `mount` | Mount filesystems | Attach devices
| `umount` | Unmount filesystems | Detach devices
| `rsync` | Sync files/directories | Backup or copy efficiently
| `nano`/`vim` | Text editors | Edit config/files
| `top`/`htop` | Real‑time process monitor | Observe resource usage
| `history` | Command history | Recall previous commands
| `sudo` | Execute as another user (root) | Run privileged commands
| `passwd` | Change user password | Update credentials
| `whoami` | Display current user | Verify effective user
| `uname -a` | System information | Identify OS/kernel
| `date` | Show/set system date | Log timestamps
| `sleep` | Delay execution | Wait in scripts
| `kill` | Send signal to process | Terminate a process
| `df -i` | Inode usage | Diagnose inode exhaustion
| `mount -o bind` | Bind mount | Share directories
| `chmod +t` | Sticky bit on directories | Secure shared tmp dirs
| `chattr +i` | Immutable attribute | Prevent file modification
| `ln -s` | Create symbolic link | Shortcut to files/dirs
| `sudo apt update && sudo apt upgrade -y` | Update system packages | Keep system patched
| `git clone` | Clone repository | Retrieve code
| `git pull` | Update local repo | Sync changes
| `git commit` | Record changes | Version control
| `ssh-keygen` | Generate SSH keys | Setup password‑less auth
| `fail2ban-client` | Manage fail2ban | Block brute‑force IPs
| `nc` (netcat) | Network utility | Test connectivity
| `traceroute` | Route tracing | Diagnose network paths
| `htpasswd` | Manage HTTP auth file | Simple web auth
| `systemd-analyze blame` | Boot time analysis | Identify slow services
| `journalctl -f` | Follow system logs | Real‑time log monitoring
| `useradd` | Create a new user | Add accounts
| `groupadd` | Create a new group | Organize permissions
| `passwd -l` | Lock user account | Temporarily disable login
| `ufw enable` | Enable uncomplicated firewall | Basic firewall setup
| `iptables -A INPUT -p tcp --dport 22 -j ACCEPT` | Allow SSH via iptables | Open specific port
| `lsof -i :80` | List processes using a port | Find service on port 80
| `rsyslog` | Syslog daemon | Centralized logging
| `tcpdump` | Capture packets | Network troubleshooting
| `nmcli` | NetworkManager CLI | Manage connections
| `systemctl status <service>` | Check service status | Verify running services
| `dpkg -l` | List installed packages | Inventory software
| `fd` | Faster alternative to find | Quickly locate files
| `bat` | Cat with syntax highlighting | Read code files
| `htop` | Interactive process viewer | Detailed resource usage
| `curl` | Transfer data with URLs | Test APIs
| `sudo sysctl -w net.ipv4.ip_forward=1` | Enable IP forwarding | Configure router functionality

*Add more entries as you encounter useful commands.*