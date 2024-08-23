Ubuntu 18.04 Server Cloud

wget https://cloud-images.ubuntu.com/bionic/current/bionic-server-cloudimg-amd64.img

cat >user-data <<EOF

#cloud-config

password: ubuntu

chpasswd: { expire: False }

ssh_pwauth: True

EOF

sudo apt-get install cloud-image-utils

cloud-localds user-data.img user-data

# user-data.img MUST come after the rootfs. 

qemu-system-x86_64 \

-drive file=ubuntu-18.04-server-cloudimg-amd64.img,format=qcow2 \

-drive file=user-data.img,format=raw

или через virt-manager подключить второй hdd

Сброс пароля...

virt-sysprep -d bionic // имя машины в kvm