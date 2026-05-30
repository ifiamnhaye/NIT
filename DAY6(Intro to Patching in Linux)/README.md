 Interview Question: Tell me if you have done PATCHING?
⚠️ MANDATORY LAB UPDATE: GUEST TOOLS PATCHING Attention Batch 3 Students
 NOTE:
To ensure your virtual machines are properly monitored and optimized within the NIT Academy infrastructure, everyone is required to perform the following critical patching activity. This will resolve the "Management Agent Not Detected" error on your dashboards (See Snapshot below).


TASK 1
Log in to your Xen Orchestra instance.
Access your assigned Linux Machine console.
Execute the following commands as root
Step 1: Enable Repositories & Install
# Install EPEL first
dnf install -y epel-release

# Install Guest Utilities
dnf install -y xe-guest-utilities-latest
Step 2: Post-Installation Validation
Enable and start the distribution service
systemctl enable --now xe-linux-distribution
Final Submission (Post Patching):
Once the patching is completed and the warning disappears from your dashboard: 

Use the Snipping Tool to capture your terminal results and the green "Agent Detected" status in Xen Orchestra.

LinkedIn Challenge: Share your screenshot on LinkedIn to document your progress in the 100-Day Journey.

#NIT <--- Do not forget this in your linkedin post