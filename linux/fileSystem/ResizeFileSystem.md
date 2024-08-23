Просмотр структуры:

    lsblk

===================Расширение qcow2===========================

qemu-img resize vm.qcow2 +5GB

============Пересоздание раздела через fdisk==================

$ fdisk /dev/sda

Command (m for help): p

   Device Boot      Start         End      Blocks   Id  System

/dev/sda1   *        2048     9437183     4717568   83  Linux

Command (m for help): d

Selected partition 1

Command (m for help): p

   Device Boot      Start         End      Blocks   Id  System

Command (m for help): n

Command action

   e   extended

   p   primary partition (1-4)

p

Partition number (1-4, default 1): 1

First sector (2048-10485759, default 2048):

Using default value 2048

Last sector, +sectors or +size{K,M,G} (2048-10485759, default 10485759):

Using default value 10485759

Command (m for help): p

   Device Boot      Start         End      Blocks   Id  System

/dev/sda1            2048    10485759     5241856   83  Linux

Command (m for help): w

The partition table has been altered!

Calling ioctl() to re-read partition table.

WARNING: Re-reading the partition table failed with error 16: Device or resource busy.

The kernel still uses the old table. The new table will be used at

the next reboot or after you run partprobe(8) or kpartx(8)

Syncing disks.

partprobe

=========Расширение физического раздела LVM =================

  pvresize /dev/sda1

=========Расширение логического раздела LVM =================

  # забирает всё свободное место с sda1

  

  lvextend /dev/ubuntu-vg/ubuntu-lv /dev/sda1 

=========Расширение файловой системы=========================

  resize2fs /dev/mapper/ubuntu--vg-ubuntu--lv

=========Альтернатива===================

# Создание физического раздела LVM 

pvcreate /dev/sdb1

# Добавление раздела в группу

vgextend VolGroup00 /dev/sdb1

# Расширение логического раздела на 10G

lvextend -L +10G /dev/mapper/VolGroup00-LogVol00

# Расширение логического раздела на 100% свободного месте

lvextend -l +100%FREE /dev/mapper/VolGroup00-LogVol00

# до нужного объема:

lvextend -L500G /dev/vg01/lv01

======================================================

Расширение файловых систем:

ext2/ext3/ext4:

resize2fs /dev/vg01/lv01

XFS:

xfs_growfs /dev/vg01/lv01

Reiserfs:

resize_reiserfs /dev/vg01/lv01