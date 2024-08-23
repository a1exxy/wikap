show route forwarding-table family vpls table vpls_name1

show route table vpls_name1.l2vpn.0 extensive 

show vpls mac-table instance vpls_name1

1) Проверка статуса сети VPLS, статистика и текущие соединения. 

sh l2vpn bridge-domain group vpls__sz detail 

2) Просмотр таблицы mac-адресов.

sh l2vpn forwarding bridge-domain vpls__sz:vpls__sz_2 mac-address detail location 0/0/CPU0 

3) Просмотр BGP таблицы для vpls__sz

sh bgp l2vpn vpls bridge-domain vpls__sz:vpls__sz_2 

4) Просмотр BGP NLRI для заданного префикса.

sh bgp l2vpn vpls bridge-domain vpls__sz:vpls__sz_2 1:1/32 detail 

5) Проверка префиксов от заданного РЕ.

sh bgp l2vpn vpls neighbors 10.99.0.12

1) Просмотр VPLS соединений. Показывает статус VPLS, в легенде приведены возможные статусы и их описания.

router> show vpls connections instance vpls__dv   

2) Просмотр таблицы mac-адресов (для очистки clear vpls mac-table).

router> show vpls mac-table instance vpls__dv 

3) Просмотр статистики по VPLS.

router> show vpls statistics instance vpls__dv 

4) Просмотр BGP-маршрутов таблицы vpls__dv.l2vpn.0 

router> show route table vpls__dv.l2vpn.0 extensive 

5) Просмотр таблицы пересылки VPLS (показывает и  mac-адреса в instance).

router> show route forwarding-table family vpls table vpls__dv 

VPLS LDP version

interface TenGigE0/10/0/2.1018 l2transport

 description -M- 150526191000 MAAS_VPLS ---

 encapsulation dot1q 1018

l2vpn

 bridge group MAAS

  bridge-domain MAAS

   interface TenGigE0/10/0/2.1018

   !

   vfi MAAS

    neighbor 10.22.0.6 pw-id 105422

    !     

    neighbor 10.66.0.6 pw-id 106654