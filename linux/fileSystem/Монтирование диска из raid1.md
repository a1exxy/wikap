# Монтирование диска из raid1

apt install mdadm



## Информация о RAID

cat /proc/mdstat

#### Информация о диске

mdadm -Q --examine  /dev/sda2

## Создание файла mdadm.conf

mkdir /etc/mdadm

echo "DEVICE partitions" > /etc/mdadm/mdadm.conf

mdadm --detail --scan --verbose | awk '/ARRAY/ {print}' >> /etc/mdadm/mdadm.conf



DEVICE partitions

ARRAY /dev/md0 level=raid1 num-devices=2 metadata=1.2 name=proxy.dmosk.local:0 UUID=411f9848:0fae25f9:85736344:ff18e41d



#### Fdisk

fdisk -l /dev/sda

...

/dev/sda2     3147776 3904929899 3901782124  1.8T Microsoft basic data

...



#### Сканирование

root@srv:~# mdadm --assemble --readonly  --run  --scan



#### Добавление

root@srv:~# mdadm --assemble --readonly  --run /dev/md126 /dev/sda2

mdadm: /dev/md126 has been started with 1 drive (out of 2).