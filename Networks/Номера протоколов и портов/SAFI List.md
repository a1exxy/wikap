# Subsequent Address Family Identifiers (SAFI) Parameters

Первоисточник
https://www.iana.org/assignments/safi-namespace/safi-namespace.xhtml#safi-namespace-2

<table class="sortable" id="table-safi-namespace-2-range">
        <thead>
          <tr style="cursor: pointer;">
            <th>Range <img style="vertical-align:middle" src="../_support/sort_none.gif"></th>
            <th>Registration Procedures <img style="vertical-align:middle" src="../_support/sort_none.gif"></th>
            <th>Note <img style="vertical-align:middle" src="../_support/sort_none.gif"></th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>1-63</td>
            <td>Standards Action</td>
            <td></td>
          </tr>
          <tr>
            <td>64-127</td>
            <td>First Come First Served</td>
            <td></td>
          </tr>
          <tr>
            <td>128-240</td>
            <td>Some recognized assignments below, others Reserved</td>
            <td></td>
          </tr>
          <tr>
            <td>241-254</td>
            <td>Reserved for Private Use</td>
            <td>Not to be assigned</td>
          </tr>
        </tbody>
      </table>


<table id="table-safi-namespace-2" class="sortable">
        <thead>
          <tr style="cursor: pointer;">
            <th>Value <img style="vertical-align:middle" src="../_support/sort_none.gif"></th>
            <th>Description <img style="vertical-align:middle" src="../_support/sort_none.gif"></th>
            <th>Reference <img style="vertical-align:middle" src="../_support/sort_none.gif"></th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td align="center">0</td>
            <td>Reserved</td>
            <td>[<a href="https://www.iana.org/go/rfc4760">RFC4760</a>]</td>
          </tr>
          <tr>
            <td align="center">1</td>
            <td>Network Layer Reachability Information used     
for unicast forwarding</td>
            <td>[<a href="https://www.iana.org/go/rfc4760">RFC4760</a>]</td>
          </tr>
          <tr>
            <td align="center">2</td>
            <td>Network Layer Reachability Information used     
for multicast forwarding</td>
            <td>[<a href="https://www.iana.org/go/rfc4760">RFC4760</a>]</td>
          </tr>
          <tr>
            <td align="center">3</td>
            <td>Reserved</td>
            <td>[<a href="https://www.iana.org/go/rfc4760">RFC4760</a>]</td>
          </tr>
          <tr>
            <td align="center">4</td>
            <td>Network Layer Reachability Information (NLRI)   
with MPLS Labels</td>
            <td>[<a href="https://www.iana.org/go/rfc8277">RFC8277</a>]</td>
          </tr>
          <tr>
            <td align="center">5</td>
            <td>MCAST-VPN</td>
            <td>[<a href="https://www.iana.org/go/rfc6514">RFC6514</a>]</td>
          </tr>
          <tr>
            <td align="center">6</td>
            <td>Network Layer Reachability Information used     
