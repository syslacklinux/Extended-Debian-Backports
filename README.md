<img width="846" height="224" alt="Screenshot From 2026-07-12 18-26-56" src="https://github.com/user-attachments/assets/94b92acb-a68e-40f0-b285-b30720853eb5" />

# Extended Debian Backports
This is a Extended Backports for Debian for example changing Debian 11 kernel and backports with Debian 13 kernel and backports
This also Works in Debian 12 11 and lower to get a latest kernel

To get it

sudo nano /etc/apt/sources.list.d/debian-backports.sources
then

Types: deb deb-src
URIs: http://deb.debian.org/debian
Suites: stable-backports
Components: main
Enabled: yes
Signed-By: /usr/share/keyrings/debian-archive-keyring.gpg

if you want other Suite change Suites stable-backports with oldstable-backports or oldoldstable-backports

Ctrl X Y Enter

run sudo apt update && sudo apt upgrade -y -t stable-backports
If oldstable backports sudo apt update && sudo apt upgrade -y -t oldstable-backports
if oldoldstable backports sudo apt update && sudo apt upgrade -y -t oldoldstable-backports
Then sudo apt autoremove then reboot
