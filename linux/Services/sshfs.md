yum install fuse-sshfs

[ipam@ipamtest ~]$ cat mount_arpa.sh

#!/bin/sh

sshfs -o reconnect -o allow_root -o fsname=ARPA ns.com.net:/var/named/chroot/var/named/master/arpa /home/ipam/arpa

[ipam@ipamtest ~]$ cat mount_6arpa.sh 

#!/bin/sh

sshfs -o reconnect -o allow_root -o fsname=ARPA6 ns.com.net:/var/named/chroot/var/named/6arpa /home/ipam/6arpa

