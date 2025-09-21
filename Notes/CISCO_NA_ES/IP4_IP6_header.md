## IPv4 Packet Header

![alt text](https://github.com/masson-js/Cybersecurity/blob/main/Notes/CISCO_NA_ES/images/ip4header.png?raw=true)

- Contains a 4-bit binary value set to 0100 that identifies this as an IPv4 packet.
- A 4-bit field containing the length of the IP header.
- The minimum length of an IP header is 20 bytes.
- Formerly called the Type of Service (ToS) field, the DS field is an 8-bit field used to determine the priority of each packet.
- The six most significant bits of the DiffServ field are the Differentiated Services Code Point (DSCP).
- The last two bits are the Explicit Congestion Notification (ECN) bits.
- Specifies the length of the IP packet including the IP header and the user data.
- The total length field is 2 bytes, so the maximum size of an IP packet is 65,535 bytes; however, packets are much smaller in practice.
- As an IP packet moves through the internet, it might need to cross a route that cannot handle the size of the packet.
- The packet will be divided, or fragmented, into smaller packets and reassembled later.
- These fields are used to fragment and reassemble packets.
- Contains an 8-bit binary value that is used to limit the lifetime of a packet.
- The packet sender sets the initial TTL value, and it is decreased by one each time the packet is processed by a router.
- If the TTL field decrements to zero, the router discards the packet and sends an Internet Control Message Protocol (ICMP) Time Exceeded message to the source IP address.
- Field is used to identify the next level protocol.
- This 8-bit binary value indicates the data payload type that the packet is carrying, which enables the network layer to pass the data to the appropriate upper-layer protocol.
- Common values include ICMP (1), TCP (6), and UDP (17).
- A value that is calculated based on the contents of the IP header.
- Used to determine if any errors have been introduced during transmission.
- Contains a 32-bit binary value that represents the source IPv4 address of the packet.
- The source IPv4 address is always a unicast address.
- Contains a 32-bit binary value that represents the destination IPv4 address of the packet.
- This is a field that varies in length from 0 to a multiple of 32 bits.
- If the option values are not a multiple of 32 bits, 0s are added, or padded, to ensure that this field contains a multiple of 32 bits.

![ip4sample](https://github.com/masson-js/Cybersecurity/blob/main/Notes/CISCO_NA_ES/images/ip4sample.png?raw=true)

## Pv6 Packet Header

![ip6header](https://github.com/masson-js/Cybersecurity/blob/main/Notes/CISCO_NA_ES/images/ip6header.png?raw=true)

- This field contains a 4-bit binary value set to 0110 that identifies this as an IPv6 packet.
- This 8-bit field is equivalent to the IPv4 Differentiated Services (DS) field.
- This 20-bit field suggests that all packets with the same flow label receive the same type of handling by routers.
- This 16-bit field indicates the length of the data portion or payload of the IPv6 packet.
- This 8-bit field is equivalent to the IPv4 Protocol field.
- It indicates the data payload type that the packet is carrying, enabling the network layer to pass the data to the appropriate upper-layer protocol.
- This 8-bit field replaces the IPv4 TTL field.
- This value is decremented by a value of 1 by each router that forwards the packet.
- When the counter reaches 0, the packet is discarded, and an ICMPv6 Time Exceeded message is forwarded to the sending host, indicating that the packet did not reach its destination because the hop limit was exceeded.
- This 128-bit field identifies the IPv6 address of the sending host.
- This 128-bit field identifies the IPv6 address of the receiving host.

![ip6sample](https://github.com/masson-js/Cybersecurity/blob/main/Notes/CISCO_NA_ES/images/ip6sample.png?raw=true)