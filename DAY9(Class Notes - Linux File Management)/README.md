Module 02 – Linux Filesystem
Student Task Guide (Day 09)
Based on Linux Filesystem class notes and lab discussions. May 17th, 2026

Table of Contents
Task	Title
1	Understanding the Linux Filesystem
2	Explore the Root Filesystem
3	Understanding Linux Users and Prompts
4	Install and Use the tree Command
5	Linux Filesystem Layers
6	Practice the ls Command
7	Understanding Metadata and Inodes
8	Filesystem Snapshot Activity
9	Absolute vs Relative Paths
10	Linux Boot Process
11	Explore the /boot Directory
12	BIOS vs UEFI
13	POST and Hardware Checks
14	Bootloader and Kernel
15	Systemd Targets
16	Shutdown and Reboot Commands
17	Understanding /home
18	Understanding /dev
19	Block Devices vs Character Devices
20	TTY and Pseudo Terminals
21	Disk Commands Practice
22	Sensors in Linux
23	Understanding /etc
24	Understanding /var
25	Linux Logging System
26	Understanding logrotate
27	Final Reflection
Task 1 - Understanding the Linux Filesystem
Objective
Understand the Linux filesystem structure. Review the class notes.

Instructions
Answer the following from the class notes:

What is a filesystem?
What is the root directory /?
Why is Linux called a hierarchical filesystem?
What is the purpose of directories?
Task 2 - Explore the Root Filesystem
Objective
Learn important Linux directories.

Instructions
Review Notes to explain the purpose of:

/boot
/home
/etc
/dev
/var
/tmp
/usr
/proc
Task 3 - Understanding Linux Users and Prompts
Objective
Understand different types of users:

root user
sudo user
regular/normal user
Instructions
Observe the shell prompts "#" and "$"

Examples:

[root@hostname ~]#
[user@hostname ~]$ sudo
[tester@hostname ~]$ 
Questions
Difference between root and regular user?
What is sudo?
Which symbol represents the root user?
Which symbol represents a normal user?
Task 4 - Install and Use the tree Command
Objective
Visualize directory structures.

Instructions
Install tree:

dnf install tree -y
Run:

tree -d /boot
tree /boot
tree -a -L 2 -h -C
Questions
What does tree -d show?
What does -L 2 mean?
Why is the tree command useful?
Task 5 - Linux Filesystem Layers
Objective
Understand filesystem architecture.

Instructions
Research the following:

Logical File System
Virtual File System (VFS)
Physical File System
Questions
What is VFS?
Why is /proc/cpuinfo considered virtual data?
Task 6 - Practice the ls Command
Objective
Learn file listing commands.

Instructions
Run:

ll
ls -l /
ls -ld /
ls -al /
ls -il /
Questions
Difference between ls -l / and ls -ld /?
What does -i display?
What is metadata?
Task 7 - Understanding Metadata and Inodes
Objective
Understand how Linux tracks files.

Instructions
Research:

Metadata
Inodes
Questions
What information does an inode store?
Does an inode store file data?
Why are inodes important?
Commands
Run:

df -i
ls -il
stat /boot
Task 8 - Filesystem Snapshot Activity
Objective
Understand the Linux filesystem tree.

Instructions
Draw the Linux filesystem hierarchy.

Include:

/
/boot
/home
/etc
/dev
/usr
/var
/tmp
Task 9 - Absolute vs Relative Paths
Objective
Understand navigation in Linux.

Instructions
Practice:

pwd
cd /home
cd ..
cd .
Questions
What is an absolute path?
What is a relative path?
Practice one example of each.
Task 10 - Linux Boot Process
Objective
Introduce where Boot system files are located. The booting process will be discussed in detail in a seperate "Linux Boot Process" class

Question
What happens if the bootloader is corrupted? This is a real world problem. We will address this question when we learn about Boot Process in the future

Task 11 - Explore the /boot Directory
Objective
Understand boot-related files.

Instructions
Run:

ls -l /boot
tree -d /boot
Questions
Find and explain:

grub.cfg
initramfs
vmlinuz
System.map
Task 12 - BIOS vs UEFI
Objective
These slides were added to give you all clarity

Task 13 - POST and Hardware Checks
Objective
Understand POST.

Questions
What does POST check?

CPU
RAM
Storage
Keyboard
GPU
Bonus
What happens if RAM fails during POST?

Task 14 - Bootloader and Kernel
Objective
We will learn in detail about GRUB and Kernel.

Task 15 - Systemd Targets
Objective
We will learn later in this course about Linux targets and runlevels.

Task 16 - Shutdown and Reboot Commands
Objective
Practice power management commands.

Instructions
Research the following:

systemctl reboot
shutdown -r now
systemctl poweroff
Questions
Difference between reboot and poweroff?
What does shutdown -c do?
Task 17 - Understanding /home
Objective
Understand user home directories.

Questions
What is the purpose of /home?
Where does a user land after login?
Why are initialization files important?
Task 18 - Understanding /dev
Objective
Learn about device files.

Instructions
Run:

ls /dev
ls -l /dev/sda1
Questions
Why is everything treated as a file in Linux?
What is /dev/sda?
What is udev?
Task 19 - Block Devices vs Character Devices
Objective
Understand Linux device types.

Questions
Just appreciate that there is a difference between block devices and character devices?
Hard Drives and block devices.
Task 20 - TTY and Pseudo Terminals
Objective
Understand Linux terminals.

Instructions
Run:

tty
w
who
ls /dev/pts
Questions
What is tty1?
What is pts/0?
What does the w command display?
Task 21 - Disk Commands Practice
Objective
Practice storage commands.

Instructions
Run:

df -hT
lsblk
fdisk -l
Task 22 - Sensors in Linux
Objective
Monitor hardware sensors.

Instructions
Install sensors:

dnf install lm_sensors -y
Run:

sensors-detect
sensors
Questions
What does lm_sensors do?
Why are sensors important in data centers?
Task 23 - Understanding /etc
Objective
Understand Linux configuration files.

Instructions
Run:

ls /etc
Questions
We will learn how User information is managed by Linux later in this course:

/etc/passwd
/etc/shadow
/etc/group
/etc/sudoers
Bonus
Why should /etc always be backed up?

Task 24 - Understanding /var
Objective
Understand variable data storage.

Instructions
Run:

ls /var
Questions
Research:

/var/log
/var/cache
/var/tmp
/var/spool
Question
Why can /var grow very large?

Task 25 - Linux Logging System
Objective
Understand Linux logs.

Instructions
Run:

journalctl
tail -f /var/log/messages
Questions
Difference between rsyslog and journald?
What does journalctl do?
Where are logs stored?
Task 26 - Understanding logrotate
Objective
Introduction to log management.

Instructions
Run:

cat /etc/logrotate.conf
ls /etc/logrotate.d/
Questions
What is logrotate?
Why is log rotation important?
What happens if logs are never rotated?
Task 27 - Final Reflection
Objective
Reflect on your learning.

Instructions
Write a short paragraph answering:

What did you learn in Module 02?
Which Linux directory was most interesting?
Which command was most useful?
Which topic was difficult?
What would you like to practice more?
