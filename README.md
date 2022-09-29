## <p align="center"> VPN Server Hardening Script (based on AKcryptoGUY's script)</p>

# About

This script intends to be an assistant to configure a Ubuntu server to be used as a VPS, performing hardening and securization tasks to prevent malicious attacks and function as a VPN server.

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

# Configure to use with OpenVPN

Follow the steps provided in the following project:
https://github.com/MJFiuba/openvpn-server-install
