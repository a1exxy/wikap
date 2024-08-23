http://help.ubuntu.ru/wiki/kvm

sudo apt-get install qemu-kvm libvirt-bin ubuntu-vm-builder bridge-utils

https://habrahabr.ru/post/242741/

apt-get install openvswitch-switch

ovs-vsctl add-br ovs-br0 

ovs-vsctl set port ovs-br0 tag=7 

ovs-vsctl add-port ovs-br0 eth0 

ovs-vsctl set port eth0 trunks=7,10,20,1010,1020,30,1030 

ifconfig eth0 0 

ifconfig ovs-br0 10.0.7.1/24 up 

ip r add default via 10.0.7.254

ovs-vsctl add-br br0

ovs-vsctl add-bond br0 bond0 eth1 eth2 

ovs-vsctl set port bond0 bond_mode=balance-tcp 

ovs-vsctl set port bond0 vlan_mode=native-untagged trunks=[1,3] tag=2 

ovs-vsctl list port bond0

ovs-vsctl add-bond ovsbr1 bond0 eth1 eth3 lacp=active

ovs-vsctl add-bond ovs-br-bond2 bond2 eno3 eno4 lacp=active

ovs-vsctl add-port ovs-br-bond2  bond2.1043 tag=1043  -- set interface bond2.1043 type=internal

ovs-vsctl add-br ovs-root-mgmnt -- set port ovs-root-mgmnt tag=7 -- add-port ovs-root-mgmnt eno1 -- set port eno1 tag=7;  ifconfig eno1 0; ifconfig ovs-root-mgmnt 10.77.128.198/24 up; ip route add default via 10.77.128.30;

cat /etc/network/interfaces

# interfaces(5) file used by ifup(8) and ifdown(8)

auto lo

iface lo inet loopback

auto eno1

iface eno1 inet manual

auto ovs-br0

iface ovs-br0 inet static

       address 10.77.124.10

	netmask	255.255.255.0

	gateway 10.77.124.30

	dns-search as.net tt.net

       dns-nameservers 10.77.128.10