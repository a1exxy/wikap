fdisk /dev/vdb

Command (m for help): n

Partition type

   p   primary (0 primary, 0 extended, 4 free)

   e   extended (container for logical partitions)

Select (default p): p

Partition number (1-4, default 1): 

First sector (2048-419430399, default 2048): 

Last sector, +sectors or +size{K,M,G,T,P} (2048-419430399, default 419430399): 

Created a new partition 1 of type 'Linux' and of size 200 GiB.

Command (m for help): t

Selected partition 1

Partition type (type L to list all types): 8e

Changed type of partition 'Empty' to 'Linux LVM'.

Command (m for help): w

The partition table has been altered.

Calling ioctl() to re-read partition table.

Syncing disks.

root@eva3:~# partprobe

root@eva3:~# fdisk -l /dev/vdb1

root@eva3:~# pvcreate /dev/vdb1

  Physical volume "/dev/vdb1" successfully created

root@eva3:~# pvs

  PV         VG        Fmt  Attr PSize   PFree  

  /dev/vda5  eve-ng-vg lvm2 a--   39.52g      0 

  /dev/vdb1            lvm2 ---  200.00g 200.00g

root@eva3:~# vgs

  VG        #PV #LV #SN Attr   VSize  VFree

  eve-ng-vg   1   2   0 wz--n- 39.52g    0 

root@eva3:~# vgex

vgexport  vgextend  

root@eva3:~# vgextend eve-ng-vg /dev/vdb1

  Volume group "eve-ng-vg" successfully extended

root@eva3:~# 

root@eva3:~# 

root@eva3:~# vgs

  VG        #PV #LV #SN Attr   VSize   VFree  

  eve-ng-vg   2   2   0 wz--n- 239.52g 200.00g

root@eva3:~# vgdisplay 

  --- Volume group ---

  VG Name               eve-ng-vg

  System ID             

  Format                lvm2

  Metadata Areas        2

  Metadata Sequence No  4

  VG Access             read/write

  VG Status             resizable

  MAX LV                0

  Cur LV                2

  Open LV               2

  Max PV                0

  Cur PV                2

  Act PV                2

  VG Size               239.52 GiB

  PE Size               4.00 MiB

  Total PE              61316

  Alloc PE / Size       10117 / 39.52 GiB

  Free  PE / Size       51199 / 200.00 GiB      <<<< ADD FREE

  VG UUID               gOBLpA-ZKjp-3LZC-U9Hh-4Mz4-EA0K-0jLYX1

root@eva3:~# lvs

  LV     VG        Attr       LSize  Pool Origin Data%  Meta%  Move Log Cpy%Sync Convert

  root   eve-ng-vg -wi-ao---- 31.52g                                                    

  swap_1 eve-ng-vg -wi-ao----  8.00g  

lvdisplay eve-ng-vg

  --- Logical volume ---

  LV Path                /dev/eve-ng-vg/root         <<< !!!NAME!!!

  LV Name                root

  VG Name                eve-ng-vg

  LV UUID                njz3z7-lVGm-wuQG-g8zL-XIrH-2Sa5-g47INN

  LV Write Access        read/write

  LV Creation host, time eve-ng, 2018-06-09 10:43:02 +0300

  LV Status              available

  # open                 1

  LV Size                31.52 GiB

  Current LE             8069

  Segments               1

  Allocation             inherit

  Read ahead sectors     auto

  - currently set to     256

  Block device           253:0

   

  --- Logical volume ---

  LV Path                /dev/eve-ng-vg/swap_1

  LV Name                swap_1

  VG Name                eve-ng-vg

  LV UUID                W2G37e-Ckaw-4680-S0gb-c0RQ-ohyq-LsQXe4

  LV Write Access        read/write

  LV Creation host, time eve-ng, 2018-06-09 10:43:02 +0300

  LV Status              available

  # open                 2

  LV Size                8.00 GiB

  Current LE             2048

  Segments               1

  Allocation             inherit

  Read ahead sectors     auto

  - currently set to     256

  Block device           253:1

   

root@eva3:~# lvextend -l +100%FREE /dev/eve-ng-vg/root

  Size of logical volume eve-ng-vg/root changed from 31.52 GiB (8069 extents) to 231.52 GiB (59268 extents).

  Logical volume root successfully resized.

root@eva3:~# 

root@eva3:~# lvdisplay eve-ng-vg

  --- Logical volume ---

  LV Path                /dev/eve-ng-vg/root

  LV Name                root

  VG Name                eve-ng-vg

  LV UUID                njz3z7-lVGm-wuQG-g8zL-XIrH-2Sa5-g47INN

  LV Write Access        read/write

  LV Creation host, time eve-ng, 2018-06-09 10:43:02 +0300

  LV Status              available

  # open                 1

  LV Size                231.52 GiB   <<<< !!!NEW!!!

  Current LE             59268

  Segments               2

  Allocation             inherit

  Read ahead sectors     auto

  - currently set to     256

  Block device           253:0

root@eva3:~# resize2fs /dev/eve-ng-vg/root

resize2fs 1.42.13 (17-May-2015)

Filesystem at /dev/eve-ng-vg/root is mounted on /; on-line resizing required

old_desc_blocks = 2, new_desc_blocks = 15

The filesystem on /dev/eve-ng-vg/root is now 60690432 (4k) blocks long.

root@eva3:~# 

root@eva3:~# df -h

Filesystem                    Size  Used Avail Use% Mounted on

udev                           16G     0   16G   0% /dev

tmpfs                         3.2G   13M  3.2G   1% /run

/dev/mapper/eve--ng--vg-root  228G  2.6G  216G   2% /      <<< !!!NEW!!!