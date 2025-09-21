# SANS 401 Network Security Cloud Essentials

## Sampling of possible router attacks:

**DoS** - service of the device is being impacted (denied). Example: Router is offline on 10 min. patching time, the organizaton suffers a loss ot money.

**DDoS** - attacks are essentially the same as DoS, albeit with one significant different - launch attack from many locations, simultaneously. You can't defense through the implementation of an ACL (access control list)

**Packet Sniffing** - refests to the capture (and analysis) of the traffic of a network ( the network's communication)

**Packet Missrouting and Routing Table Poising** - with packet missrouting, a router's configuration is manipulated such that traffic is no longer routed prperly; trafic might be routed to non-existent network locations, or looping. RTP - the adversary convinces a router to update it's routing table, resulting in traffic redirection.

## Sampling of possible switch attacks:

**CDP Information Disclosure** - CISCO Discovery Protocol - Lack of encryption and authentication enables data interception, man-in-the-middle attacks, or DoS via spoofed packets.Open ifo about OS, Ports and other in Packets via Switches