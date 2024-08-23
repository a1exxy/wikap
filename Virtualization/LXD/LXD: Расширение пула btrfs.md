LXD: Расширение пула btrf:

Процедура:

sudo truncate -s +5G /var/lib/lxd/disks/<POOL>.img

sudo losetup -c <LOOPDEV>

sudo btrfs filesystem resize max /var/lib/lxd/storage-pools/<POOL>/

=========================================================

root@hostname:/var/lib/lxd/disks# btrfs filesystem show 

Label: 'default'  uuid: 552ce885-db9b-4f3a-ac2b-212c0de679de

Total devices 1 FS bytes used 128.37GiB

devid    1 size 139.70GiB used 136.02GiB path /dev/loop2   <<<< это LOOPDEV

root@hostname:/var/lib/lxd/disks# sudo truncate -s +50G /var/lib/lxd/disks/default.img

sudo losetup -c /dev/loop2

root@hostname:/var/lib/lxd/disks# btrfs filesystem resize max /var/lib/lxd/storage-pools/default/

Resize '/var/lib/lxd/storage-pools/default/' of 'max'

root@hostname:/var/lib/lxd/disks# lxc storage show default

config:

  size: 150GB

  source: /var/lib/lxd/disks/default.img

root@hostname:/var/lib/lxd/disks# btrfs filesystem show 

Label: 'default'  uuid: 552ce885-db9b-4f3a-ac2b-212c0de679de

Total devices 1 FS bytes used 128.37GiB

devid    1 size 189.70GiB used 136.02GiB path /dev/loop2

btrfs qgroup show /var/lib/lxd/storage-pools/default

ERROR: can't list qgroups: quotas not enabled    <<< квота отключена