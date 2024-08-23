cat /etc/systemd/system/csmserver.service

[Unit]

Description=csmserver

After=syslog.target

After=network.target

After=mysql.service

Requires=mysql.service

[Service]

Type=forking

ExecStart=/usr/local/csm/csmserver/csmserver start

ExecStop=/usr/local/csm/csmserver/csmserver stop

[Install]

WantedBy=multi-user.target 

Перезагрузка демонов:

systemctl daemon-reload

/usr/lib/systemd/system/ – юниты из установленных пакетов RPM — всякие nginx, apache, mysql и прочее

/run/systemd/system/ — юниты, созданные в рантайме — тоже, наверное, нужная штука

/etc/systemd/system/ — юниты, созданные системным администратором — а вот сюда мы и положим свой юнит.