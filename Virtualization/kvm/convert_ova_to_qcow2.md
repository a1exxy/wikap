Extract the .ova file

$ tar -xvf file.ova

Convert the .vmdk to .qcow2

$ qemu-img convert -O qcow2 file.vmdk file.qcow2