Windows 11 VM Setup

Date: Aug 5, 2025

Purpose: Create a baseline Windows 11 lab VM for Sysmon, logging, and Blue Team training.

Configuration:
- RAM: 5000 MB
- CPUs: 2
- Disk: 64 GB (dynamic)
- ISO: Win11_24H2_English_x64.iso
- Network: NAT (default)

Documentation:
- Setup and configured a Win11 VM for the first time. Lots of settings that I don't understand yet but I'll learn, set most of them to default with the exceptions of increasing my allocated RAM.
- Installed VirtualBox Guest Additions to fix a screen size issue.
  
Next Steps:
- Install Sysmon and logging configs
- Enable RDP
- Add to Splunk later
