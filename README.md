## <p align="center"> Server Hardening Script (based on AKcryptoGUY's script)</p>

# About

A lot of good virtual servers get destroyed every year because they are hacked by evildoers that take advantage of unpatched exploits and simple passwords. It's frustrating that many of these hacks could have been prevented by some basic hardening. With large numbers of Linux newcomers flocking to enter the space and set up masternodes I saw a need for a simple way to secure virtual servers that would, *for the most part*, keep the bad guys out. It is my intent to keep this script general enough that it could be the first script run on many different types of VPS installations to prepare them for whatever use you have planned.

The following is a list of different sections of the script, which are broken up into separate functions which are called from the very end of the script. 

1. CREATE SWAP / if no swap exists, set swap to 2x RAM (not less than 2GB)
2. UPDATE AND UPGRADE / update operating system & pkgs
3. INSTALL FAVORED PACKAGES / useful tools & utilities
4. USER SETUP / add new sudo user, copy SSH keys
5. SSH CONFIG / change SSH port, disable root login
6. UFW CONFIG / UFW - add rules, harden, enable firewall
7. HARDENING / before rules, secure shared memory, etc
8. GOOGLE AUTH / enable 2fa using Google Authenticator
9. KSPLICE INSTALL / automatically update without reboot
10. MOTD EDIT / replace boring banner with customized one
11. RESTART SSHD / apply settings by restarting systemctl
12. INSTALL COMPLETE / display new SSH and login info



# Installation

Follow the steps provided in install_steps.txt
