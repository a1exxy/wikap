cat /etc/sysconfig/iptables

# Firewall configuration written by system-config-firewall

# Manual customization of this file is not recommended.

*nat

:PREROUTING ACCEPT [87:14062]

:POSTROUTING ACCEPT [24:1682]

:OUTPUT ACCEPT [37:2496]

-A POSTROUTING -o eth1 -j MASQUERADE

COMMIT

*filter

:INPUT ACCEPT [0:0]

:FORWARD ACCEPT [0:0]

:OUTPUT ACCEPT [0:0]

-A INPUT -m state --state ESTABLISHED,RELATED -j ACCEPT

-A INPUT -p icmp -j ACCEPT

-A INPUT -i lo -j ACCEPT

-A INPUT -m state --state NEW -m tcp -p tcp --dport 22 -j ACCEPT

-A INPUT -s 192.168.1.0/24 -m state --state NEW -m tcp -p tcp --dport 3389 -j ACCEPT

-A INPUT -s 192.168.1.0/24 -m state --state NEW -m tcp -p tcp --dport 22 -j ACCEPT

-A INPUT -s 192.168.1.0/24 -m state --state NEW -m tcp -p tcp --dport 3128 -j ACCEPT

-A INPUT -s 192.168.1.0/24 -m state --state NEW  -p tcp --dport 53 -j ACCEPT

-A INPUT -s 192.168.1.0/24 -m state --state NEW  -p udp --dport 53 -j ACCEPT

-A INPUT -s 192.168.1.0/24 -m state --state NEW  -p tcp --dport 445 -j ACCEPT

-A INPUT -s 192.168.1.0/24 -m state --state NEW  -p udp --dport 445 -j ACCEPT

-A INPUT -s 192.168.1.0/24 -m state --state NEW  -p udp --dport 123 -j ACCEPT

-A INPUT -s 192.168.1.0/24 -m state --state NEW  -p tcp --dport 143 -j ACCEPT

-A INPUT -s 192.168.1.0/24 -m state --state NEW  -p tcp --dport 25 -j ACCEPT

-A INPUT -s 192.168.1.0/24 -m state --state NEW  -p tcp --dport 110 -j ACCEPT

-A INPUT -j REJECT --reject-with icmp-host-prohibited

#-A FORWARD -j REJECT --reject-with icmp-host-prohibited

-A FORWARD -m state --state ESTABLISHED,RELATED -j ACCEPT

-A FORWARD -m state --state NEW -i eth0 -s 192.168.1.32/28 -j ACCEPT

-A FORWARD -m state --state NEW -i eth0 -s 192.168.1.112/28 -j ACCEPT   

-P FORWARD DROP

COMMIT

cat /etc/sysconfig/iptables

# Firewall configuration written by system-config-firewall

# Manual customization of this file is not recommended.

*filter

:INPUT ACCEPT [0:0]

:FORWARD ACCEPT [0:0]

:OUTPUT ACCEPT [0:0]

-N HOSTS

-A HOSTS -s 200.100.35.243/32 -j ACCEPT

-A HOSTS  -s 70.107.200.131/32 -j ACCEPT

-A INPUT -m state --state ESTABLISHED,RELATED -j ACCEPT

-A INPUT -p icmp -j ACCEPT

-A INPUT -i lo -j ACCEPT

-A INPUT -m state --state NEW -m tcp -p tcp --dport 22 -j HOSTS

-A INPUT  -p tcp --dport 53 -j ACCEPT

-A INPUT  -p udp --dport 53 -j ACCEPT

-P INPUT DROP

#-A FORWARD -j REJECT --reject-with icmp-host-prohibited

COMMIT

http://www.linuxspace.org/archives/4645
Фаерволы продолжение… Часть 2
Как и обещал продолжаю сагу о фаерволах. В предыдущей статье мы рассмотрели работу ufw и разобрали некоторые простые примеры. Сегодня речь пойдет об IPtables. Я не буду углублятся в принципы работы, это не википедия, зато покажу несколько реально полезных примером, которые помогут вам обезапасить сервер. Настройки которые будут предложены ниже используются в основном на серверах расположенных в зоне MZ или же на домашних машинах.

