[root@co network-scripts]#  cat ifcfg-eth0

DEVICE="eth0"

BOOTPROTO="static"

#BROADCAST="192.168.1.255"

#DNS1="192.168.1.1"

#GATEWAY="192.168.1.1"

HWADDR="00:25:22:9C:F2:BE"

#IPADDR="192.168.1.30"

#NETMASK="255.255.255.0"

NM_CONTROLLED="no"

BRIDGE="br0"

ONBOOT="yes"

TYPE="Ethernet"

UUID="4cb6bec4-d848-4ef0-945e-8a6e45bd5516"

ETHTOOL_OPTS="speed 100 duplex full autoneg off"

[root@co network-scripts]#  cat ifcfg-br0

DEVICE="br0"

TYPE="Bridge"

BOOTPROTO="static"

BROADCAST="192.168.1.255"

DNS1="192.168.1.1"

GATEWAY="192.168.1.1"

HWADDR="00:25:22:9C:F2:BE"

IPADDR="192.168.1.30"

NETMASK="255.255.255.0"

NM_CONTROLLED="no"

ONBOOT="yes"

STP="on"