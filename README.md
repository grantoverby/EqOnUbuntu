&#x200B;

Install Ubuntu 18.04. Any desktop flavor should work; I use Xubuntu.

Run the following in a terminal.

    sudo apt-get update
    sudo apt-get install -y git
    me="$(whoami)"
    sudo mkdir -p /opt/eq
    sudo chown "${me}" /opt/eq
    sudo chgrp "${me}" /opt/eq
    git clone http://github.com/grantoverby/EqOnUbuntu.git /opt/eq
    /opt/eq/bin/install

You'll be prompted with some GUIs. Follow the defaults, with one exception: On the direct x install, accept the license, click next, and then on the next part of the install window click close without direct x actually being installed.

Wait for EQ to fully download, then exit the patcher.

    /opt/eq/bin/post-install

To run EQ

    /opt/eq/bin/launch
