Просмотр всех доменов(виртуалок), включая выключенных:

    virsh list --all

Запуск домена:

    virsh start <имя домена>

Отключение питания у домена:

    virsh destroy <имя домена>

Подключение к консоли:

    virsh console <имя домена>

Отключение от консоли:

    Ctrl+]

Просмотр конфига домена:

    virsh dumpxml <имя домена>

Изменение конфигурации домена:

    virsh edit <имя домена>

Помощь:

    virsh help