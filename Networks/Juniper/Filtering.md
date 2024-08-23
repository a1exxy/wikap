set policy-options policy-statement REJECT then reject

set routing-instances relay instance-type vrf

set routing-instances relay route-distinguisher 13604:400

set routing-instances relay vrf-export REJECT

set routing-instances relay vrf-target target:485:2001

set routing-instances relay vrf-table-label

set routing-instances relay routing-options rib relay.inet6.0 static route ::/0 next-table internet.inet6.0

set routing-instances relay routing-options static route 0.0.0.0/0 next-table internet.inet.0

set interfaces ae3 unit 503 family inet filter input FBF_RK

set interfaces ae3 unit 503 family inet6 filter input FBF_RK6

set firewall family inet filter FBF_RK term 10 then routing-instance relay

set firewall family inet6 filter FBF_RK6 term 10 then routing-instance relay

