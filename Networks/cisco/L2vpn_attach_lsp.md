pw-class ETHER_MODE_balan_te1

  encapsulation mpls

   transport-mode ethernet

   load-balancing

    flow-label both

   !

   preferred-path interface tunnel-te 1

interface tunnel-te1

 description -E- 161026152222 Tunnel cta06rb ---

 ipv4 unnumbered Loopback0

 load-interval 30

 logging events all

 logging events lsp-status state

 destination 10.75.0.6

 path-option 1 explicit name irk06-cta06

 path-option 2 dynamic

explicit-path name irk06-cta06

 index 1 next-address strict ipv4 unicast 10.38.75.2