Я имею ввиду, что для серьезных продакшн серверов настройки фаерволов должны быть более тонкими и гибкими, чем я предложу вам, но это уже дело каждого. Например на крупных серверах есть защита против ддосов, брут форсов и прочего. Кстати опцию как защитить 22 порт от брут форса я привел в прошлой статье. Примеры будут отображать настройку на двух системах, на Ubuntu\Debian и на Fedora 17. Для других дистрибутивов могут быть отличия. Если интересно, то поехали, вся необходимая инфа в продолжении.

Настройка IPtables в Ubuntu 12.04\Debian
Мой домашний сервер управляется системой Ubuntu 12.04 и он же смотрит в мир (т.е. у него есть интерфейс к которому привязан внешний IP) так же многие серверы за которые я был ответсвенный в армии и на работе так же работают под управлением Ubuntu 10.04 or 10.12 Server.

Так как настроить IPtables, с чего наать? Начать надо с определения политик безопасности. Как было сказано ранее, в предыдущей статье, я придерживаю такой политики:

- Allow all outgoing connections (разрешить ВСЕ исходящие)

- Allow established connections (разрешить ВСЕ установленные)

- Deny all incoming connections (запретить ВСЕ входящие, т.е. все кроме того что мы откроем должно пресекаться на корню без суда и следствия)

- Deny all forward connections (запретить форвардинг)

Остальное уже настраивается по вкусу.

В Ubuntu\Debian по умолчанию фаервол отключен. Проверить статус и посмотреть активыне правила можно так:

1 2 3

$ sudo iptables -L $ sudo iptables -L -v $ sudo iptables -n -L -v --line-numbers

Сбросить все установленные прежде правила можно так:

1

$ sudo iptables -F

Создаем файл с правилами:

1

$ vi /etc/iptables.rules

Туда вносим следующие правила:

1 2 3 4 5 6 7 8 9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 27 28 29 30 31 32 33 34 35

*filter   # Allows all loopback (lo0) traffic and drop all traffic to 127/8 that doesn't use lo0-A INPUT -i lo -j ACCEPT -A INPUT ! -i lo -d 127.0.0.0/8 -j REJECT   # Accepts all established inbound connections-A INPUT -m state --state ESTABLISHED,RELATED -j ACCEPT   # Allows all outbound traffic# You could modify this to only allow certain traffic-A OUTPUT -j ACCEPT   # Allows HTTP and HTTPS connections from anywhere (the normal ports for websites)-A INPUT -p tcp --dport 80 -j ACCEPT -A INPUT -p tcp --dport 443 -j ACCEPT   # Allows SSH connections # THE -dport NUMBER IS THE SAME ONE YOU SET UP IN THE SSHD_CONFIG FILE-A INPUT -p tcp -m state --state NEW --dport 30000 -j ACCEPT   # Now you should read up on iptables rules and consider whether ssh access # for everyone is really desired. Most likely you will only allow access from certain IPs.   # Allow ping-A INPUT -p icmp -m icmp --icmp-type 8 -j ACCEPT   # log iptables denied calls (access via 'dmesg' command)-A INPUT -m limit --limit 5/min -j LOG --log-prefix "iptables denied: " --log-level 7   # Reject all other inbound - default deny unless explicitly allowed policy:-A INPUT -j REJECT -A FORWARD -j REJECT   COMMIT

Теперь активируем правила:

1

$ sudo iptables-restore < /etc/iptables.rules

Смотрим на результат:

1 2 3 4 5 6 7 8 9 10 11 12 13 14 15 16 17 18 19 20 21

$ sudo iptables -L   Chain INPUT (policy ACCEPT) target     prot opt source               destination ACCEPT     all  --  anywhere             anywhere REJECT     all  --  anywhere             127.0.0.0/8          reject-with icmp-port-unreachable ACCEPT     all  --  anywhere             anywhere             state RELATED,ESTABLISHED ACCEPT     tcp  --  anywhere             anywhere             state NEW tcp dpt:ssh ACCEPT     icmp --  192.168.0.0/16       anywhere             icmp echo-request LOG        all  --  anywhere             anywhere             limit: avg 5/min burst 5 LOG level debug prefix "iptables denied: " REJECT     all  --  anywhere             anywhere             reject-with icmp-port-unreachable   Chain FORWARD (policy ACCEPT) target     prot opt source               destination ACCEPT     all  --  anywhere             anywhere             state RELATED,ESTABLISHED ACCEPT     all  --  anywhere             anywhere REJECT     all  --  anywhere             anywhere             reject-with icmp-port-unreachable   Chain OUTPUT (policy ACCEPT) target     prot opt source               destination ACCEPT     all  --  anywhere             anywhere

