#Hardware /GPU

## Check GPU driver 
Command:
```bash
lspci -k | grep -EA3 'VGA|3d|Display'

## Shows current loaded drivers for GPU,Network,storage, etc
```bash
lsmod

## Show CPU info
```bash
lscpu

##Show memory info
```bash
free -h

##Show detailed hardware info
```bash
sudo lshw


#Disk/Storage

##list disk and partitioned
```bash
lsblk

##show detailed disk info
sudo fdisk-|

##show disk usage
df -h

##show inode usage
df -i

##Check disk read/write speed
sudo hdparm -Tt/dev/sda

#Network

##Show IP
ip a

##show routing table
ip route

##show listing port
ss -tuln

##test connectivity
ping google.com

##trace route to host
traceroute google.com

##check DNS resolution
nslookup google.com

##check network drive
lspci -k | grep -A3 Ethernet
lspci -k | grep -A3 Network


#System/packaged
##Update package list
sudo apt update

##upgrade installed packages
sudo apt upgrade -y

##install package
sudo apt install <package-name>

##remove package
sudo apt remove <package-name>

##remove a package completely
sudo apt purge <package-name>

##search for a package
apt search <package-name>

##show package info 
apt show <package-name>

#Users & permission
##show current user
whoami

##list all users
cat/etc/passwd

##check sudo privilages
sudo -|

##change file permission
chmod 755 filename

##change file ownership
chmod user:group filename

#Process and monitoring
##show running processes
ps aux

##interactive process viewer
htop

##Show memory usage
free -h


##Show disk usage per folder
du -h --max-depth=1

#show system uptime
uptime

#Files/Dir
##list files with details
ls -lah

##change directory
cd /path/to/folder

##copy files
cp source destination

#move or rename files
mv source destination

#delete files or directories
rm filename
rm -r foldername

#logs
##show system logs
journalctl -xe

##tail logs live
tail -f/var/log/syslog

##show kernel msg
dmesg | less

#Terminal
##clear terminal
clear

#show current shell
echo $SHELL

#show history
history


