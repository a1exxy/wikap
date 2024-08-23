KVM на CentOS :

yum  install kvm libvirt python-virtinst qemu-kvm bridge-utils

http://habrahabr.ru/post/168791/

http://www.alsigned.ru/?p=2027

https://www.dmosk.ru/miniinstruktions.php?mini=kvm-centos7

Просмотр доступных ОС для ВМ:

osinfo-query os

Bridge network config:

[root@co ~]# cat /etc/sysconfig/network

NETWORKING=yes

HOSTNAME=co.hs.net

GATEWAY=192.168.1.1

NTPSERVERARGS=iburst

[root@co ~]# cat /etc/sysconfig/network-scripts/ifcfg-eth0 

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

UUID="173ed70d-ace5-4ac1-9505-f0eda4b2090c"

[root@co ~]# cat /etc/sysconfig/network-scripts/ifcfg-br0 

DEVICE="br0"

TYPE="Bridge"

BOOTPROTO="static"

IPADDR="192.168.1.80"

NETMASK="255.255.255.0"

GATEWAY="192.168.1.1"

STP="on"

ONBOOT="yes"

[root@co ~]# cat /etc/sysconfig/network-scripts/ifcfg-

ifcfg-br0   ifcfg-eth0  ifcfg-lo    

[root@co ~]# cat /etc/hosts

127.0.0.1   localhost localhost.localdomain localhost4 localhost4.localdomain4

::1         localhost localhost.localdomain localhost6 localhost6.localdomain6

[root@co ~]# cat /etc/host

host.conf    hosts        hosts.allow  hosts.deny   

[root@co ~]# cat /etc/host.conf 

multi on

[root@co ~]# cat /etc/sysconfig/iptables

# Firewall configuration written by system-config-firewall

# Manual customization of this file is not recommended.

*filter

:INPUT ACCEPT [0:0]

:FORWARD ACCEPT [0:0]

:OUTPUT ACCEPT [0:0]

-A INPUT -m state --state ESTABLISHED,RELATED -j ACCEPT

-A INPUT -p icmp -j ACCEPT

-A INPUT -i lo -j ACCEPT

-A INPUT -m state --state NEW -m tcp -p tcp --dport 21 -j ACCEPT

-A INPUT -m state --state NEW -m tcp -p tcp --dport 22 -j ACCEPT

-A INPUT -m state --state NEW -m tcp -p tcp --dport 16509 -j ACCEPT

-A INPUT -m state --state NEW -m tcp -p tcp --dport 16514 -j ACCEPT

-A INPUT -j REJECT --reject-with icmp-host-prohibited

-A FORWARD -j REJECT --reject-with icmp-host-prohibited

COMMIT

[root@co ~]# cat /etc/sysconfig/ip6tables

# Firewall configuration written by system-config-firewall

# Manual customization of this file is not recommended.

*filter

:INPUT ACCEPT [0:0]

:FORWARD ACCEPT [0:0]

:OUTPUT ACCEPT [0:0]

-A INPUT -m state --state ESTABLISHED,RELATED -j ACCEPT

-A INPUT -p ipv6-icmp -j ACCEPT

-A INPUT -i lo -j ACCEPT

-A INPUT -m state --state NEW -m tcp -p tcp --dport 21 -j ACCEPT

-A INPUT -m state --state NEW -m tcp -p tcp --dport 22 -j ACCEPT

-A INPUT -m state --state NEW -m tcp -p tcp --dport 16509 -j ACCEPT

-A INPUT -m state --state NEW -m tcp -p tcp --dport 16514 -j ACCEPT

-A INPUT -j REJECT --reject-with icmp6-adm-prohibited

-A FORWARD -j REJECT --reject-with icmp6-adm-prohibited

COMMIT

[root@co ~]#