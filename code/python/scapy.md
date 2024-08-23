pip3 install scapy

#!/usr/local/bin/python3

from scapy.all import *

os.system("iptables -A OUTPUT -p tcp -o eth0 --sport 1:65535 --tcp-flags RST RST -j DROP")

def packet(pkt):

    if pkt[TCP].flags == 2:

        print('SYN packet detected port : ' + str(pkt[TCP].sport) + ' from IP Src : ' + pkt[IP].src)

        send(IP(dst=pkt[IP].src, src=pkt[IP].dst)/TCP(dport=pkt[TCP].sport, sport=pkt[TCP].dport,ack=pkt[TCP].seq + 1, flags='SA'))

sniff(iface="eth0", prn=packet, filter="tcp[0xd]&18=2",count=100)

os.system("iptables -D OUTPUT -p tcp -o eth0 --sport 1:65535 --tcp-flags RST RST -j DROP")