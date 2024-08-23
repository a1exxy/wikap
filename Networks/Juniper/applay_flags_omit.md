Let’s hide this filter. Use this command:

 

[edit]root@r1# set firewall family inet filter protect-re apply-flags omit [edit]root@r1#

 

And now, you will see this:

 

[edit]root@r1# show firewall                                                  family inet {    filter protect-re { /* OMITTED */ };}[edit]root@r1#

 

However, you can see the configuration by using “display omit” or “display set”:

 

[edit]root@r1# show firewall | display omit   family inet {    filter protect-re {        apply-flags omit;        term 1 {            from {                prefix-list {                    bgp-peers;                }            }            then accept;        }        term 2 {            then accept;        }        term OTHER {            then {                reject;            }        }    }}[edit]root@r1# show firewall | display set     set firewall family inet filter protect-re apply-flags omitset firewall family inet filter protect-re term 1 from prefix-list bgp-peersset firewall family inet filter protect-re term 1 then acceptset firewall family inet filter protect-re term 2 then acceptset firewall family inet filter protect-re term OTHER then reject[edit]root@r1#