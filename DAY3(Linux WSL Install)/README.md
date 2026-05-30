Welcome to NIT Academy - Day 3
Day-3: Monday 11th May, 2026

Table of Contents
Task	Title	Summary
1	Open PowerShell as Administrator	Open elevated PowerShell
2	Check if WSL is Installed	Verify existing WSL installation
3	Check Installed Linux Distros	View installed Linux distributions
4	Check Available Distros	View downloadable Linux distros
5	Install WSL	Install WSL and Ubuntu
6	Install Specific Distro	Install Ubuntu, Debian, etc.
7	First Linux Setup	Create Linux username/password
8	Start WSL Manually	Launch Linux manually
9	Verify Linux Is Working	Test Linux functionality
10	Check WSL Version	Verify WSL 2
11	Convert Existing Distro to WSL2	Upgrade distro version
12	Set Default Distro	Configure default Linux distro
13	Shutdown and Restart WSL	Restart Linux environment
14	Access Windows Files from Linux	Access Windows drives
15	Access Linux Files from Windows	Access Linux files from Explorer
16	Common Commands	Frequently used commands
17	Common Problems and Fixes	Beginner troubleshooting
18	Final Verification Checklist	Confirm installation success
What is WSL?
WSL (Windows Subsystem for Linux) is a feature in Windows that allows you to run a Linux environment directly inside Windows without requiring:

Dual boot
A separate virtual machine
Additional hypervisors
This allows students to use Linux commands and development tools directly from Windows.

Why Do We Need WSL?
Our goal is to provide Linux systems in an Open-Source environment without requiring students to purchase additional software or subscriptions.

WSL allows students to:

Practice Linux commands
Use Bash shell
Run Linux tools
Learn DevOps/Linux administration
Access Linux directly from Windows
Tasks Covered in This Guide
Install WSL
Install Ubuntu Linux
Check existing WSL installation
Verify Linux is working correctly
Fix common beginner issues
Official Microsoft References
Command	Purpose
wsl --install	Install WSL
wsl --list --verbose	List installed distros
wsl --list --online	List downloadable distros
Source: Microsoft Learn

Task 1 - Open PowerShell as Administrator
Open the Start Menu
Type:
PowerShell
Right-click Windows PowerShell
Select:
Run as administrator
Task 2 - Check if WSL is Already Installed
Run:

wsl --status
If WSL is installed, you may see:

Default Distribution
Default Version
Kernel Version
WSL Version
Task 3 - Check Installed Linux Distros
Run:

wsl --list --verbose
Short version (same command as above)

wsl -l -v
Example output:

  NAME      STATE           VERSION
* Ubuntu    Stopped         2
Explanation
Column	Meaning
NAME	Installed Linux distro
STATE	Running or stopped
VERSION	WSL version
*	Default distro
If Ubuntu appears, WSL is already installed.

Task 4 - Check Available Linux Distros
Run:

wsl --list --online
Short version:(same command as above)

wsl -l -o
Example:

NAME            FRIENDLY NAME
Ubuntu          Ubuntu
Debian          Debian GNU/Linux
kali-linux      Kali Linux Rolling
openSUSE        openSUSE Leap
Task 5 - Install WSL with Default Ubuntu
Run:

wsl --install
This installs:

WSL
Ubuntu
WSL 2
Restart your computer if prompted.

Task 6 - Install a Specific Distro
To view valid distro names:

wsl --list --online
Install Ubuntu:

wsl --install -d Ubuntu
Task 7 - First Linux Setup
After installation, Linux will ask for:

Enter new UNIX username:
New password:
Retype new password:
Example username:

student
Important Notes
Linux username does NOT need to match Windows username
Password characters will NOT appear while typing
Do NOT forget your password
Task 8 - Start WSL Manually
Start default distro:

wsl
Start Ubuntu directly:

wsl -d Ubuntu
Task 9 - Verify Linux is Working
Inside Linux, run:

whoami
pwd
uname -a
cat /etc/os-release
Expected output example:

NAME="Ubuntu"
VERSION="24.04 LTS"
Update Linux Packages
Run:

sudo apt update
Then:

sudo apt upgrade -y
Task 10 - Check WSL Version
Run:

wsl --version
Also verify distro version:

wsl -l -v
Expected:

VERSION
2
Example:

  NAME      STATE           VERSION
* Ubuntu    Stopped         2
Set WSL 2 as Default
Run:

wsl --set-default-version 2
Task 11 - Convert an Existing Distro to WSL 2
If your distro shows VERSION 1:

wsl --set-version Ubuntu 2
Replace Ubuntu with your distro name.

Verify again:

wsl -l -v
Task 12 - Set Default Distro
If multiple distros are installed:

wsl --set-default Ubuntu
Now running:

wsl
will open Ubuntu automatically.

Task 13 - Shutdown and Restart WSL
Shutdown WSL:

wsl --shutdown
Restart Ubuntu:

wsl -d Ubuntu
Task 14 - Access Windows Files from WSL
Windows drives are mounted under:

/mnt
Example:

cd /mnt/c/Users
List files:

ls
Task 15 - Access Linux Files from Windows
Open File Explorer and type:

\\wsl$
Example:

\\wsl$\Ubuntu
Task 16 - Common Commands for Students
Task	Command
Check WSL status	wsl --status
List installed distros	wsl -l -v
List online distros	wsl -l -o
Install WSL	wsl --install
Install Ubuntu	wsl --install -d Ubuntu
Start WSL	wsl
Start Ubuntu	wsl -d Ubuntu
Shutdown WSL	wsl --shutdown
Set WSL2 default	wsl --set-default-version 2
Set default distro	wsl --set-default Ubuntu
Task 17 - Common Problems and Fixes
Problem 1 - wsl Command Not Recognized
Try:

Restart computer
Open PowerShell as Administrator
Run:
wsl --install
Problem 2 - No Linux Distro Installed
Check installed distros:

wsl -l -v
View downloadable distros:

wsl -l -o
Install Ubuntu:

wsl --install -d Ubuntu
Problem 3 - Ubuntu Opens Then Closes
Run:

wsl -d Ubuntu
Copy any error message and send it to the instructor.

Problem 4 - Forgot Linux Password
Open root shell:

wsl -u root
Reset password:

passwd username
Example:

passwd student
Exit:

exit
Problem 5 - Distro is WSL 1 Instead of WSL 2
Check:

wsl -l -v
Convert:

wsl --set-version Ubuntu 2
Task 18 - Final Student Verification Checklist
Run:

wsl --status
wsl -l -v
Start Ubuntu:

wsl -d Ubuntu
Inside Linux:

whoami
pwd
cat /etc/os-release
sudo apt update
If all commands work successfully, WSL is installed correctly.

Final Summary
Recommended installation:

wsl --install -d Ubuntu
Recommended updates:

sudo apt update
sudo apt upgrade -y
Recommended verification:

wsl -l -v
Expected result:

Ubuntu    Running or Stopped    2
This confirms Ubuntu is installed successfully using WSL 2.