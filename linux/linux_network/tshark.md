tcpdump -i eno2 -K -n -nn vlan 1998 and vlan 161 and icmp and src 1.2.3.4

tshark -Y 'http' -T fields -e frame.number  -e ip.src -e tcp.srcport -e ip.dst -e tcp.dstport -e http.request.full_uri -r dump.pcap 

tshark -Y 'http.request.full_uri contains "site.net"' -r dump.pcap

tshark   -r dump.pcap -V frame.number == 1