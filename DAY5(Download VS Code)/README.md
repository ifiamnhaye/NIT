Downloading Visual Studio Code on Windows, Chromebook, and Mac
Wednesday 13th May, 2026 - DAY 5

DO ONLY ONE TASK BASED ON YOUR MACHINE!
Table of Contents
Task	Title
1	Installation for Windows
2	Installation for Chrome Book
3	Installation for Mac
Task 1 - Installation for Windows
Step 1: Open the VS Code Website
Go to:

https://code.visualstudio.com/

You will see a large blue download button.

Step 2: Download VS Code for Windows
Click:

Download for Windows

This downloads the .exe installer.

Step 3: Run the Installer
Open the downloaded file
Click Next
Accept the license agreement
Keep clicking Next
Click Install
Recommended Options
Add to PATH
Create desktop icon
Step 4: Launch VS Code
After installation:

Click Finish
VS Code opens automatically
You can also search:

Start Menu → Visual Studio Code
Task 2 - Installation for Chrome Book
Step 1: Enable Linux on Chromebook
Open Settings
Go to Developer
Turn ON Linux Development Environment
Step 2: Open the Linux Terminal
After Linux installs:

Open Launcher
Search for Terminal
Open it
Step 3: Install VS Code
Run these commands one by one:

sudo apt update
sudo apt install wget gpg -y
wget -qO- https://packages.microsoft.com/keys/microsoft.asc | gpg --dearmor > packages.microsoft.gpg
sudo install -D -o root -g root -m 644 packages.microsoft.gpg /etc/apt/keyrings/packages.microsoft.gpg
echo "deb [arch=amd64 signed-by=/etc/apt/keyrings/packages.microsoft.gpg] https://packages.microsoft.com/repos/code stable main" | sudo tee /etc/apt/sources.list.d/vscode.list
sudo apt update
sudo apt install code -y
Step 4: Launch VS Code
Open Launcher
Search for:
Visual Studio Code
Open it
Task 3 - Installation for Mac
Step 1: Open the VS Code Website
Visit:

https://code.visualstudio.com/download

Click:

Download for Mac

Choose:

Apple Silicon OR
Intel Chip
Step 2: Open the Downloaded ZIP File
Open Downloads
Double-click the ZIP file
Extract Visual Studio Code
Step 3: Move VS Code to Applications
Drag:

Visual Studio Code.app
into:

Applications
Step 4: Open VS Code
Open Applications
Click Visual Studio Code
If prompted:

Click Open
