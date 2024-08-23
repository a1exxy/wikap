http://support.huawei.com/enterprise/en/doc/EDOC1000036943?section=j008
5.4  Configuring Destination-Based QPPB
Destination-based QPPB differentiates the routes to different destinations and associates differentiated QoS policies with them.

Usage Scenario
QPPB is applicable to both IBGP and EBGP and can be configured for one or more ASs.

As shown in Figure 5-5, traffic is transmitted from Router B (AS 200) and Router C (AS 300) to Router D (AS 400) through Router A (AS 100). Routers B and C function as BGP route senders and Router A functions as a BGP route receiver. Based on the traffic control policies that are signed between providers A and D, Router A needs to limit the rate of the traffic sent to Router D.

Routers B and C advertise BGP routes carrying the community attribute to Router A. After receiving the BGP routes, Router A matches the routes with the community list, ACL list, or AS_Path list, and associates QoS policy IDs with QoS behaviors for the routes. Destination-based QPPB is enabled on the Router A interface that allows traffic to pass through. Therefore, QPPB local policies are applied to all traffic that passes through Router A.

Destination-based QPPB is applicable to both incoming and outgoing traffic on a device.

Figure 5-5  Networking diagram for destination-based QPPB configuration 