for Dynamic Placement of Multi-Segment Pseudowires</td>
            <td>[<a href="https://www.iana.org/go/rfc7267">RFC7267</a>]</td>
          </tr>
          <tr>
            <td align="center">7</td>
            <td>Encapsulation SAFI (OBSOLETE)</td>
            <td>[<a href="https://www.iana.org/go/rfc9012">RFC9012</a>]</td>
          </tr>
          <tr>
            <td align="center">8</td>
            <td>MCAST-VPLS</td>
            <td>[<a href="https://www.iana.org/go/rfc7117">RFC7117</a>]</td>
          </tr>
          <tr>
            <td align="center">9</td>
            <td>BGP SFC</td>
            <td>[<a href="https://www.iana.org/go/rfc9015">RFC9015</a>]</td>
          </tr>
          <tr>
            <td align="center">10-63</td>
            <td>Unassigned</td>
            <td></td>
          </tr>
          <tr>
            <td align="center">64</td>
            <td>Tunnel SAFI</td>
            <td>[<a href="#Gargi_Nalawade">Gargi_Nalawade</a>][<a href="https://www.iana.org/go/draft-nalawade-kapoor-tunnel-safi-01">draft-nalawade-kapoor-tunnel-safi-01</a>]</td>
          </tr>
          <tr>
            <td align="center">65</td>
            <td>Virtual Private LAN Service (VPLS)</td>
            <td>[<a href="https://www.iana.org/go/rfc4761">RFC4761</a>][<a href="https://www.iana.org/go/rfc6074">RFC6074</a>]</td>
          </tr>
          <tr>
            <td align="center">66</td>
            <td>BGP MDT SAFI</td>
            <td>[<a href="https://www.iana.org/go/rfc6037">RFC6037</a>]</td>
          </tr>
          <tr>
            <td align="center">67</td>
            <td>BGP 4over6 SAFI</td>
            <td>[<a href="https://www.iana.org/go/rfc5747">RFC5747</a>]</td>
          </tr>
          <tr>
            <td align="center">68</td>
            <td>BGP 6over4 SAFI</td>
            <td>[<a href="#Yong_Cui">Yong_Cui</a>]</td>
          </tr>
          <tr>
            <td align="center">69</td>
            <td>Layer-1 VPN auto-discovery information</td>
            <td>[<a href="https://www.iana.org/go/rfc5195">RFC5195</a>]</td>
          </tr>
          <tr>
            <td align="center">70</td>
            <td>BGP EVPNs</td>
            <td>[<a href="https://www.iana.org/go/rfc7432">RFC7432</a>]</td>
          </tr>
          <tr>
            <td align="center">71</td>
            <td>BGP-LS</td>
            <td>[<a href="https://www.iana.org/go/rfc9552">RFC9552</a>]</td>
          </tr>
          <tr>
            <td align="center">72</td>
            <td>BGP-LS-VPN</td>
            <td>[<a href="https://www.iana.org/go/rfc9552">RFC9552</a>]</td>
          </tr>
          <tr>
            <td align="center">73</td>
            <td>SR TE Policy SAFI</td>
            <td>[<a href="https://www.iana.org/go/draft-ietf-idr-segment-routing-te-policy-20">draft-ietf-idr-segment-routing-te-policy-20</a>]</td>
          </tr>
          <tr>
            <td align="center">74</td>
            <td>SD-WAN Capabilities</td>
            <td>[<a href="https://www.iana.org/go/draft-ietf-idr-sdwan-edge-discovery-03">draft-ietf-idr-sdwan-edge-discovery-03</a>]</td>
          </tr>
          <tr>
            <td align="center">75</td>
            <td>Routing Policy SAFI</td>
            <td>[<a href="https://www.iana.org/go/draft-ietf-idr-rpd-02">draft-ietf-idr-rpd-02</a>]</td>
          </tr>
          <tr>
            <td align="center">76</td>
            <td>Classful Transport SAFI</td>
            <td>[<a href="https://www.iana.org/go/draft-ietf-idr-bgp-ct-30">draft-ietf-idr-bgp-ct-30</a>]</td>
          </tr>
          <tr>
            <td align="center">77</td>
            <td>Tunneled Traffic Flowspec</td>
            <td>[<a href="https://www.iana.org/go/draft-ietf-idr-flowspec-nvo3-10">draft-ietf-idr-flowspec-nvo3-10</a>]</td>
          </tr>
          <tr>
            <td align="center">78</td>
            <td>MCAST-TREE</td>
            <td>[<a href="https://www.iana.org/go/draft-ietf-bess-bgp-multicast-03">draft-ietf-bess-bgp-multicast-03</a>]</td>
          </tr>
          <tr>
            <td align="center">79</td>
            <td>BGP-DPS (Dynamic Path Selection)</td>
            <td>[<a href="https://eos.arista.com/eos-4-26-2f/dps-vpn-scaling-using-bgp">https://eos.arista.com/eos-4-26-2f/dps-vpn-scaling-using-bgp</a>][<a href="#Venkit_Kasiviswanathan">Venkit_Kasiviswanathan</a>]</td>
          </tr>
          <tr>
            <td align="center">80</td>
            <td>BGP-LS-SPF</td>
            <td>[<a href="https://www.iana.org/go/draft-ietf-lsvr-bgp-spf-15">draft-ietf-lsvr-bgp-spf-15</a>][<a href="#Victor_Kuarsingh">Victor_Kuarsingh</a>]</td>
          </tr>
          <tr>
            <td align="center">81-82</td>
            <td>Unassigned</td>
            <td></td>
          </tr>
          <tr>
            <td align="center">83</td>
            <td>BGP CAR</td>
            <td>[<a href="https://www.iana.org/go/draft-ietf-idr-bgp-car-05">draft-ietf-idr-bgp-car-05</a>]</td>
          </tr>
          <tr>
            <td align="center">84</td>
            <td>BGP VPN CAR</td>
            <td>[<a href="https://www.iana.org/go/draft-ietf-idr-bgp-car-05">draft-ietf-idr-bgp-car-05</a>]</td>
          </tr>
          <tr>
            <td align="center">85</td>
            <td>BGP-MUP SAFI</td>
            <td>[<a href="https://www.iana.org/go/draft-mpmz-bess-mup-safi-00">draft-mpmz-bess-mup-safi-00</a>]</td>
          </tr>
          <tr>
            <td align="center">86-127</td>
            <td>Unassigned</td>
            <td></td>
          </tr>
          <tr>
            <td align="center">128</td>
            <td>MPLS-labeled VPN address</td>
            <td>[<a href="https://www.iana.org/go/rfc4364">RFC4364</a>][<a href="https://www.iana.org/go/rfc8277">RFC8277</a>][<a href="https://www.iana.org/go/rfc9252">RFC9252</a>]</td>
          </tr>
          <tr>
            <td align="center">129</td>
            <td>Multicast for BGP/MPLS IP Virtual Private       
Networks (VPNs)</td>
            <td>[<a href="https://www.iana.org/go/rfc6513">RFC6513</a>][<a href="https://www.iana.org/go/rfc6514">RFC6514</a>]</td>
          </tr>
          <tr>
            <td align="center">130-131</td>
            <td>Reserved</td>
            <td>[<a href="https://www.iana.org/go/rfc4760">RFC4760</a>]</td>
          </tr>
          <tr>
            <td align="center">132</td>
            <td>Route Target constrains</td>
            <td>[<a href="https://www.iana.org/go/rfc4684">RFC4684</a>]</td>
          </tr>
          <tr>
            <td align="center">133</td>
            <td>Dissemination of Flow Specification rules</td>
            <td>[<a href="https://www.iana.org/go/rfc8955">RFC8955</a>]</td>
          </tr>
          <tr>
            <td align="center">134</td>
            <td>L3VPN Dissemination of Flow Specification rules</td>
            <td>[<a href="https://www.iana.org/go/rfc8955">RFC8955</a>]</td>
          </tr>
          <tr>
            <td align="center">135-139</td>
            <td>Reserved</td>
            <td>[<a href="https://www.iana.org/go/rfc4760">RFC4760</a>]</td>
          </tr>
          <tr>
            <td align="center">140</td>
            <td>VPN auto-discovery</td>
            <td>[<a href="https://www.iana.org/go/draft-ietf-l3vpn-bgpvpn-auto">draft-ietf-l3vpn-bgpvpn-auto</a>]</td>
          </tr>
          <tr>
            <td align="center">141-240</td>
            <td>Reserved</td>
            <td>[<a href="https://www.iana.org/go/rfc4760">RFC4760</a>]</td>
          </tr>
          <tr>
            <td align="center">241-254</td>
            <td>Reserved for Private Use</td>
            <td>[<a href="https://www.iana.org/go/rfc4760">RFC4760</a>]</td>
          </tr>
          <tr>
            <td align="center">255</td>
            <td>Reserved</td>
            <td>[<a href="https://www.iana.org/go/rfc4760">RFC4760</a>]</td>
          </tr>
        </tbody>
      </table>