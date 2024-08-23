Обычный конфиг для копирования:

network:   ethernets:     ens4:       dhcp4: true         ens3:       dhcp4: false       addresses: [172.16.0.1/24]       #gateway4:       #nameservers:       #  addresses: [1.1.1.1]   version: 2

В случае применения DHCP простейшая конфигурация netplan будет выглядеть следующим образом:

    network:      version: 2      ethernets:         enp3s0:             dhcp4: yes 

Более сложный пример:

  network:       version: 2        ethernets:         id0:           match:             macaddress: 00:11:22:33:44:55           wakeonlan: true           dhcp4: true           addresses:             - 192.168.14.2/24             - 2001:1::1/64           gateway4: 192.168.14.1           gateway6: 2001:1::2           nameservers:             search: [foo.local, bar.local]             addresses: [8.8.8.8]         lom:           match:             driver: ixgbe           set-name: lom1           dhcp6: true         switchports:           match:             name: enp2*           mtu: 1280       wifis:         all-wlans:           match: {}           access-points:             "Joe's home":               password: "s3kr1t"         wlp1s0:           access-points:             "guest":                mode: ap                channel: 11       bridges:         br0:           interfaces: [wlp1s0, switchports]           dhcp4: true       routes:        - to: 0.0.0.0/0          via: 11.0.0.1          metric: 3

Tag + ubtag:

network:     version: 2     ethernets:         eth0:             dhcp4: no     vlans:         vl10:             id: 10             link: br0         vl20:             id: 20             link: br0      bridges:         br0:             interfaces: [ eth0 ]             dhcp4: no             addresses: [ 10.68.216.243/24 ]             gateway4: 10.68.216.1         br0.10:             interfaces: [ vl10 ]         br0.20:             interfaces: [ vl20 ]

------------------------------------------------------------

From GIGA

network:     ethernets:         enp6s0:             dhcp4: no         vlans:         vl17:             id: 17             link: br0          vl500:             id: 500             link: br0          vl501:             id: 501             link: br0                                   vl101:             id: 101             link:  br0            vl202:             id: 202             link:  br0         bridges:         br0:             dhcp4: no             addresses: [ 192.168.1.102/24 ]             gateway4: 192.168.1.100             nameservers:                 addresses:                 - 192.168.1.100                 search:                 - hs.net              interfaces:             - enp6s0          br0.17:             interfaces: [ vl17 ]           br0.500:             interfaces: [ vl500 ]          br0.501:             interfaces: [ vl501 ]          br0.101:             interfaces: [ vl101 ]         br0.202:             interfaces: [ vl202 ]                       version: 2