cat /etc/networkd-dispatcher/routable.d/50-ifup-hooks 

#!/bin/bash

/usr/sbin/ethtool -s enp5s0 speed 100 duplex full autoneg off

----------------------

chmod +x /etc/networkd-dispatcher/routable.d/50-ifup-hooks 