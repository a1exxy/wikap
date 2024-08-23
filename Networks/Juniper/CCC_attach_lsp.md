set protocols l2circuit neighbor 10.38.0.6 interface ae144.952 virtual-circuit-id 3543

set protocols l2circuit neighbor 10.38.0.6 interface ae144.952 control-word

set protocols l2circuit neighbor 10.38.0.6 interface ae144.952 community attach-to-lsp-irk06

set protocols l2circuit neighbor 10.38.0.6 interface ae144.952 ignore-encapsulation-mismatch

set protocols l2circuit neighbor 10.38.0.6 interface ae144.952 ignore-mtu-mismatch

set policy-options community attach-to-lsp-irk06 members 5402:3806

set routing-options forwarding-table export l2c_mapping_to_lsp-irk06

set policy-options policy-statement l2c_mapping_to_lsp-irk06 from community attach-to-lsp-irk06

set policy-options policy-statement l2c_mapping_to_lsp-irk06 then install-nexthop lsp nsk02_irk06

set protocols mpls label-switched-path nsk02_irk06 from 10.54.0.2

set protocols mpls label-switched-path nsk02_irk06 to 10.38.0.6

set protocols mpls label-switched-path nsk02_irk06 primary nsk02_irk06 optimize-timer 30

set protocols mpls label-switched-path nsk02_irk06 primary nsk02_irk06 adaptive

set protocols mpls label-switched-path nsk02_irk06 primary nsk02_irk06 select manual

set protocols mpls path nsk02_irk06 10.54.54.86

set protocols mpls path nsk02_irk06 10.38.54.5