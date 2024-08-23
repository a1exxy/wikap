1) Переходим в /var/lib/libvirt/images/

2) sudo virt-sysprep -a Centos-7-x86_64-GenericCloud.qcow2 --root-password password:super

где super это пароль root

3) Создаем виртуальную машину на основе этого образа

4) Логинимся со своим паролем

Установка virt-sysprep в xUbuntu 16.04

apt install libguestfs-tools