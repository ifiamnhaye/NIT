Linux Practice Lab - Created by Instructor M.Khalid Khan
May 20th, 2026 - Day 20th A complete hands-on Linux practice environment for beginners and intermediate learners.

This project automatically creates files, directories, logs, scripts, CSV data, and practice resources to help you learn and practice 100+ Linux commands.

Features
✅ Creates a complete Linux practice environment
✅ Generates sample files and directories
✅ Creates CSV and log files
✅ Includes shell scripting examples
✅ Permission practice setup
✅ Compression practice data
✅ Great for beginners learning Linux commands

📂 Project Structure
linux-practice/
│
├── files/
├── logs/
├── scripts/
├── backup/
├── data/
├── users/
├── temp/
├── projects/
└── compress_me/
⚙️ Requirements
Linux OS (Ubuntu, CentOS, Fedora, Kali, WSL, etc.)
Bash shell
🚀 Setup
1️⃣ Clone Repository
git clone https://github.com/yourusername/linux-practice-lab.git
2️⃣ Move into Project Directory
cd linux-practice-lab
3️⃣ Make Script Executable
chmod +x linux-practice.sh
4️⃣ Run Script
./linux-practice.sh
OR

bash linux-practice.sh
📁 What This Script Creates
Files
employees.txt
fruits.txt
story.txt
numbers.txt
secure.txt
bigfile.img
CSV Files
students.csv
Logs
system.log
Scripts
hello.sh
Directories
backup/
projects/
temp/
compress_me/
🧪 Linux Commands You Can Practice
Navigation Commands
pwd
whoami
date
ls
ls -ltr
clear
cd files
cd ..
File Management (Creation & Deletion)
touch files/test.txt

rm files/test.txt

mkdir testdir

rmdir testdir
Copy / Move / Rename
cp files/story.txt backup/

mv files/story.txt files/newstory.txt

mv files/newstory.txt files/story.txt
File Viewing
cat files/story.txt

less files/story.txt

more files/story.txt

head -3 files/story.txt

tail -2 files/story.txt
Search Commands
grep "Linux" files/story.txt

egrep "ERROR|WARNING" logs/system.log

find ~/linux-practice -name "*.txt"
Sorting & Unique
sort files/fruits.txt

sort files/fruits.txt | uniq
Count Lines
wc -l files/fruits.txt
Shuffle
shuf files/fruits.txt
Split File
split -l 5 files/numbers.txt split_
Compare Files
cp files/story.txt files/story2.txt

cmp files/story.txt files/story2.txt

diff files/story.txt files/story2.txt
Copy / Move / Rename
cp files/story.txt backup/

mv files/story.txt files/newstory.txt

mv files/newstory.txt files/story.txt
Find Files
find ~/linux-practice -name "*.txt"
AWK Practice
Print second column:

awk -F "," '{print $2}' data/students.csv
CUT Practice
cut -c1-5 files/story.txt
SED Practice
Print line 2:

sed -n '2p' files/story.txt
Replace word:

sed 's/Linux/UNIX/g' files/story.txt
TR Practice
Uppercase:

tr '[:lower:]' '[:upper:]' < files/story.txt
FOLD Practice
echo "ABCDEFGHIJK" | fold -w1
Compression Practice
gzip
gzip files/story.txt

gunzip files/story.txt.gz
tar
tar -czf backup.tar.gz compress_me/

tar -xzf backup.tar.gz
zip
zip files.zip files/fruits.txt files/story.txt

unzip -l files.zip
Process Practice
Run process in background:

sleep 300 &
Check jobs:

jobs
Foreground / Background:

bg

fg
Kill process:
ps -ef | grep sleep

pkill sleep
System Information
hostname

uname -a

lscpu

free -h

df -h

du -sh ~/linux-practice
Networking Practice
ping google.com

curl http://numbersapi.com/random

wget https://example.com
Environment Variables
export MYNAME="Khalid"

echo $MYNAME

printenv
Alias Practice
alias ll='ls -ltr'

ll
Scheduling Practice
crontab -e
Example cron:

* * * * * echo "Hello" >> ~/linux-practice/logs/cron.log
User Management
sudo useradd testuser

sudo passwd testuser

id testuser

sudo userdel testuser
Permissions
chmod 755 files/story.txt

chown $USER files/story.txt

chgrp $USER files/story.txt
🎯 Learning Goals
This project helps you learn:

Linux terminal basics
File operations
Directory management
Text processing
Shell scripting
Permissions
Compression tools
Networking basics
Process management
📚 Recommended Practice Order
Practice in this order:

Navigation Commands
File Management
Text Processing
Search Commands
Compression
Permissions
Process Management
Networking
Automation
User Management
🐧 Happy Learning Linux!
Practice daily and experiment with commands to become comfortable with Linux administration and shell scripting.