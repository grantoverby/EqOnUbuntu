Install Ubuntu 18.04. Any desktop flavor should work. This was tested on Xubuntu 18.04.

Run the following in a terminal.

    sudo apt-get update
    sudo apt-get install -y git
    mkdir -p ~/eq
    git clone http://github.com/grantoverby/EqOnUbuntu.git ~/eq
    ~/eq/bin/install

You'll be prompted with some GUIs. Follow the defaults, with one exception: On the DirectX install, accept the license, click next, and then on the next part of the install window click close without DirectX actually being installed.

Wait for EverQuest to fully download, then exit the patcher.

    ~/eq/bin/post-install

Run EverQuest.

    ~/eq/bin/launch
