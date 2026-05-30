Practice Lab – Linux Shell Basics
Date: 19th May, 2026 - Day 11

Table of Contents
Task	Title
1	What is a Linux Shell?
2	Linux Shells Available in Linux
3	Ways to Access the Linux Shell
4	Explore the Bash Shell
5	Explore the date Command
6	How to Get Help in Linux
7	Final Summary
Task 1: What is a Linux Shell?
A shell provides you with an interactive interface to the Unix/Linux based system. It gathers input from you and executes programs based on that input. When the program finishes executing, it displays that output.

Your Input -> Linux Shell -> Kernel Helps to Execute -> Output Display
A shell accepts human readable commands and translates them into something the kernel can understand and process.

A Shell provides you with an interface to the Unix/Linux based systems. It gathers input from you and executes programs based on that input. When a program finishes executing, it displays that program's output.

The shell accepts human readable commands and translates them into something the kernel can read and process.

Question
Use any simple sentence above and explain in your own words what you understood about the Linux Shell.

NOTE: This answer has to be included in your "Final Summary".

Task 2: What are some of the Shells Available in Linux?
Common Linux Shells
1. BASH (Bourne-Again Shell)
Most common shell in Linux
Open Source
Default shell in many Linux distributions
2. CSH (C Shell)
Syntax is similar to the C programming language
3. KSH (Korn Shell)
Created by David Korn at AT&T Bell Labs
Became the base for POSIX shell standards
4. TCSH
Enhanced version of the Berkeley UNIX C Shell (CSH)
Question
What is the most common shell you will use as a Linux System Administrator?

NOTE: This answer has to be included in your "Final Summary".

Task 3 - Different Ways to Access the Linux Shell
1. Through Secure Shell (SSH)
Examples:

PuTTY
Super PuTTY
MobaXterm
Guacamole
2. Through CMD Prompt Terminal
You can access Linux systems through Windows CMD or PowerShell.

3. Through a Console
Example:

Xen-Orchestra Console
Task 4: Explore the Bash Shell
Run:
# How many shells are available in your system?
cat /etc/shells
Expected Output:
/bin/sh
/bin/bash
/usr/bin/sh
/usr/bin/bash
Check Your Current Shell
Run:

echo $SHELL
Expected Output:
/bin/bash
Find the Process ID (PID) of Your Shell
Run:

ps $$
Example Output:
PID TTY      STAT   TIME COMMAND
17217 pts/0  Ss     0:00 -bash
NOTE: Your PID number will be different.

Task 5 - Explore the date Command in Linux
Run:
date
Example Output:
Mon May 18 11:36:58 PM CDT 2026
Check How the date Command Executes
Run:

whereis date
Example Output:
date: /usr/bin/date /usr/share/man/man1/date.1.gz
Explanation
This output tells you that the backend program /usr/bin/date is being executed to communicate with the Kernel.

Task 6: How to Get Help in Linux?
Using Linux Manual Pages
Run:

man date
Explanation
This command opens the manual page for the date command
You can exit the manual by pressing q on your keyboard
Example Output
NAME
       date - print or set the system date and time
Using Help in Linux Bash Shell
Run:
uptime --help
Example Output:
Usage:
 uptime [options]

Options:
 -p, --pretty   show uptime in pretty format
 -h, --help     display this help and exit
 -s, --since    system up since
 -V, --version  output version information and exit
Final Summary
Questions
1. How many commands have you learned so far?
Commands learned so far:

pwd
cd
touch
mkdir -p
ls
ll
date
uptime
clear
Ctrl + C
man
2. What did you understand about the Linux Shell?
Write a short explanation in your own words.

3. What is the most common shell used by Linux System Administrators?
Expected Answer:

BASH (Bourne-Again Shell)
Important Activity
Post Your Final Summary on LinkedIn
Share:

What you learned
Commands practiced
Your understanding of Linux Shell
Your Linux learning journey so far