# Flowspec

https://tools.ietf.org/html/rfc5575

Actions
```
+--------+--------------------+--------------------------+
| type   | extended community | encoding                 |
+--------+--------------------+--------------------------+
| 0x8006 | traffic-rate       | 2-byte as#, 4-byte float |
| 0x8007 | traffic-action     | bitmask                  |
| 0x8008 | redirect           | 6-byte Route Target      |
| 0x8009 | traffic-marking    | DSCP value               |
+--------+--------------------+--------------------------+
```

NLRI

     Type 1 - Destination Prefix
     Type 2 - Source Prefix       
     Type 3 - IP Protocol       
     Type 4 - Port       
     Type 5 - Destination port
     Type 6 - Source port       
     Type 7 - ICMP type       
     Type 8 - ICMP code       
     Type 9 - TCP flags       
     Type 10 - Packet length
     Type 11 - DSCP       
     Type 12 - Fragment