slash

Shell that helps set up common parameters for a virtual appliance for a Red Hat or CentOS server.
Tested with CentOS 7.

To set up SLASH:
Put the two scripts in /usr/local/bin, and edit /etc/password so that the root user's shell is /usr/local/bin/slash

Now whenever the root user logs in, she is prompted to choose a new root password, hostname, networking, and whether or not to repeat this script in the next login.

Requirements:
* nmtui must be installed for non-DHCP networking configuration to work

Copyright(C) Intigua 2015

