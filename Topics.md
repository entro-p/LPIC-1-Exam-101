Topic 101: System Architecture101.1 Determine and configure hardware settingsWeight: 2

Description: Candidates should be able to determine and configure fundamental system hardware.

Key Knowledge Areas:

Tools and utilities to list various hardware information (e.g. lsusb, lspci, etc.)
Tools and utilities to manipulate USB devices
Conceptual understanding of sysfs, udev, dbus
The following is a partial list of the used files, terms and utilities:

/sys/
/proc/
/dev/
modprobe
lsmod
lspci
lsusb
 

101.2 Boot the systemWeight: 3

Description: Candidates should be able to guide the system through the booting process.

Key Knowledge Areas:

Provide common commands to the boot loader and options to the kernel at boot time
Demonstrate knowledge of the boot sequence from BIOS to boot completion
Understanding of SysVinit and systemd
Awareness of Upstart
Check boot events in the log files
Terms and Utilities:

dmesg
BIOS
bootloader
kernel
initramfs
init
SysVinit
systemd
 

101.3 Change runlevels / boot targets and shutdown or reboot systemWeight: 3

Description: Candidates should be able to manage the SysVinit runlevel or systemd boot target of the system. This objective includes changing to single user mode, shutdown or rebooting the system. Candidates should be able to alert users before switching runlevels / boot targets and properly terminate processes. This objective also includes setting the default SysVinit runlevel or systemd boot target. It also includes awareness of Upstart as an alternative to SysVinit or systemd.

Key Knowledge Areas:

Set the default runlevel or boot target
Change between runlevels / boot targets including single user mode
Shutdown and reboot from the command line
Alert users before switching runlevels / boot targets or other major system events
Properly terminate processes
Terms and Utilities:

/etc/inittab
shutdown
init
/etc/init.d/
telinit
systemd
systemctl
/etc/systemd/
/usr/lib/systemd/
wall
Topic 102: Linux Installation and Package Management102.1 Design hard disk layoutWeight: 2

Description: Candidates should be able to design a disk partitioning scheme for a Linux system.

Key Knowledge Areas:

Allocate filesystems and swap space to separate partitions or disks
Tailor the design to the intended use of the system
Ensure the /boot partition conforms to the hardware architecture requirements for booting
Knowledge of basic features of LVM
Terms and Utilities:

/ (root) filesystem
/var filesystem
/home filesystem
/boot filesystem
swap space
mount points
partitions
 102.2 Install a boot managerWeight: 2

Description: Candidates should be able to select, install and configure a boot manager.

Key Knowledge Areas:

Providing alternative boot locations and backup boot options
Install and configure a boot loader such as GRUB Legacy
Perform basic configuration changes for GRUB 2
Interact with the boot loader
The following is a partial list of the used files, terms and utilities:

menu.lst, grub.cfg and grub.conf
grub-install
grub-mkconfig
MBR
 

102.3 Manage shared librariesWeight: 1

Description: Candidates should be able to determine the shared libraries that executable programs depend on and install them when necessary.

Key Knowledge Areas:

Identify shared libraries
Identify the typical locations of system libraries
Load shared libraries
Terms and Utilities:

ldd
ldconfig
/etc/ld.so.conf
LD_LIBRARY_PATH
 

102.4 Use Debian package managementWeight: 3

Description: Candidates should be able to perform package management using the Debian package tools.

Key Knowledge Areas:

Install, upgrade and uninstall Debian binary packages
Find packages containing specific files or libraries which may or may not be installed
Obtain package information like version, content, dependencies, package integrity and installation status (whether or not the package is installed)
Terms and Utilities:

/etc/apt/sources.list
dpkg
dpkg-reconfigure
apt-get
apt-cache
aptitude
 

102.5 Use RPM and YUM package managementWeight: 3

Description: Candidates should be able to perform package management using RPM and YUM tools.

Key Knowledge Areas:

Install, re-install, upgrade and remove packages using RPM and YUM
Obtain information on RPM packages such as version, status, dependencies, integrity and signatures
Determine what files a package provides, as well as find which package a specific file comes from
Terms and Utilities:

rpm
rpm2cpio
/etc/yum.conf
/etc/yum.repos.d/
yum
yumdownloader
Topic 103: GNU and Unix Commands103.1 Work on the command lineWeight: 4

Description: Candidates should be able to interact with shells and commands using the command line. The objective assumes the Bash shell.

Key Knowledge Areas:

Use single shell commands and one line command sequences to perform basic tasks on the command line
Use and modify the shell environment including defining, referencing and exporting environment variables
Use and edit command history
Invoke commands inside and outside the defined path
Terms and Utilities:

bash
echo
env
export
pwd
set
unset
man
uname
history
.bash_history
 

103.2 Process text streams using filtersWeight: 3

Description: Candidates should be able to apply filters to text streams.

Key Knowledge Areas:

Send text files and output streams through text utility filters to modify the output using standard UNIX commands found in the GNU textutils package

Terms and Utilities:

cat
cut
expand
fmt
head
join
less
nl
od
paste
pr
sed
sort
split
tail
tr
unexpand
uniq
wc
 

103.3 Perform basic file managementWeight: 4

Description: Candidates should be able to use the basic Linux commands to manage files and directories.

Key Knowledge Areas:

