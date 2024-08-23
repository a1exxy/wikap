 ipv4 access-group ABF_RK ingress

 ipv6 access-group ABF_RK6 ingress

ipv4 access-list ABF_RK

 10 permit ipv4 any any nexthop1 vrf relay

ipv6 access-list ABF_RK6

 10 permit ipv6 any any nexthop1 vrf relay

vrf relay

 fallback-vrf internet

 address-family ipv4 unicast

  import route-target

   485:2001

  !

 !

 address-family ipv6 unicast

  import route-target

   0485:2001

router bgp 485

 vrf relay

  rd 485:12

  label mode per-ce

  address-family ipv4 unicast

   bgp dampening 5 750 4000 20

   bgp attribute-download

   maximum-paths ebgp 4

  !

  address-family ipv6 unicast

   bgp dampening 5 750 4000 20

   bgp attribute-download

   maximum-paths ebgp 4