EXABGP.CONF(5)                                               BSD File Formats Manual                                               EXABGP.CONF(5)

NAME

     exabgp.conf — Configuration file controlling the BGP configuration for exabgp(1).

DESCRIPTION

   CONFIGURATION FILE SYNTAX

        group <groupname> {

          // Most if not all the attributes under neighbor can be defined

          // at the group level as well, and the settings will be inherited

          // unless overridden in the neighbor section

          neighbor <ip-address> {

            description <text>;

            router-id <router-id>;

            local-address <ip-address>;

            local-as <asn>;

            peer-as <asn>;

            passive;

            hold-time <seconds>;

            md5 <md5-secret>;

            ttl-security;

            group-updates;

            aigp <truthvalue>;

            route-refresh <truthvalue>;

            graceful-restart <...>;

            multi-session <truthvalue);

            add-path <path>;

            auto-flush <truthvalue>;

            adj-rib-out <truthvalue>;

            // Can also have the groups listed under group <gn> { } below:

            static {

            }

            flow {

            }

            l2vpn {

            }

            process {

            }

            family {

            }

            capability {

            }

            operational {

            }

          }

          static {

            route <ip-address>/<prefixlength> {

              next-hop <ip-address>; // only mandatory attribute

              origin ( IGP | EGP | INCOMPLETE );

              as-path [ <as-sequence-asn> | ( <as-set ) ];

              as-sequence

              med <med>;

              aigp <aigp>;

              local-preference <preference>;

              atomic-aggregate;

              aggregator <asn>:<ip-address>;

              path-information <ip-address>;

              community ( <community> | [ <community> <community> ... ] );

              originator-id <ip-address>;

              cluster-list ( <ip-address> | [ <ip-address> <ip-address> ... ] );

              extended-community ( <extended-community> |

                                   [ <extended-community>

                                     <extended-community> ... ] );

              split /<prefixlength>;

              label ( <label> | [ <label> <label> ... ] );

              ( rd | route-distinguisher ) <route-distinguisher>;

              watchdog <watchdog-name>;

              withdraw;

            }

            // or alternatively

            route <ip-address>/<prefixlength> <attribute-sequence>;

            // where <attribute-sequence> is a sequence of

            // any of the attributes above

          }

          flow {

            route <route-name> {

              (rd | route-distinguisher ) <route-distinguisher>;

              next-hop <ip-address>; // for redirect-to-nexthop

              match {

                // one or more match terms

                source <ip-address>/<prefixlength>;

                destination <ip-address>/<prefixlength>;

                port <portnumber>;

                source-port <portnumber>;

                destination-port <portnumber-expression>;

                protocol [ udp | tcp ]; // IPv4 only

                next-header [ udp | tcp ]; // IPv6 only

                tcp-flags [ fin | syn | rst | push | ack | urgent ];

                icmp-type [ echo-reply | echo-request | info-reply |

                            info-request | mask-reply | mask-request |

                            parameter-problem | redirect | router-advertisment |

                            router-solicit | source-quench | time-exceeded |

                            timestamp | timestamp-reply | unreachable ];

                icmp-code [ communication-prohibited-by-filtering |

                            destination-host-prohibited |

                            destination-host-unknown |

                            destination-network-unknown |

                            fragmentation-needed | host-precedence-violation |

                            ip-header-bad | network-unreachable |

                            network-unreachable-for-tos | port-unreachable |

                            redirect-for-host | redirect-for-network |

                            redirect-for-tos-and-host |

                            redirect-for-tos-and-net |

                            required-option-missing | source-host-isolated |

                            source-route-failed |

                            ttl-eq-zero-during-reassembly |

                            ttl-eq-zero-during-transit ];

                fragment [ not-a-fragment | dont-fragment | is-fragment |

                           first-fragment | last-fragment ];

                // fragment is IPv4 only, poorly tested

                dscp <dscp-value>;

                traffic-class <traffic-class>;

                packet-length <packet-length-expression>;

                flow-label <flow-label-expression>; // IPv6 only

              }

              then {

                // one action only

                accept;

                discard;

                rate-limit <ratelimit>;

                redirect ( <route-distinguisher> | <ip-address> );

                redirect-to-nexthop; // Ref. next-hop above

                copy <ip-address>;

                mark <mark>;

                action ( sample | terminal | sample-terminal );

                community

                extended-community

              }

            }

          }

          l2vpn {

            vpls <site-name> {

              next-hop <ip-address>;

              origin ( IGP | EGP | INCOMPLETE );

              as-path [ <as-sequence-asn> | ( <as-set ) ];

              med <med>;

              local-preference <preference>;

              community ( <community> | [ <community> <community> ... ] );

              originator-id <ip-address>;

              cluster-list [ <ip-address> <ip-address> ... ];

              extended-community ( <extended-community> |

                                   [ <extended-community>

                                     <extended-community> ... ] );

              ( rd | route-distinguisher ) <route-distinguisher>;

              withdraw;

              endpoint ( <vpls-endpoint> | <integer> );

              offset ( <block-offset> | <integer> );

              size ( <block-size> | <integer> );

              base ( <label-base> | <integer> );

              name <route-name>;

          }

          process {

            run <command> <args>;

          }

          family {

            all; // default, or a list of the below

            minimal; // use AFI/SAFI required to announce routes in config

            ipv4 unicast;

            ipv4 multicast;

            ipv4 nlri-mpls;

            ipv4 mpls-vpn;

            ipv4 flow;

            ipv4 flow-vpn;

            ipv6 unicast;

            ipv6 flow;

            ipv6 flow-vpn;

          }

          capability {

            graceful-restart <seconds>;

            asn4 ( enable | disable );

            add-path ( disable | send | receive | send/receive );

            multi-session ( enable | disable );

            operational ( enable | disable );

          }

          operational {

            // ??

          }

        }

        neighbor <ip-address> {

          // Attributes and sections as for under

          // group <groupname> { neighbor <neighbor> {

          // ref. above

        }

     Please note that multi-line sections really do need to be written as multiple lines: the first one ending in "{", and ending with a line

     with a "}" by itself.

SEE ALSO

     exabgp(1).

                                                                February 26, 2015