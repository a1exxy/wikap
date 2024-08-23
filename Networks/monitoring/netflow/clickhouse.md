SELECT 

    count(), 

    sum(bytes) AS TrafBytes, 

    in_iface, 

    out_iface, 

    IPv4NumToString(src_net) AS srcnet, 

    IPv4NumToString(dst_net) AS dstnet, 

    dictGetString('ifIndex', 'Description', (IPv4StringToNum('10.99.0.15'), in_iface)) AS ifDescr

FROM sdNetAS_nexthop_iface_dir 

WHERE (d = today()) AND (device = IPv4StringToNum('10.99.0.15')) AND ((dst_net >= (IPv4StringToNum('81.100.209.0') AS net2)) AND (dst_net <= ((net2 + pow(2, 32 - 24)) - 1)))

GROUP BY 

    in_iface, 

    out_iface, 

    src_net, 

    dst_net

select count(dt) as s,dt from bgp_msglog where d = today() and dt >= toDateTime('2019-01-14 11:40:00')  and dt <= toDateTime('2019-01-14 12:00:00') group by dt order by s;

SELECT 

    dt, 

    IPv4NumToString(src_ip) AS src, 

    IPv4NumToString(dst_ip) AS dst, 

    tos

FROM detailed 

WHERE (d = (today() - 1)) AND (device = IPv4StringToNum('10.78.0.1')) AND (src_ip = IPv4StringToNum('174.129.28.92')) AND (dt >= toDateTime('2019-04-04 00:00:00')) AND (dt <= toDateTime('2019-04-04 12:00:00'))

LIMIT 1