Ubuntu 16.04 configuration

cat /etc/network/interfaces

source /etc/network/interfaces.d/*

auto lo

iface lo inet loopback

auto eno1

iface eno1 inet static

address 10.146.128.130

netmask 255.255.255.192

network 10.146.128.128

broadcast 10.146.128.191

gateway 10.146.128.129

# dns-* options are implemented by the resolvconf package, if installed

dns-nameservers 10.77.128.10

dns-search as0485.net

auto eno4

iface eno4 inet manual

auto eno4.1010

iface eno4 inet manual

vlan_raw_device eno4

auto eno4.1010.111

iface eno4.1010.111 inet static

address 88.43.209.2

netmask 255.255.255.252

vlan_raw_device eno4.1010