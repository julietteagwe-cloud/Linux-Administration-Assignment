📘🖥️ Assignment 1 — Server Setup (CentOS & Ubuntu Servers)

👩🏽‍💻 By: Juliette Joseph-Odogbo
🎓 Course: CIS-245 Linux Administration
🔐 Major: Networking & Information Security
📅 Date: 09/19/2025

📝✨ Overview

This assignment demonstrates the complete setup of two Linux server environments — CentOS Server and Ubuntu Server — using Oracle VirtualBox.
Tasks included downloading ISO files, creating virtual machines, configuring system resources, networking setup, installing operating systems, verifying connectivity, and enabling secure communication between servers.

This lab helped me build foundational skills in virtualization, Linux installation, network configuration, SSH remote access, and secure file transfers—key abilities for every Networking & Information Security professional.

🎯🚀 Skills Learned
🖥️ Virtualization & VM Configuration

Installed and configured Oracle VirtualBox

Created CentOS and Ubuntu VM instances

Adjusted system resources: RAM, CPU cores, storage

Attached ISO images for installation

Reviewed VM summaries and validated hardware settings

⚙️🐧 Linux Server Installation

Installed CentOS Server (No GUI)

Installed Ubuntu Server 24.04 LTS

Selected language, keyboard, time zone

Configured server name, usernames, and passwords

Enabled administrative privileges

🌐📡 Networking & Connectivity

Switched VirtualBox networking from NAT → Bridged Adapter

Viewed network interfaces using:

ip addr


Tested internet access using:

ping -c 4 www.google.com


Verified server-to-server communication (ping tests)

Confirmed 0% packet loss between CentOS and Ubuntu

🔐📁 Secure Remote Access & File Sharing

Installed OpenSSH server on both systems

Enabled and started SSH using systemctl

Created test files with echo

Transferred files securely between servers using scp

Verified file placement with ls

Successfully authenticated remote connections

🔧💻 Important Commands Used
# View IP address
ip addr

# Test internet connection
ping -c 4 www.google.com

# Install SSH on Ubuntu
sudo apt install openssh-server -y

# Install SSH on CentOS
sudo yum install openssh-server -y

# Enable SSH services
sudo systemctl enable ssh
sudo systemctl enable sshd

# Start SSH services
sudo systemctl start ssh
sudo systemctl start sshd

# Create files for testing
echo "hello" > ubuntu.txt
echo "centos test" > centos.txt

# Secure file transfer (Ubuntu → CentOS)
scp ubuntu.txt centosuser@CENTOS-IP:/home/centosuser/

# Secure file transfer (CentOS → Ubuntu)
scp centos.txt ubuntuuser@UBUNTU-IP:/home/ubuntuuser/

# Verify file transfer
ls /home/username/

🖼️📸 Screenshots Included

Upload your screenshots to:

📁 Assignment1_Server_Setup/screenshots/

Recommended filenames:

📝 Description	📁 File Name
VM Creation	01_vm_creation.png
Network Adapter Settings	02_network_adapter.png
CentOS Installation Menu	03_centos_install.png
Ubuntu Installation Steps	04_ubuntu_install.png
IP Address Output	05_ip_addr.png
Ping Test Results	06_ping_test.png
SSH Service Status	07_ssh_status.png
SCP File Transfer	08_scp_transfer.png
