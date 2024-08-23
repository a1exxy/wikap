    root@hostname:~# lxc config show nfs
```yaml
architecture: x86_64
config:
  image.architecture: amd64
  image.description: ubuntu 18.04 LTS amd64 (release) (20200518.1)
  image.label: release
  image.os: ubuntu
  image.release: bionic
  image.serial: "20200518.1"
  image.version: "18.04"
  raw.lxc: lxc.apparmor.profile=unconfined
  security.privileged: "yes"
  volatile.base_image: 5539cdd71a7b2f56a75d9bb8f45c70b6c1618217ae4df5977215c5636bf8adce
  volatile.eth0.hwaddr: 00:16:3e:a2:b4:18
  volatile.idmap.base: "0"
  volatile.idmap.next: '[]'
  volatile.last_state.idmap: '[]'
  volatile.last_state.power: RUNNING
devices: {}
ephemeral: false
profiles:
  - default
stateful: false
description: ""
```
   
```shell
sudo apt install nfs-kernel-server
```
```shell
cat /etc/netplan/50-cloud-init.yaml
```    
```yaml
network:
    version: 2
    ethernets:
        eth0:
            dhcp4: false
            addresses: [ 10.164.82.3/24 ]
            gateway4: 10.164.82.1
            nameservers:
                addresses: [ 1.1.1.1 ]
```                

================================
```shell
cat /etc/exports 

/opt 12.64.128.0/255.255.252.0(rw,sync) 9.37.5.1(rw,sync)
```
```shell
chmod -R 777 /opt/
```