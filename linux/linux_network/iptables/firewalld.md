firewall-cmd  --zone=public --list-all

firewall-cmd   --list-all-zones

firewall-cmd --list-rich-rules

firewall-cmd --zone=public --add-service=http --permanent

firewall-cmd --zone=public --remove-service=http --permanent

firewall-cmd --permanent --zone=public --add-rich-rule='rule family=ipv4 source address=1.1.1.0/24 destination address=10.10.10.10/32 port port=22 protocol=tcp accept'