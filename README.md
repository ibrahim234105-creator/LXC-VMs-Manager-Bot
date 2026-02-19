# 🚀 LXC-Bot-V6

- **⚡ Easy & Fast LXC Container Management**
- ✨ **Quick Creations & Responses**
- 🔐 **Secure Containers Creation**
- ✅ **Made for Hosting Owners**
- 🟢 **100% Free & Open-Source**

# Installation Guide

1) bash <(curl -fsSL https://raw.githubusercontent.com/hopingboyz/lxc-installer/main/lxc-installer.sh)

**⚠️ IF YOU GET ERROR WHILE USING THE SCRIPT, TRY THE CODE BELOW!**
**——————————————————————————————————————————————————————————————————————**

sudo apt install snapd -y

sudo systemctl enable --now snapd.socket

sudo ln -s /var/lib/snapd/snap /snap

sudo snap install lxd

**——————————————————————————————————————————————————————————————————————**

sudo usermod -aG lxd $USER
newgrp lxd

reboot

sudo lxd init

apt install python3-pip -y

mkdir -p ~/.config/pip && echo -e "[global]\nbreak-system-packages = true" > ~/.config/pip/pip.conf

sudo nano /etc/systemd/system/fusionodes.service

Paste it:
[Unit]
Description=FusionNodes Discord Bot
After=network.target

[Service]
User=root
WorkingDirectory=/root

Environment="PYTHONUNBUFFERED=1"
Environment="DISCORD_TOKEN=YOUR_DISCORD_BOT_TOKEN"
Environment="MAIN_ADMIN_ID=YOUR_ADMIN_ID"

ExecStart=/usr/bin/python3 /root/bot.py

Restart=always
RestartSec=5

[Install]
WantedBy=multi-user.target



sudo systemctl daemon-reload

sudo systemctl restart fusionodes

14) Add bot.py file.

15) pip install discord

16) pip install PyNaCl

17) python3 bot.py

# FeatherPlayz All Right Reserved
