echo 'Acquire::http::Proxy "http://10.77.127.254:3128/";'  > /etc/apt/apt.conf && apt update && apt -y upgrade &&  apt -y install ethtool bridge-utils ifenslave vlan vim ipmitool qemu-kvm libvirt-bin ubuntu-vm-builder bridge-utils virtinst

cp /etc/network/interfaces /etc/network/interfaces.origin && echo "0 * * * * root cp -f /etc/network/interfaces /etc/network/interfaces.autobackup && cp -f /etc/network/interfaces.origin /etc/network/interfaces" >> /etc/crontab

echo 'Acquire::http::Proxy "http://10.77.128.254:3128/";'  > /etc/apt/apt.conf

apt update && apt -y upgrade

apt -y install ethtool bridge-utils ifenslave vlan vim ipmitool

apt -y install qemu-kvm libvirt-bin ubuntu-vm-builder bridge-utils virtinst

vim vim /etc/network/interfaces

auto lo

iface lo inet loopback

# The primary network interface

auto eno1

iface eno1 inet static

address 10.54.125.11

netmask 255.255.255.128

network 10.54.125.0

broadcast 10.54.125.127

gateway 10.54.125.1

# dns-* options are implemented by the resolvconf package, if installed

dns-nameservers 10.77.128.10

dns-search as485.net

auto eno2

iface eno2 inet manual

up ip link set dev $IFACE txqueuelen 5000

bond-master bond0

auto eno3

iface eno3 inet manual

up ip link set dev $IFACE txqueuelen 5000

bond-master bond0

auto eno4

iface eno4 inet manual

up ip link set dev $IFACE txqueuelen 5000

bond-master bond0

auto bond0

iface bond0 inet manual

bond-slaves eno2 eno3 eno4

bond-mode 802.3ad

bond-xmit_hash_policy layer2+3

up ip link set dev $IFACE up; ip link set dev $IFACE txqueuelen 5000

down ip link set dev $IFACE down

auto bond0.1040

iface bond0.1040 inet manual

up ip link set dev $IFACE up; ip link set dev $IFACE txqueuelen 5000

down ip link set dev $IFACE down

auto bond0.1041

iface bond0.1041 inet manual

up ip link set dev $IFACE up; ip link set dev $IFACE txqueuelen 5000

down ip link set dev $IFACE down