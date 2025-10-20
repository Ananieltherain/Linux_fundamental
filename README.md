# Linux_fundamental

## Dasar-dasar linux & file system

### pengenalan parrot os & command line:
- pwd > Lihat direktori saat ini
- ls > Lihat files
- cd > Change directory
- whoami > Lihat user saat ini
- uname -a > Info system

### File system hierarchy:
- ls -la > Lihat root directory
- cd/etc > Konfigurasi system
- cd/var > Variabel files
- cd/home > User directory
- cd/usr > User programs

  Manipulasi file && directory:
- mkdir > Membuat directory
- rmdir > Menghapus directory
- touch > Membuat file
- cp > Copy
- mv > Move/cut
- rm > Delete
- nano > Edit file
- cat > Baca file
  
## Manajemen Sistem & Permission

### User Management
- sudo su > Switch to root
- adduser > Add user
- passwd > Ganti password

### File Permission
- chmod > Ubah permission
- chown > Ubah ownership
- chgrp > Ubah group
- ls -l > Lihat permission

### Proccess Management
- ps aux > lihat semua proccess
- top > Monitor ressources
- kill > Terminate proccess
- pkill > Kill by name

### Package Manajemen
- sudo apt update > update
- sudo apt upgrade > upgrade
- sudo apt install [package] > Install package
- sudo apt remove [package] > Uninstall package


### Networking Fundamental:
- ifconfig > Network interfaces
- ping > Test connectvity
- netstat > Network statistic
- Ss > Socket statistic
- route > Routing table

### Powerfull text manipulation
- grep
- awk
- sed
- cut
- sort
- uniq

### Shell Scripting Dasar:
buat script sederhana:
#!/bin/bash
echo "Hello World"
variables, loops, conditions.


### Security Tools Built-in:
- iptables > firewall
- sryptsetup > Encryption
- auditd > Auditing
- fail2ban > Protection

### System Monitoring
- journalctl > systems log
- /var/logs > Log dirrectory
- lsof > list open files
- Strace > System calls

### Automation & Customitation:
buat bash env
.bashbrc customitation
alias creation
function script
scheduled task (cron)

### Tools sec bawaan Parrot:
- sudo parrot-updater > update system
- anonsurf > Anonymization
- aircrack-ng suite > wireless tools
- etc.
