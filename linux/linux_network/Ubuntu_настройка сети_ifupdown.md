ip link add link eth0 name vlan122 type vlan id 122

For 18.04:

#cat /etc/network/interfaces

source /etc/network/interfaces.d/*

#cat /etc/network/interfaces.d/mgnt 

auto eno1

iface eno1 inet dhcp

#cat /etc/network/interfaces.d/vmnet 

auto eno2 eno3 eno4

iface eno2 inet manual

bond-master bond0

up ip link set dev $IFACE txqueuelen 10000

iface eno3 inet manual

bond-master bond0

up ip link set dev $IFACE txqueuelen 10000

iface eno4 inet manual

bond-master bond0

up ip link set dev $IFACE txqueuelen 10000

auto bond0

iface bond0 inet manual

bond-slaves eno2 eno3 eno4

bond-miimon 100

bond-mode 802.3ad

bond-xmit_hash_policy layer2+3

# 

auto enp0s7

iface enp0s7 inet static

    address 192.168.1.112

    netmask 255.255.255.0 

    gateway 192.168.1.100

    dns-nameservers 192.168.1.100

    link-speed 100

    link-duplex full

    ethernet-autoneg off

Updateing:

sudo apt-get update

sudo apt-get upgrade

Updating:

sudo apt-get update

sudo apt-get upgrade

Installing:

sudo apt-get install ethtool

sudo apt-get install bridge-utils

sudo apt-get install ifenslave

sudo apt-get install vlan

sudo apt-get update && sudo apt-get upgrade

sudo apt-get install ethtool bridge-utils ifenslave vlan

====================================================================

Adding modules

sudo vi /etc/modules

Make sure it has these in it

# /etc/modules: kernel modules to load at boot time.

#

# This file contains the names of kernel modules that should be loaded

# at boot time, one per line. Lines beginning with “#” are ignored.

loop

lp

rtc

bonding

====================================================================

root@brlvsi01:~# cat /etc/network/interfaces

auto lo

iface lo inet loopback

auto em1

iface em1 inet manual

mtu 9000

bond-master bond0

auto em2

iface em2 inet manual

mtu 9000

bond-master bond0

auto em3

iface em3 inet manual

mtu 9000

bond-master bond1

auto em4

iface em4 inet manual

mtu 9000

bond-master bond1

auto bond0

iface bond0 inet manual

bond-mode 1

bond-miimon 100

#bond-slaves em1 em3

bond-slaves none

auto br0

iface br0 inet static

address 10.22.125.130

gateway 10.22.125.129

netmask 255.255.255.192

dns-nameservers 10.77.128.10

dns-search ttk.net

bridge_ports bond0

auto br0.1050

iface br0.1050 inet manual

#iface br0.1050 inet static

#        address 188.143.42.2

#        netmask 255.255.255.0

        vlan-raw-device br0

auto bond1

iface bond1 inet manual

bond-mode 1

bond-miimon 100

#bond-slaves em2 em4

bond-slaves none

auto br1

iface br1 inet static

address 10.22.125.227

netmask 255.255.255.224

bridge_ports bond1

auto br1050

iface br1050 inet manual

bridge_ports br0.1050

iptech@ebgvsi01:~$ cat /etc/network/interfaces

auto lo

iface lo inet loopback

auto em1

iface em1 inet manual

mtu 9000

bond-master bond0

auto em2

iface em2 inet manual

mtu 9000

bond-master bond0

auto em3

iface em3 inet manual

mtu 9000

bond-master bond1

auto em4

iface em4 inet manual

mtu 9000

bond-master bond1

auto bond0

iface bond0 inet manual

bond-mode 1

bond-miimon 100

bond-slaves none

auto br0

iface br0 inet static

address 10.66.125.130

gateway 10.66.125.129

netmask 255.255.255.192

dns-nameservers 10.77.128.10

dns-search ttk.net

bridge_ports bond0

auto br0.1050

iface br0.1050 inet manual

        vlan-raw-device br0

auto br0.1018

iface br0.1018 inet manual

        vlan-raw-device br0

auto br0.19

iface br0.19 inet manual

        vlan-raw-device br0

auto bond1

iface bond1 inet manual

bond-mode 1

bond-miimon 100

bond-slaves none

auto br1

iface br1 inet static

address 10.66.125.227

netmask 255.255.255.224

bridge_ports bond1

auto br1050

iface br1050 inet manual

bridge_ports br0.1050

auto br1018

iface br1018 inet manual

bridge_ports br0.1018

auto br19

iface br1019 inet manual

bridge_ports br0.19