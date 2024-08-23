Скачать ova c eve-ng.net

Extract the .ova file

$ tar -xvf file.ova

Convert the .vmdk to .qcow2

$ qemu-img convert -O qcow2 file.vmdk file.qcow2

sudo virt-install -n EVE -r 16386 --vcpus=8 --accelerate --os-type=linux --os-variant=ubuntu16.04 --disk path=/var/lib/libvirt/images/eve.qcow2,bus=virtio  --network bridge=virbr0,model=virtio --graphics vnc,listen=0.0.0.0  -v

sudo virt-install -n EVE -r 16386 --vcpus=8 --accelerate --os-type=linux --os-variant=ubuntu16.04 --disk path=/var/lib/libvirt/images/eve.qcow2,bus=virtio  --network bridge=virbr0,model=virtio --graphics vnc,listen=0.0.0.0 --import  -v

Проверить

$ cat /sys/module/kvm_intel/parameters/nested

Y

в секцию CPU

<feature policy='require' name='vmx'/>