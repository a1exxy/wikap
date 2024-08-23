wget http://www.pmacct.net/pmacct-1.5.3.tar.gz

yum groupinstall "Development Tools"

yum install libpcap libpcap-devel

./configure 

make

make install

[root@nfa01 config]# cat as.conf

! включить отладочный режим

!!!debug: true

!

! уходить в фон?

daemonize: true

!!!daemonize: false

!

! куда писать лог файл

logfile: /opt/pmacct/logs/net_as.conf.log

!

maps_refresh: true

!

!

! базовая настройка для nfacctd

!

! какой IP и порт слушать

nfacctd_ip: 10.77.127.29

nfacctd_port: 50009

!

! чтобы убрать проверку/logging out-or-order пакетов (Sequence checks)

!!!nfacctd_disable_checks: true

!

! метод агрегации IP префиксов

nfacctd_net: netflow

!

!populate 'peer_dst_ip' field from NetFlow IP next hop field if BGP next-hop is not available

use_ip_next_hop: true

!

! makes 'nfacctd' to ignore timestamps included in NetFlow header and build new ones

nfacctd_time_new: true

!

!если true добавляет 2 новых поля timestamp_min и timestamp_max:

!   timestamp_min - timestamp первого элемента, попадающего в определённый агрегат,

!   timestamp_max - timestamp последнего элемента

!nfacctd_stitching: true

! nfacctd_pro_rating не совместимо с nfacctd_stitching

!!!nfacctd_pro_rating: true

!

!брать ASNs из BGP RIB пира, ассоциированного с NetFlow exporter 

nfacctd_as_new: bgp

!

! автоматически ренормализует счётчики пакетов/байт с учётом семплинга , приходящие в потоках netflow

nfacctd_renormalize: true

! коэффициенты семплирования - переопределяют сообщаемые роутерами

sampling_map: /opt/pmacct/config/sampling.map

!

! файл соответствий между route-distinguisher и экспортёром netflow

flow_to_rd_map: /opt/pmacct/config/flow_to_rd.map

!

!!!plugins: memory[a1], print[p1], print[p2], amqp, amqp[a1], amqp[a2]

!!plugins: mysql[5m], mysql[1h], print[p5m]

plugins: print[p5m]

!

! настройки print плагина(ов) (в основном нужны при отладке, если не хотим писать в SQL базу)

!

! [p1]

plugin_pipe_size[p5m]: 10024000

plugin_buffer_size[p5m]: 10240

print_output[p5m]: csv

print_output_file[p5m]: /opt/pmacct/out/%Y-%m-%d/$peer_src_ip/p5m.%H%M.csv

print_output_file_append[p5m]: true

print_refresh_time[p5m]: 300

print_history[p5m]: 5m

print_history_roundoff[p5m]: m

!print_cache_entries[p5m]: 64007

print_cache_entries[p5m]: 1000000

!aggregate[p5m]: peer_src_ip, peer_dst_ip, in_iface, out_iface, src_net, src_mask, dst_net, dst_mask, src_as, peer_src_as, peer_dst_as, dst_as, mpls_vpn_rd

!aggregate[p5m]: peer_src_ip, peer_dst_ip, in_iface, out_iface, src_as, peer_src_as, peer_dst_as, dst_as, mpls_vpn_rd

!

!aggregate[p5m]:  in_iface, out_iface, src_as, peer_src_as, peer_dst_as, dst_as

!aggregate[p5m]: peer_src_ip, peer_dst_ip, in_iface, out_iface, src_net, src_mask, dst_net, dst_mask, src_as, peer_src_as, peer_dst_as, dst_as

aggregate[p5m]: peer_src_ip, peer_dst_ip, in_iface, out_iface, src_net, src_mask, dst_net, dst_mask, src_as, peer_src_as, peer_dst_as, dst_as,src_port, dst_port, tos, proto

!

!print_trigger_exec[p5m]: /root/pmacct/bin/print_trigger.sh

!

! настройки для BGP daemon

!

! включать BGP daemon/пиринг?

!!!bgp_daemon: false

bgp_daemon: true

!

! на каком IP адресе слушать BGP connect-ы от пиров (напр., адрес eth0 интерфейса)

bgp_daemon_ip: 10.77.127.29

! обычно сам выставляется = bgp_daemon_ip, но чтоб наверняка...

bgp_daemon_id: 10.77.127.29

!

! максимальное число разрешенных пиринговых сессий

bgp_daemon_max_peers: 20

!

!full pathname to a file to map source IP address of NetFlow agents to source IP address or Router ID of BGP peers

bgp_agent_map: /opt/pmacct/config/bgp_agent.map

!

!file to write a list of the BGP neighbors in the established state

bgp_neighbors_file: /opt/pmacct/out/bgp_neighbors.out

! в какой файл писать BGP protocol messages

!bgp_daemon_msglog_file: /root/pmacct/out/bgp_msglog.$peer_src_ip.out

!

bgp_daemon_pipe_size: 16777216

! если хотим получать дампы BGP RIB

! в какой файл(ы) писать дампы BGP таблиц

!bgp_table_dump_file: /opt/pmacct/out/%Y-%m-%d/$peer_src_ip/bgp_table.%H%M.dump

! как часто делать дамп

!bgp_table_dump_refresh_time: 3600

!

!bgp_table_dump_output:json // надо проверять

!

!

! метод сопоставления входящего трафика с source peer ASN. bgp - делает нативный lookup в BGP RIB (предполагая, что трафик симметричный)

bgp_peer_src_as_type: bgp

!

bgp_src_as_path_type: bgp

bgp_src_local_pref_type: bgp

bgp_src_med_type: bgp

!

bgp_follow_default: 1

!