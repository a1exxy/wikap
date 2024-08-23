sudo apt-get install davfs2

В /etc/davfs2/secrets запишем учетки:

echo "/var/webdav/disk-1 Login(e-mail) PASSWORD" > /etc/davfs2/secrets

echo "/var/webdav/disk-2 Login(e-mail) PASSWORD" >> /etc/davfs2/secrets

конфигурационный файл davfs2: /etc/davfs2/davfs2.conf

смонтировать вручную:

sudo mount -t davfs https://webdav.yandex.ru /var/webdav/disk-1

В /etc/fstab:

https://webdav.yandex.ru /var/webdav/disk-1 davfs gid=Login(e-mail),uid=Login(e-mail),noauto 0 0

https://webdav.yandex.ru /var/webdav/disk-2 davfs gid=Login(e-mail),uid=Login(e-mail),noauto 0 0

noauto – данный параметр говорит о том, что WebDaV разделы не будут монтироваться автоматически. Это обязательный параметр, так как в момент загрузки системы и обработки конфига /etc/fstab сетевые подключения еще не готовы.

Создаем каталоги для точек монтирования WebDav, в котрые мы будем монтировать Яндекс.Диски:

mkdir -p \

/var/webdav/disk-1 \

/var/webdav/disk-2

монтируем в ранее подготовленные точки монтирования:

sudo mount /var/webdav/disk-1

sudo mount /var/webdav/disk-2

Для автоматического монтирования при загрузке системы можно добавить команды монтирования в файл /etc/rc.local перед exit 0:

mount /var/webdav/disk-1

mount /var/webdav/disk-2

/////////////////////////////////////////////////////////////////////////////////

Объединение

sudo apt-get install mhddfs

в fstab

mhddfs#/opt/webdav/<YA1>,/opt/webdav/<YA2> /opt/webdav/ya fuse mlimit=100%,logfile=/var/log/mhddfs.log,allow_other 0 0

sudo aptitude install encfs

ENCFS6_CONFIG=/opt/webdav/encfs6.xml \

encfs /opt/webdav/ya/enc \

/opt/webdav/point \

--extpass=" cat /opt/webdav/passwd"

sudo fusermount -u dir