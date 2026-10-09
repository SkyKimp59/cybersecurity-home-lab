Linux File Permissions & Access Control
Project Overview

This project demonstrates basic Linux file permissions and access control using an Ubuntu virtual machine running in UTM on an Apple Silicon Mac.

Objectives
Create a sample file in Linux.
Inspect initial file permissions.
Restrict file permissions using chmod.
Verify file contents and permission settings.
Capture screenshots documenting each stage.
Tools and Environment
Ubuntu Linux
UTM virtual machine
Linux terminal
Apple Silicon MacBook Pro
Commands Used
Command	Purpose
echo "Confidential test data" > sample.txt	Creates a sample file
ls -l sample.txt	Displays file permissions and ownership
chmod 600 sample.txt	Restricts permissions to owner read/write
cat sample.txt	Displays the file contents
stat -c '%A %a %n' sample.txt	Verifies permission symbols, numeric mode, and filename
Findings

The initial file permissions were rw-rw-r--, allowing the owner and group to read and write, while other users could read the file.

After applying chmod 600 sample.txt, the permissions changed to rw-------.

The cat command confirmed that the file contents remained readable by the current user. The stat command verified permission mode 600.

Screenshots
01-initial-permissions.png — Initial file permissions.
02-restricted-permissions.png — Permissions after applying chmod 600.
03-permission-verification.png — File contents and final permission verification.
Skills Demonstrated
Linux command-line fundamentals
File permissions and access control
Permission mode interpretation
Basic system security
Technical documentation and evidence collection
Security Note

This exercise was performed in a self-managed virtual machine for educational purposes. Permission settings were verified, but access by a separate user account was not tested.