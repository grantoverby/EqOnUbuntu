# 64bit EverQuest Notice

This repo has been updated to work with EQ's new 64 bit client.

You may need to start with a fresh install, and as such, the install directory in the guide below has been changed. If you'd like to try without reinstalling, change win32 to win64 in lib/vars or pull the latest changes.

---

# Instructions

Install Ubuntu 18.04. Any desktop flavor should work. This was tested on Xubuntu 18.04.

Run the following in a terminal.

    sudo apt-get update
    sudo apt-get install -y git
    mkdir -p ~/eq64
    git clone http://github.com/grantoverby/EqOnUbuntu.git ~/eq64
    ~/eq64/bin/install

You'll be prompted with some GUIs. Follow the defaults, with one exception: On the DirectX install, accept the license, click next, and then on the next part of the install window click close without DirectX actually being installed.

Wait for EverQuest to fully download, then exit the patcher.

    ~/eq64/bin/post-install

Run EverQuest.

    ~/eq64/bin/launch
