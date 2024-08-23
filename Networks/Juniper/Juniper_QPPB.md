Using destination-class to achieve the QoS Policy Propagation via BGP (QPPB) on M-series routers

Avg. Rating:  2

 [KB9298] Show Article Properties https://kb.juniper.net/InfoCenter/index?page=content&id=KB9298&act=login#

SUMMARY:

In QoS design, BGP community might be used to represent service class; this is called QoS Policy Propagation via BGP (QPPB) by other vendors.   For JUNOS on M-series, the destination-class (DCU) does the similar function of QPPB.

SOLUTION:

JUNOS has two different features to achieve the QPPB on M-series.  

classification-override which can only change traffic forwarding class based on BGP community

destination-class. (DCU).  The DCU is using normal JUNOS firewall to do action on the matched traffic.  Besides the forwarding class changing, DCU can change the loss-priority (PLP) and do policing.

Configuration example:

The remote router is sending a prefix with community 100:1000 which indicates low priority traffic's destination.  The below configuration will forward the traffic designated to this prefix into queue 1 and mark the loss-priority to be high.

On the local router, define a policy to match the prefix with community 100:1000 and tag them to be "dcu-1". Then apply the policy to forwarding table. 

routing-options {

    forwarding-table {

        export set-destination-class;

    }

}

policy-options {

    policy-statement set-destination-class {

        term 1 {

            from community low-priority-traffic;

            then destination-class dcu-1;

        }

        term 2 {

            then accept;

        }

    }

    community low-priority-traffic members 100:1000;

}

Define CoS configuration.

class-of-service {

    forwarding-classes {

        queue 0 best-effort;

        queue 1 low-priority;

        queue 3 network-control;

    }

    interfaces {

        so-0/1/0 {

            scheduler-map juniper;

        }

    }

    scheduler-maps {

        juniper {

            forwarding-class best-effort scheduler 95-95-high;

            forwarding-class low-priority scheduler 0-0-low;

            forwarding-class network-control scheduler 5-5-stright-high;

        }

    }

    schedulers {

        5-5-stright-high {

            buffer-size percent 5;

            priority strict-high;

        }

        0-0-low {

            buffer-size percent 0;

            priority low;

        }

        95-95-high {

            transmit-rate percent 95;

            buffer-size percent 95;

            priority high;

        }

    }

}

Define the firewall filter to match traffic tagged with destination class dcu-1 and an action with forwarding-class and loss-priority changing. Then apply the filter to the interface's outbound direction.

interfaces {

    so-0/1/0 {

        unit 0 {

            family inet {

                filter {

                    output differentiate-forwarding-class;

                }

                address 1.1.1.1/30;

            }

        }

    }

}

firewall {

    filter differentiate-forwarding-class {

        term low-priority-traffic {

            from {

                destination-class dcu-1;

            }

            then {

                loss-priority high;

                forwarding-class low-priority;

            }

        }

        term others {

            then accept;

        }

    }

}