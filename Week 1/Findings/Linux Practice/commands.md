# Linux Practice – 30 Common Commands (output snapshots)

| # | Command | What It Does | Sample Output |
|---|---------|--------------|---------------|
| 1 | `pwd` | Print current working directory | `/home/user`
| 2 | `ls -la` | List all files with details | `drwxr-xr-x  5 user user 4096 Sep 10 12:00 .` ... |
| 3 | `cd /var/log` | Change directory to /var/log | *(no output)* |
| 4 | `cat /etc/hostname` | Show hostname file | `ubuntu-host`
| 5 | `grep "error" syslog` | Search for "error" in syslog | `Oct 24 12:01:23 host systemd[1]: Failed to start ...`
| 6 | `find /home -name "*.conf"` | Find all *.conf files under /home | `/home/user/.config/app.conf`
| 7 | `ps aux | grep nginx` | List nginx processes | `root  1234  0.0  0.1  123456  2345 ?  Ss 12:00 0:00 nginx: master process /usr/sbin/nginx`
| 8 | `ss -tulpn` | Show listening sockets with programs | `LISTEN 0 128 0.0.0.0:22 0.0.0.0:* users:("sshd",pid=567,fd=3)`
| 9 | `top -b -n 1 | head -5` | Snapshot of top processes | `top - 12:00:00 up 1 day,  3 users, load average: 0.07, 0.03, 0.01` ... |
|10| `df -h` | Disk usage in human‑readable form | `Filesystem      Size  Used Avail Use% Mounted on` ... |
|11| `du -sh ~/projects` | Size of projects directory | `2.4G    /home/user/projects`
|12| `free -h` | Memory usage | `Mem: 7.8G  3.2G  4.6G  210M  0%  1.9G`
|13| `uptime` | System uptime and load | ` 12:05:01 up 3 days,  4:23,  2 users,  load average: 0.12, 0.08, 0.05`
|14| `whoami` | Current user | `user`
|15| `date` | Current date/time | `Mon Oct 24 12:06:00 UTC 2026`
|16| `hostname -I` | IP addresses of host | `192.168.56.101`
|17| `ip a` | Show network interfaces | `2: enp0s3: <BROADCAST,MULTICAST,UP,LOWER_UP> ... inet 192.168.56.101/24 ...`
|18| `ping -c 3 8.8.8.8` | Ping Google DNS 3 times | `--- 8.8.8.8 ping statistics --- 3 packets transmitted, 3 received, 0% packet loss` |
|19| `traceroute 8.8.8.8` | Trace route to Google DNS | `1  192.168.56.1  1.123 ms ...`
|20| `dig @8.8.8.8 example.com A +short` | DNS query for A record | `93.184.216.34`
|21| `nslookup example.com` | DNS lookup utility | `Name:    example.com
Address: 93.184.216.34`
|22| `sudo apt update && sudo apt upgrade -y` | Update system packages | `Reading package lists... Done
... 0 upgraded, 0 newly installed, 0 to remove and 0 not upgraded.` |
|23| `sudo systemctl status ssh` | Service status for SSH | `● ssh.service - OpenBSD Secure Shell server
   Loaded: loaded (/lib/systemd/system/ssh.service; enabled; ...)` |
|24| `sudo systemctl restart ssh` | Restart SSH service | *(no output, service restarts)* |
|25| `chmod 750 /var/log/secure` | Change permissions on a log file | *(no output, returns to prompt)* |
|26| `chown root:adm /var/log/syslog` | Change owner/group of syslog | *(no output)* |
|27| `sudo useradd student1` | Create new user | *(no output)* |
|28| `sudo groupadd devteam` | Create new group | *(no output)* |
|29| `sudo usermod -aG devteam student1` | Add user to group | *(no output)* |
|30| `crontab -l` | List current cron jobs (after adding one) | `*/5 * * * * /home/user/scripts/backup.sh` |


