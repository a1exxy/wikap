nterface POS0/2/1/0

 description 

 mtu 1518

 service-policy input TELECOM-IN-FILTER

 service-policy output ACCESS_DSCP0

policy-map TELECOM-IN-FILTER

 class FILTER

  police rate percent 100 

   conform-action drop

  !

 !

 class class-default

  set dscp default

 !

 end-policy-map

class-map match-any FILTER

 match access-group ipv4 T_F 

 end-class-map

ipv4 access-list T_F

 20 permit udp any eq 1900 3.190.200.0 0.0.7.255

 30 permit udp any eq 1900 4.140.224.0 0.0.31.255

 40 permit udp any eq 1900 78.19.240.0 0.0.15.255

 50 permit udp any eq 1900 5.90.100.0 0.0.3.255