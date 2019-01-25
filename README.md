Install Ubuntu 18.04. Any desktop flavor should work. This was tested on Xubuntu 18.04.

Run the following in a terminal.

    me="$(whoami)"
    sudo apt-get update
    sudo apt-get install -y git
    sudo mkdir -p /opt/eq
    sudo chown "${me}" /opt/eq
    sudo chgrp "${me}" /opt/eq
    git clone http://github.com/grantoverby/EqOnUbuntu.git /opt/eq
    /opt/eq/bin/install

You'll be prompted with some GUIs. Follow the defaults, with one exception: On the DirectX install, accept the license, click next, and then on the next part of the install window click close without DirectX actually being installed.

Wait for EverQuest to fully download, then exit the patcher.

    /opt/eq/bin/post-install

Run EverQuest.

    /opt/eq/bin/launch
