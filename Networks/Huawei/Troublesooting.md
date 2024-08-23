Протокол IPv4

1) Просмотр текущей конфигурации протокола BGP.

[~mskl15]dis current-configuration configuration bgp 

2) Просмотр содержания таблицы BGP для address-family VPNv4 VRF Internet 

[~mskl15]dis bgp vpnv4 vpn-instance internet routing-table 

3) Просмотр информация по BGP соседям в рамках VRF Internet 

[~mskl15]dis bgp vpnv4 vpn-instance internet peer 

4) Просмотр анонсируемых ipv4 маршрутов с сторону заданного BGP соседа 

[~mskl15]dis bgp vpnv4 vpn-instance internet routing-table peer 21.15.47.85 advertised-routes 

5) Просмотр полученных ipv4 маршрутов от заданного BGP соседа 

[~mskl15]dis bgp vpnv4 vpn-instance internet routing-table peer 21.15.47.85 received-routes 

 

6) Просмотр подробной BGP информации по выбранному ipv4 префиксу 

[~mskl15]dis bgp vpnv4 vpn-instance internet routing-table 15.4.1.1 

 

7) Просмотр содержания таблицы BGP для VRF Internet полученной в результате применения фильтра, построенного на основе регулярного выражения. 

[~mskl15]dis bgp vpnv4 vpn-instance internet routing-table regular-expression 65004

 

8) Обновление политики приема BGP анонсов со стороны заданного BGP соседа на основе локально хранимых BGP IPv4 маршрутов от данного BGP соседа. Локальной хранение маршрутов обеспечивается применением команды keep-all-routes на уровне настройки peer группы.   

<mskl15>refresh bgp vpn-instance internet ipv4-family 21.15.47.81 import

9) Просмотр содержания таблицы маршрутизации VRF internet для IPv4 address-family.   

[~mskl15]dis ip routing-table vpn-instance internet

10) Просмотр содержания FIB таблицы VRF internet для IPv4 address-family.   

[~mskl15]dis fib slot 1 vpn-instance internet 

11) Проверка доступности заданного ipv4 адреса в рамках VRF Internet

[~mskl15]ping -vpn-instance internet 21.15.47.85                      

Протокол IPv6

1) Просмотр содержания таблицы BGP для address-family VPNv6 VRF Internet 

[~mskl15]display bgp vpnv6 vpn-instance internet routing-table 

2) Просмотр информации по BGP соседям в рамках VRF Internet 

[~mskl15]display bgp vpnv6 vpn-instance internet peer 

3) Просмотр анонсируемых ipv6 маршрутов с сторону заданного BGP соседа 

[~mskl15]display bgp vpnv6 vpn-instance internet routing-table peer 2A00:1E:1:1::A advertised-routes 

 

4) Просмотр полученных ipv6 маршрутов от заданного BGP соседа 

[~mskl15]display bgp vpnv6 vpn-instance internet routing-table peer 2A00:1E:1:1::A received-routes 

 

5) Просмотр подробной BGP информации по выбранному ipv6 префиксу 

[~mskl15]display bgp vpnv6 vpn-instance internet routing-table 2A00:1B:77:5:5:5:5:5                

 

6) Просмотр содержания таблицы BGP для VRF Internet полученной в результате применения фильтра, построенного на основе регулярного выражения. 

[~mskl15]display bgp vpnv6 vpn-instance internet routing-table regular-expression 65005

 

7) Проверка доступности заданного ipv6 адреса в рамках VRF Internet

[~mskl15]ping ipv6 vpn-instance internet 2A00:1E:1:1::2

8) Обновление политики приема BGP анонсов со стороны заданного BGP соседа на основе локально хранимых BGP IPv6 маршрутов от данного BGP соседа. Локальной хранение маршрутов обеспечивается применением команды keep-all-routes на уровне настройки peer группы.   

<mskl15>refresh bgp vpn-instance internet ipv6-family 2A00:1E:1:1::2 import

9) Просмотр содержания таблицы маршрутизации VRF internet для IPv6 address-family.

[~mskl15]dis ipv6 routing-table vpn-instance internet 

10) Просмотр содержания FIB таблицы VRF internet для IPv6 address-family.

[~mskl15]dis ipv6 fib slot 1 vpn-instance internet 

Протокол BFD

1) Просмотр всех существующих BFD сессий.

[~mskl15]dis bfd session all

2) Просмотр детальной информации по BFD сессии с заданным IPv4 BFD соседом.

[~mskl15]dis bfd session peer-ip 21.15.47.81 verbose 

3) Просмотр детальной информации по BFD сессии с заданным IPv6 BFD соседом.

[~mskl15]dis bfd session peer-ipv6 2A00:1E:1:1::A verbose 

4) Просмотр существующих BFD сессий для протокола BGP.

[~mskl15]dis bgp bfd session all

5) Просмотр текущей статистики протокола BFD.

[~mskl15]dis bfd statistics 