Copy, move and remove files and directories individually
Copy multiple files and directories recursively
Remove files and directories recursively
Use simple and advanced wildcard specifications in commands
Using find to locate and act on files based on type, size, or time
Usage of tar, cpio and dd
Terms and Utilities:

cp
find
mkdir
mv
ls
rm
rmdir
touch
tar
cpio
dd
file
gzip
gunzip
bzip2
xz
file globbing
 

103.4 Use streams, pipes and redirectsWeight: 4

Description: Candidates should be able to redirect streams and connect them in order to efficiently process textual data. Tasks include redirecting standard input, standard output and standard error, piping the output of one command to the input of another command, using the output of one command as arguments to another command and sending output to both stdout and a file.

Key Knowledge Areas:

Redirecting standard input, standard output and standard error
Pipe the output of one command to the input of another command
Use the output of one command as arguments to another command
Send output to both stdout and a file
Terms and Utilities:

tee
xargs
 

103.5 Create, monitor and kill processesWeight: 4

Description: Candidates should be able to perform basic process management.

Key Knowledge Areas:

Run jobs in the foreground and background
Signal a program to continue running after logout
Monitor active processes
Select and sort processes for display
Send signals to processes
Terms and Utilities:

&
bg
fg
jobs
kill
nohup
ps
top
free
uptime
pgrep
pkill
killall
screen
 

103.6 Modify process execution prioritiesWeight: 2

Description: Candidates should should be able to manage process execution priorities.

Key Knowledge Areas:

Know the default priority of a job that is created
Run a program with higher or lower priority than the default
Change the priority of a running process
Terms and Utilities:

nice
ps
renice
top
 

103.7 Search text files using regular expressionsWeight: 2

Description: Candidates should be able to manipulate files and text data using regular expressions. This objective includes creating simple regular expressions containing several notational elements. It also includes using regular expression tools to perform searches through a filesystem or file content.

Key Knowledge Areas:

Create simple regular expressions containing several notational elements
Use regular expression tools to perform searches through a filesystem or file content
Terms and Utilities:

grep
egrep
fgrep
sed
regex(7)
 

103.8 Perform basic file editing operations using viWeight: 3

Description: Candidates should be able to edit text files using vi. This objective includes vi navigation, basic vi modes, inserting, editing, deleting, copying and finding text.

Key Knowledge Areas:

Navigate a document using vi
Use basic vi modes
Insert, edit, delete, copy and find text
Terms and Utilities:

vi
/, ?
h,j,k,l
i, o, a
c, d, p, y, dd, yy
ZZ, :w!, :q!, :e!
Topic 104: Devices, Linux Filesystems, Filesystem Hierarchy Standard104.1 Create partitions and filesystemsWeight: 2

Description: Candidates should be able to configure disk partitions and then create filesystems on media such as hard disks. This includes the handling of swap partitions.

Key Knowledge Areas:

Manage MBR partition tables
Use various mkfs commands to create various filesystems such as:
ext2/ext3/ext4
XFS
VFAT
Awareness of ReiserFS and Btrfs
Basic knowledge of gdisk and parted with GPT
Terms and Utilities:

fdisk
gdisk
parted
mkfs
mkswap
 

104.2 Maintain the integrity of filesystemsWeight: 2

Description: Candidates should be able to maintain a standard filesystem, as well as the extra data associated with a journaling filesystem.

Key Knowledge Areas:

Verify the integrity of filesystems
Monitor free space and inodes
Repair simple filesystem problems
Terms and Utilities:

du
df
fsck
e2fsck
mke2fs
debugfs
dumpe2fs
tune2fs
XFS tools (such as xfs_metadump and xfs_info)
 

104.3 Control mounting and unmounting of filesystemsWeight: 3

Description: Candidates should be able to configure the mounting of a filesystem.

Key Knowledge Areas:

Manually mount and unmount filesystems
Configure filesystem mounting on bootup
Configure user mountable removable filesystems
Terms and Utilities:

/etc/fstab
/media/
mount
umount
 

104.4 Manage disk quotasWeight: 1

Description: Candidates should be able to manage disk quotas for users.

Key Knowledge Areas:

Set up a disk quota for a filesystem
Edit, check and generate user quota reports
Terms and Utilities:

quota
edquota
repquota
quotaon
 

104.5 Manage file permissions and ownershipWeight: 3

Description: Candidates should be able to control file access through the proper use of permissions and ownerships.

Key Knowledge Areas:

Manage access permissions on regular and special files as well as directories
Use access modes such as suid, sgid and the sticky bit to maintain security
Know how to change the file creation mask
Use the group field to grant file access to group members
Terms and Utilities:

chmod
umask
chown
chgrp
 

104.6 Create and change hard and symbolic linksWeight: 2

Description: Candidates should be able to create and manage hard and symbolic links to a file.

Key Knowledge Areas:

Create links
Identify hard and/or soft links
Copying versus linking files
Use links to support system administration tasks
Terms and Utilities:

ln
ls
 

104.7 Find system files and place files in the correct locationWeight: 2

Description: Candidates should be thoroughly familiar with the Filesystem Hierarchy Standard (FHS), including typical file locations and directory classifications.

Key Knowledge Areas:

Understand the correct locations of files under the FHS
Find files and commands on a Linux system
Know the location and purpose of important file and directories as defined in the FHS
Terms and Utilities:

find
locate
updatedb
whereis
which
type
/etc/updatedb.conf
