# Запись трафика

nohup tcpdump -i eno4 -K -n -nn -G 60 -w 'dump___%Y_%m_%d__%H_%M_%S%z.pcap' &