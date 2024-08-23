Ubuntu:

sudo ufw allow in proto udp to 224.0.0.0/4

sudo ufw allow in proto udp from 224.0.0.0/4

vlc -vvv /path/to/file.avi —sout '#standard{access=udp{ttl=15},mux=ts{tsid=22,pid-video=23,pid-audio=24,pid-pmt=25,use-key-frames},dst=239.255.1.1}' —random —loop —volume 100

Включение мультикаста на интерфейсе

ifconfig $Interface allmulti

Подписка к группе с сервера:

apt install smcroute # установка пакета

smcroute -j ens17 233.12.144.9 // подключение к группе

smcroute -l ens17 233.12.144.9 // отключение от группы

Просмотр подписок:

netstat -g