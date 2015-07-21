SLASH Shell
===========
SLASH is a utility that can be used when building a virtual appliance to make its initial setup easier for end-users.
When the end-user first logs into a SLASH-enabled virtual appliance, she is asked a few setup questions, and can respond right in the terminal.
Currently SLASH can offer to replace the built-in root password, set the hostname, and set up static networking settings.
Finally, SLASH lets the user remove it from subsequence login shells.
Internally SLASH is implemented as a Linux shell that simply runs its set of commands and then uses BASH.

Supported Platforms
-------------------
SLASH has been tested with CentOS 7.

Pre-requisites
--------------
* nmtui must be installed for non-DHCP networking configuration to work

Setup
-----
To set up SLASH in a virtual appliance:
* Put the slash and slash-initial-setup scripts in /usr/local/bin
* Make sure they are executable
* Edit /etc/password so that the root user's shell is /usr/local/bin/slash

