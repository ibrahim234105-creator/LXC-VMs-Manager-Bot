# LXC-Bot-V6

- ⚡ Easy & Fast LXC Container Management
- ✨ Quick Creations & Responses
- 🔐 Secure Containers Creation
- ✅ Made for Hosting Owners
- 🟢 100% Free & Open-Source

# Installation Guide

1) bash <(curl -fsSL https://raw.githubusercontent.com/hopingboyz/lxc-installer/main/lxc-installer.sh)

2) sudo apt install snapd -y

3) sudo systemctl enable --now snapd.socket

4) sudo ln -s /var/lib/snapd/snap /snap

5) sudo snap install lxd

6) sudo usermod -aG lxd $USER
newgrp lxd

7) reboot

8) sudo lxd init

9) apt install python3-pip -y

10) mkdir -p ~/.config/pip && echo -e "[global]\nbreak-system-packages = true" > ~/.config/pip/pip.conf

11) sudo nano /etc/systemd/system/fusionodes.service

12) Paste it
[Unit]
Description=FusionNodes Discord Bot
After=network.target

[Service]
User=root
WorkingDirectory=/root

# Environment Variables
Environment="PYTHONUNBUFFERED=1"
Environment="DISCORD_TOKEN=YOUR_DISCORD_BOT_TOKEN"
Environment="MAIN_ADMIN_ID=YOUR_ADMIN_ID"

# Start Bot
ExecStart=/usr/bin/python3 /root/bot.py

# Auto-Restart
Restart=always
RestartSec=5

[Install]
WantedBy=multi-user.target

13) sudo systemctl daemon-reload
sudo systemctl restart fusionodes

14) Add bot.py file.

15) pip install discord

16) pip install PyNaCl

17) python3 bot.py

# Made by FeatherPlayz & HopingBoyz
