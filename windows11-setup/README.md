Windows 11 VM Setup

Date: Aug 5, 2025

VM Program: Oracle VirtualBox

Purpose: Create a baseline Windows 11 lab VM for Sysmon, logging, and Blue Team training.

Configuration:
- RAM: 5000 MB
- CPUs: 2
- Disk: 64 GB (dynamic)
- ISO: Win11_24H2_English_x64.iso
- Network: NAT (default)

Configured Tools:
- VirtualBox Guest Additions
- Sysinternals Suite
- Sysmon with SwiftOnSecurity config
- Event Viewer monitoring (Sysmon/Operational)
  
Documentation:
- Setup and configured a Win11 VM for the first time. Enabled EFI and configured ISO manually
- Installed VirtualBox Guest Additions to fix a screen size issue.
- Set up internet, bidirectional clipboard, drag and drop
- Installed Sysinternals Suite
- Installed Sysmon with SwiftOnSecurity config via "cmd"
- Added Sysinternals to PATH so I can run commands from any terminal
- Tried to update Windows Advanced Audit Policy but couldn't because my Win11 VM is running Win11 Home. I could update via regedit but I heard no one should touch it if you don't know what you're doing so I opted to redo everything on a Win11 Pro VM instead.
- Set up password policy and enabled audit process creation via "secpol.msc"
- Enable behavior monitoring, real time monitoring, include command line in process creation events, etc,. In Local Group Policy Editor
- Verified Sysmon is working with harmless command in Powershell
  
Next Steps:
- Enable RDP
- Add to Splunk later