Cохраняем правила:

1

$ sudo iptables-save > /etc/iptables.up.rules

Что-бы правила активировались после перезагрузки, делаем такой скрипт:

1 2 3 4

$ sudo vi /etc/network/if-pre-up.d/iptables   #!/bin/bash/sbin/iptables-restore < /etc/iptables.up.rules

Даем скрипту права на выполнения:

1

$ sudo chmod +x /etc/network/if-pre-up.d/iptables

Пояснения некоторых правил:

Разрешить исходящие установленные соединения:

1

-A INPUT -m state --state ESTABLISHED,RELATED -j ACCEPT

Разрешить весь исходящий траффик:

1

-A OUTPUT -j ACCEPT

Разрешить соединения на порт 80,443:

1 2

-A INPUT -p tcp --dport 80 -j ACCEPT -A INPUT -p tcp --dport 443 -j ACCEPT

Запретить все входящие соединения и форвардинг:

1 2

-A INPUT -j REJECT -A FORWARD -j REJECT

Универсальное правило, на разрешение пинга:

1

-A INPUT -p icmp -m icmp --icmp-type 8 -j ACCEPT

Разрешить SSH соединения на порту 30000 (протокол TCP):

1

-A INPUT -p tcp -m state --state NEW --dport 30000 -j ACCEPT

Это не полное объяснение, но по чуть-чуть картина сложится:

Настройка IPtables в Fedora 17
В Fedora 17 правила все теже, но их настройка и активация чуть иная. Тут все правила пачкой прописываются в файл: /etc/sysconfig/iptables

После чего делается стандартные рестарт на сервис:

1

# /etc/init.d/iptables restart

Или

1

# systemctl restart iptables.service

Или

1

# service iptables restart

Что-бы фаервол стартовал с системой делаем так:

1

# chkconfig iptables on

Некоторые примеры
Разрешить подключение к порту 22 только с определенной сети:

1

-A INPUT -m state --state NEW -m tcp -p tcp --source 192.168.98.0/24 --dport 22 -j ACCEPT

Закрыть пинг:

1

-I INPUT -i eth0 -p icmp -s 0/0 -d 0/0 -j DROP

Закрыть пинг на внешнем интерфейсе eth0:

1 2 3

-A INPUT -p icmp --icmp-type echo-reply -s 0/0 -i eth0 -j DROP -A INPUT -p icmp --icmp-type destination-unreachable -s 0/0 -i eth0 -j DROP -A INPUT -p icmp --icmp-type time-exceeded -s 0/0 -i eth0 -j DROP

Закрыть пинг на любом интерфейсе:

1

-A INPUT -p icmp -m icmp --icmp-type 8 -j DROP

Забанить IP адрес:

1

-A INPUT -s 65.55.44.100 -j DROP

Забанить доступ к 21 порту для определенного IP:

1

-A INPUT -s 65.55.44.100 -p tcp --destination-port 25 -j DROP

Забанить целую подсеть:

1

-A INPUT -s 192.168.98.0/24 -j DROP

Запретить все соединения на 80 порт (все интерфейсы, протокол TCP):

1

-A INPUT -p tcp --dport 80 -j DROP

Запретить все соединения на 80 порт внешнего интерфейса eth1, протокол TCP

1

-A INPUT -i eth1 -p tcp --dport 80 -j DROP

Закрыть весь исходящий трафик по направлению к неугодному IP:

1

-A OUTPUT -d <IP ADDRESS> -j DROP

К примеру я хочу забанить сайт www.facebook.com на шлюзе, что-бы с офиса не было к нему доступа:

1 2 3 4 5

# sudo nslookup facebook.com   Name:   facebook.com Address: 173.252.100.16 Name:   facebook.com

Добавляю правило:

1

-A OUTPUT -d 173.252.100.16 -j DROP

Но это забанит только один из серверов, а мы хитрые, так что чекаем подсеть:

1 2 3

# host -t a www.facebook.com www.facebook.com is an alias for star.facebook.com. star.facebook.com has address 66.220.158.20

# whois 69.171.228.40 | grep CIDR

CIDR: 69.171.224.0/19

Баним:

1

-A OUTPUT -p tcp -d 69.171.224.0/19 -j DROP

Но можно и проще:

1 2

