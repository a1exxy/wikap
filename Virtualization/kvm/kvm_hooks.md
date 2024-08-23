mkdir /etc/libvirt/hooks

cat /etc/libvirt/hooks/qemu

#!/bin/bash

# Documentation  https://www.libvirt.org/hooks.html

Interface1='macvtap0'

Interface2='macvtap1'

#if [ "$2" == "started" ]; then

 timestamp=$(date +"%Y-%m-%d %H:%M:%S")

 exists=$(ifconfig | grep $Interface1 | wc -l)

 if [ "$exists" -gt "0" ]; then

   ifconfig $Interface1 allmulti

   echo "$timestamp ALLMULTI set on $Interface1" >> /var/log/libvirt/libvirt_hook_qemu.log

 fi

 exists=$(ifconfig | grep $Interface2 | wc -l)

 if [ "$exists" -gt "0" ]; then

   ifconfig $Interface2 allmulti

   echo "$timestamp ALLMULTI set on $Interface2" >> /var/log/libvirt/libvirt_hook_qemu.log

 fi

#fi

ifconfig em2 mtu 9000

ifconfig em4 mtu 9000

=========================

version 2:

#cat /etc/libvirt/hooks/qemu

#!/bin/bash

for L in $(ip address | grep -E macvtap | cut -d" " -f 2 | cut -d@ -f1)

do

    ifconfig $L allmulti

done

=========================

chmod +x /etc/libvirt/hooks/qemu