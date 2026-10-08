# Headless Arch Linux Home Server & Network Storage

A personal home-server project built on an older Intel PC running Arch Linux.
The project was created to gain practical experience with Linux system administration, networking, storage management, SSH security, and SMB file sharing.

## 🛠️ Architecture & Hardware

* **Server:** Intel PC running Arch Linux
* **Client/Host:** Windows laptop
* **Network:** Direct Ethernet connection between the server and laptop
* **Storage:** SSD and HDDs using ext4/Btrfs
* **Server access:** Headless administration via SSH

## ⚙️ Networking & System Administration

* Configured a static IP network for direct Ethernet communication.
* Configured and managed the network using `systemd-networkd`.
* Disabled `NetworkManager` to avoid conflicts with `systemd-networkd`.
* Configured routing and Windows Internet Connection Sharing (ICS) for temporary Internet access during system setup.
* Troubleshot network interfaces, IP addresses, routes, and connectivity issues.

## 🔐 SSH & Security

* Configured headless remote administration through SSH.
* Set up SSH public-key authentication using `authorized_keys`.
* Configured the system so the server could be administered remotely without a monitor or keyboard.
* Disabled SSH password authentication after configuring key-based authentication.

## 💾 Storage Management

* Configured persistent disk mounting using `/etc/fstab`.
* Used UUIDs for persistent filesystem identification.
* Managed multiple SSD/HDD filesystems, including ext4 and Btrfs.
* Configured storage directories for network file sharing.
* Experimented with HDD power management and automatic disk spin-down.

## 📁 SMB / Samba File Sharing

* Installed and configured Samba/SMB.
* Created network shares for local storage.
* Configured Samba permissions and user mapping.
* Accessed the server's shared storage from Windows using UNC paths and mapped network drives.
* Tested file transfers between Windows and the Linux server.

## 🖥️ OpenMediaVault

* Later Installed and experimented with OpenMediaVault for web-based server and storage management.
* Used the system to explore practical NAS administration and storage management.

## 🧠 What I Learned

Through this project I gained hands-on experience with:

* Linux system administration
* SSH
* Public-key authentication
* Networking and routing
* `systemd-networkd`
* Samba / SMB
* Filesystem mounting and `/etc/fstab`
* UUID-based disk configuration
* SSD/HDD storage management
* Windows–Linux file sharing
* Basic server security and troubleshooting

## 🚀 Future Plans

Possible future improvements include:

* Docker and container management
* Automated backups
* Bash scripting
* Monitoring and logging
* Network-wide DNS/ad blocking
* Additional Linux security hardening
* More advanced virtualization and networking experiments

## 📌 Project Status

This is an ongoing personal learning project.
The main goal is to gain practical Linux and system-administration experience by building, troubleshooting, and maintaining a real physical server rather than only studying these concepts theoretically.
