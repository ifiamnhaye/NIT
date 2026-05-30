Linux Practice Lab – Users, Directories & Files
Hands-On Linux Filesystem Practice
Date 18th May, 2026 - Day 10

Objective: Practice Linux navigation, user management, directory creation, file creation, and filesystem visualization.

Task 1 - Verify Current Logged-in User
Run:
whoami
Questions
What username is displayed?
Are you logged in as root or a normal user?
Task 2 - Navigate to the /home Directory
Run:
cd /home
Verify Your Current Location
Run:

pwd
Expected output:

/home
Task 3 - List the Contents of /home
Run:
ls -l
Observation
What do you see?
Are there any user directories already created?
NOTE: On a fresh installation there should normally be NO regular user directories unless users were already created earlier.

Task 4 - Create Two Users
Run:
useradd student
useradd Alice
Verify the Users Were Created
Run:

ls -l /home
Expected output should now include:

student
Alice
Task 5 - Navigate to Alice's Home Directory
Run:
cd /home/Alice
Verify Your Current Location
Run:

pwd
Expected output:

/home/Alice
Task 6 - Check the Contents of Alice's Directory
Run:
ls -l
Observation
What do you see?
There should be nothing inside Alice's home directory initially.
Task 7 - Create Multiple Directories Using mkdir -p
Run: You can create all these directories in one go!
mkdir -p projects docs images
Verify the Directories
Run:

ls -l
Expected directories:

projects
docs
images
Task 8 - Navigate to the projects Directory
Run:
cd projects
Verify the Contents
Run:

ls -l
OR

ll
Observation
Is the directory empty?
Task 9 - Create a File
Run:
touch report.txt
Verify the File Was Created
Run:

ls -l
Expected output should include:

report.txt
Task 10 - Move One Level Up
Run:
cd ..
Verify Your Current Location
Run:

pwd
Expected output:

/home/Alice
Task 11 - List the Contents Again
Run:
ls -l
Observation
You should now see:

projects
docs
images
Task 12 - Navigate to the images Directory
Run:
cd images
Verify the Directory Contents
Run:

ls -l
Observation
Is the images directory empty?
Task 13 - Create an Image File
Run:
touch logo.png
Verify the File
Run:

ls -l
Expected output:

logo.png
Task 14 - Return to Your Home Directory
Run:
cd
Questions
Do you see the tilde symbol ~?
The tilde ~ means you are inside your home directory.
Task 15 - Verify Your User and Current Directory
Run:
whoami
pwd
Questions
Which user are you logged in as?
Which home directory are you currently inside?
Task 16 - Install the tree Package
Run:
dnf install -y tree
Important Practice
During installation:

Press:

Ctrl + C
Observation
What happened?
The installation should stop/interupt.
Task 17 - Install tree Again
Run:
dnf install -y tree
This Time
Allow the installation to complete successfully.

Task 18 - Display the Linux Directory Hierarchy
Run:
tree -d /home
Observation
Do you see the directory hierarchy?
Can you identify:
Alice
projects
docs
images
Final Questions
What does whoami do?
What does pwd display?
What does cd .. mean?
What does cd by itself do?
What is the purpose of touch?
Why is tree useful?
What does the tilde ~ represent?
What does mkdir -p do?
Final Reflection
Write a short paragraph explaining:

What you learned from this lab
Which command was most useful
Which command was difficult
Why Linux filesystem navigation is important