-A OUTPUT -p tcp -d www.facebook.com -j DROP -A OUTPUT -p tcp -d facebook.com -j DROP

Забанить комп по MAC адресу (таблица ARP на шлюзе вам в помощь):

1

-A INPUT -m mac --mac-source 00:0F:EA:91:04:08 -j DROP

Открыть диапазон портов:

1

-A INPUT -m state --state NEW -m tcp -p tcp --dport 7000:7010 -j ACCEPT

Список полезных правил, понятно что ACCEPT, DROP, REJECT по желанию

1 2 3 4 5 6 7 8 9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 27 28 29 30 31 32 33 34 35 36 37 38 39 40 41 42 43 44 45 46 47 48 49 50 51 52

Replace ACCEPT with DROP to block port: ## open port ssh tcp port 22 ## iptables -A INPUT -m state --state NEW -m tcp -p tcp --dport 22 -j ACCEPT iptables -A INPUT -s 192.168.1.0/24 -m state --state NEW -p tcp --dport 22 -j ACCEPT   ## open cups (printing service) udp/tcp port 631 for LAN users ## iptables -A INPUT -s 192.168.1.0/24 -p udp -m udp --dport 631 -j ACCEPT iptables -A INPUT -s 192.168.1.0/24 -p tcp -m tcp --dport 631 -j ACCEPT   ## allow time sync via NTP for lan users (open udp port 123) ## iptables -A INPUT -s 192.168.1.0/24 -m state --state NEW -p udp --dport 123 -j ACCEPT   ## open tcp port 25 (smtp) for all ## iptables -A INPUT -m state --state NEW -p tcp --dport 25 -j ACCEPT   # open dns server ports for all ## iptables -A INPUT -m state --state NEW -p udp --dport 53 -j ACCEPT iptables -A INPUT -m state --state NEW -p tcp --dport 53 -j ACCEPT   ## open http/https (Apache) server port to all ## iptables -A INPUT -m state --state NEW -p tcp --dport 80 -j ACCEPT iptables -A INPUT -m state --state NEW -p tcp --dport 443 -j ACCEPT   ## open tcp port 110 (pop3) for all ## iptables -A INPUT -m state --state NEW -p tcp --dport 110 -j ACCEPT   ## open tcp port 143 (imap) for all ## iptables -A INPUT -m state --state NEW -p tcp --dport 143 -j ACCEPT   ## open access to Samba file server for lan users only ## iptables -A INPUT -s 192.168.1.0/24 -m state --state NEW -p tcp --dport 137 -j ACCEPT iptables -A INPUT -s 192.168.1.0/24 -m state --state NEW -p tcp --dport 138 -j ACCEPT iptables -A INPUT -s 192.168.1.0/24 -m state --state NEW -p tcp --dport 139 -j ACCEPT iptables -A INPUT -s 192.168.1.0/24 -m state --state NEW -p tcp --dport 445 -j ACCEPT   ## open access to proxy server for lan users only ## iptables -A INPUT -s 192.168.1.0/24 -m state --state NEW -p tcp --dport 3128 -j ACCEPT   # Allow FTP connections @ port 21 iptables -A INPUT  -p tcp --sport 21 -m state --state ESTABLISHED -j ACCEPT iptables -A OUTPUT -p tcp --dport 21 -m state --state NEW,ESTABLISHED -j ACCEPT   # Allow Active FTP Connections iptables -A INPUT -p tcp --sport 20 -m state --state ESTABLISHED,RELATED -j ACCEPT iptables -A OUTPUT -p tcp --dport 20 -m state --state ESTABLISHED -j ACCEPT   # Allow Passive FTP Connections iptables -A INPUT -p tcp --sport 1024: --dport 1024:  -m state --state ESTABLISHED -j ACCEPT iptables -A OUTPUT -p tcp --sport 1024: --dport 1024:  -m state --state ESTABLISHED,RELATED -j ACCEPT   ## open access to mysql server for lan users only ## iptables -I INPUT -p tcp --dport 3306 -j ACCEPT

Посмотреть что происходит с портом 22:

1

iptables -L INPUT -v -n | grep 22

И в заключении можно сказать, что я привел выше только самые общие, базисные примеры, на самом деле IPtables умеет делать много вещей.

- Инспекция пакетов

- Фильтрация траффика

- Транслирование адресов (NAT)

и т.д.

За помощь в примерах, спасибо cyberciti.biz