sudo virt-install -n collector1 -r 1024 --vcpus=1 --accelerate --os-type=linux --os-variant=rhel6 --disk path=/var/lib/libvirt/images/collector1.img,bus=virtio,size=20 -c  /var/lib/libvirt/images/CentOS-6.7-x86_64-minimal.iso --network bridge=br0,model=virtio --graphics vnc,listen=0.0.0.0  -v

sudo virt-install -n cloudera -r 8192 --vcpus=16 --accelerate --os-type=linux --os-variant=rhel6 --disk path=/var/lib/libvirt/images/cloudera.img,bus=virtio,size=40 -c  /var/lib/libvirt/images/CentOS-6.7-x86_64-minimal.iso --network bridge=br0,model=virtio --graphics vnc,listen=0.0.0.0  -v

sudo virt-install -n lake01 -r 8192 --vcpus=16 --accelerate --os-type=linux --os-variant=ubuntu16.04 --disk path=/var/lib/libvirt/images/lake01.img,bus=virtio,size=100 -c  /var/lib/libvirt/images/ubuntu-16.04.2-server-amd64.iso --network bridge=virbr0,model=virtio --graphics vnc,listen=0.0.0.0  -v

Clone

virt-clone -o ubuntu_base_20 -n ceph-mon01 -f /var/lib/libvirt/images/ceph-mon01.img

virsh dumpxml vm1 > /tmp/vm3-template.xml

virsh define /tmp/vm3-template.xml

Virsh console enable:

$ sudo systemctl enable serial-getty@ttyS0.service

$ sudo systemctl start serial-getty@ttyS0.service