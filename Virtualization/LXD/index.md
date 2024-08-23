Конфиг прокси:

lxc config set core.proxy_http http://10.77.127.254:3128/

lxc config set core.proxy_https http://10.77.127.254:3128/

lxc config set core.proxy_ignore_hosts image-server.local

Настройка lxd хоста на прослушивание сети:

lxc config set core.https_address [::]

lxc config set core.trust_password <some-secret-string>

Снапшоты:

lxc snapshot   CONT1   snap1 # для конейнера CONT1 делаем снапшот snap1

lxc restore   CONT1   snap1      # восстанавливаем контейнер CONT1 из снапшота snap1

Бекап:

Бекап контейнера CONT1:

lxc snapshot   CONT1   CONT1_backup                                            # делаем снапшот

lxc publish   CONT1/CONT1_backup   --alias   CONT1_backup # публикуем образ

lxc image export   CONT1_backup  .                                      # экспортируем тарбол в текущую директорию

lxc image delete   CONT1_backup                                                      # удаляем образ

# по умолчанию имя тарбола равно фингерпринту

Восстановление CONT1:

lxc image import   TARBALL-NAME   --alias   CONT1_restored # импортируем

lxc launch   CONT1_restored   CONT1                                               # создаем контейнер из образа

lxc image delete   CONT1_restored                                                     # удаляем образ