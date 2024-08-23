CentOS-7-x86_64-Minimal-1511.iso

yum remove NetworkManager

echo 'proxy=http://10.77.127.254:3128/' >> /etc/yum.conf

yum update

yum install -y mc nano vim wget open-ssh openssh-clients man bind-utils bzip2 unzip zip sysstat bash-completion vnstat net-tools lsof tcpdump

/etc/selinux/config => SELINUX=disabled

yum  install -y kvm libvirt python-virtinst qemu-kvm bridge-utils virt-install

reboot

scp -v jinstall64-vrr-15.1F6.9-domestic.img root@10.146.128.131:/var/lib/libvirt/images/

virt-install --name mskn41rr --ram 8192 --import --disk=/var/lib/libvirt/images/jinstall64-vrr-15.1F6.9-domestic.img

 virt-install --name brl71rr --ram 16384 --import --disk=/var/lib/libvirt/images/junos-x86-64-16.1R5-S1.img  --import --disk=/var/lib/libvirt/images/metadata.img

 virt-install --name brl71rr --ram 16384 --import --disk=/var/lib/libvirt/images/junos-x86-64-16.2R2.8.img  --import --disk=/var/lib/libvirt/images/metadata.img

virsh edit mskn41rr

    <interface type='direct' trustGuestRxFilters='no'>

      <mac address='52:54:00:e6:99:a5'/>

      <source dev='em2' mode='bridge'/>

      <model type='virtio'/>

      <address type='pci' domain='0x0000' bus='0x00' slot='0x03' function='0x0'/>

    </interface>

    <interface type='direct' trustGuestRxFilters='no'>

      <mac address='52:54:00:e6:99:a6'/>

      <source dev='em4' mode='bridge'/>

      <model type='virtio'/>

      <address type='pci' domain='0x0000' bus='0x00' slot='0x08' function='0x0'/>

    </interface>

===================================

    <interface type='direct' trustGuestRxFilters='no'>

      <mac address='52:54:00:e6:99:a7'/>

      <source dev='bond0.71' mode='bridge'/>

      <target dev='macvtap0'/>

      <model type='virtio'/>

      <alias name='net0'/>

      <address type='pci' domain='0x0000' bus='0x00' slot='0x03' function='0x0'/>

    </interface>

    <interface type='direct' trustGuestRxFilters='no'>

      <mac address='52:54:00:e6:99:a7'/>

      <source dev='bond1.71' mode='bridge'/>

      <target dev='macvtap1'/>

      <model type='virtio'/>

      <alias name='net1'/>

      <address type='pci' domain='0x0000' bus='0x00' slot='0x11' function='0x0'/>

    </interface>

===================================

virsh autostart mskn41rr

kvm_hooks

reboot

==========================================================

    <interface type='direct' trustGuestRxFilters='no'>

      <mac address='52:54:00:e6:99:a5'/>

      <source dev='em2' mode='bridge'/>

      <target dev='macvtap0'/>

      <model type='virtio'/>

      <alias name='net0'/>

      <address type='pci' domain='0x0000' bus='0x00' slot='0x03' function='0x0'/>

    </interface>

    <interface type='direct' trustGuestRxFilters='no'>

      <mac address='52:54:00:e6:99:a6'/>

      <source dev='em1' mode='bridge'/>

      <target dev='macvtap1'/>

      <model type='virtio'/>

      <alias name='net1'/>

      <address type='pci' domain='0x0000' bus='0x00' slot='0x08' function='0x0'/>

    </interface>