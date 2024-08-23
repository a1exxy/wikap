# Загружаем модуль ядра Network Block Device modprobe nbd  # "Подключаем" образ к устройству /dev/nbd0. qemu-nbd --connect /dev/nbd0 --read-only /путь/к/образу.qcow2  # Ищем разделы на устройстве. kpartx -arvs /dev/nbd0  # Здесь ты можешь делать с разделами /dev/mapper/ndb0p* что угодно: монтировать, форматировать и т.п.  # Убираем девайсы разделов. kpartx -dvs /dev/nbd0  # Выключаем qemu-nbd. qemu-nbd --disconnect /dev/nbd0

modprobe nbd max_part=8

qemu-nbd -c /dev/nbd0 название_образа.qcow2

mkdir /mnt/qemu

mount /dev/nbd0p1 /mnt/qemu

Диск монтируется в режиме чтения-записи. Чтобы отмонтировать диск и освободить ресурсы выполним обратную операцию:

umount /mnt/qemu

rm -R /mnt/qemu

qemu-nbd -d /dev/nbd0

modprobe -r nbd