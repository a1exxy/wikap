Поиск:

iscsiadm -m discovery -t sendtargets -p 10.0.0.30

коротко:

iscsiadm -m discovery -t st -p 10.0.0.30

Подключение:

iscsiadm --mode node --targetname iqn.2013-10.linuxspace.server:target0 --portal 10.0.0.30 --login

коротко:

iscsiadm -m node -T iqn.2013-10.linuxspace.server:target0 -p 10.0.0.30 -l

Отключениие:

iscsiadm -m node -T iqn.2013-10.linuxspace.server:target0 -p 10.0.0.30 -u

Удаление:

iscsiadm -m node -T iqn.2013-10.linuxspace.server:target0 -p 10.0.0.30 -o delete

CO6

[root@frtvsi02 iscsi]# iscsiadm -m discovery -t st -p 10.149.128.225

Запускается iscsid:                                        [  OK  ]

10.149.128.225:3260,1 iqn.2001-05.com.equallogic:0-1cb196-df4f04432-491004efabc56b83-frt-cloudera-node1

10.149.128.225:3260,1 iqn.2001-05.com.equallogic:0-1cb196-fe5f04432-6ed004efabf56b83-frt-vm-pool

[root@frtvsi02 iscsi]# iscsiadm -m node -T iqn.2001-05.com.equallogic:0-1cb196-fe5f04432-6ed004efabf56b83-frt-vm-pool -p 10.149.128.225 -l

Logging in to [iface: default, target: iqn.2001-05.com.equallogic:0-1cb196-fe5f04432-6ed004efabf56b83-frt-vm-pool, portal: 10.149.128.225,3260] (multiple)

Login to [iface: default, target: iqn.2001-05.com.equallogic:0-1cb196-fe5f04432-6ed004efabf56b83-frt-vm-pool, portal: 10.149.128.225,3260] successful.

Ubuntu 16.04

1. !!!!  Only first !!!!  else use iscsiadm -u 

/etc/iscsi/iscsid.conf    

node.startup = manual  ==>> node.startup = automatic

2. iscsiadm -m discovery -t st -p 10.0.0.30

3. iscsiadm -m node -T iqn.2013-10.linuxspace.server:target0 -p 10.0.0.30 -l

4. fdisk -l

5. mkfs /dev/sdX

6. blkid

7.

Add to /etc/fstab

UUID="..."   /mnt_point    type_of_FS    defaults,_netdev   0  0