# Packet Tracer: Identify MAC and IP Addresses

## Project Overview
This hands-on networking lab uses Cisco Packet Tracer to examine how Ethernet frames and IPv4 packets travel across local and remote networks. The activity focuses on MAC addressing, IP addressing, router forwarding, and ICMP communication.

## Objectives
- Identify source and destination MAC addresses.
- Examine source and destination IPv4 addresses.
- Compare local and remote network communication.
- Observe how routers forward packets between networks.
- Analyze ICMP echo requests and echo replies using Simulation Mode.

## Tools Used
- Cisco Packet Tracer
- IPv4 networking
- Ethernet and wireless networking
- ICMP (ping)
- OSI model and PDU analysis

## Lab Topology
The activity uses two IP networks:

- Local network: `172.16.31.0` (subnet mask to be verified in Packet Tracer)
- Remote network: `10.10.10.0` (subnet mask to be verified in Packet Tracer)

The router connects the two networks and acts as the default gateway for remote communication.

## Tasks Performed
1. Sent ICMP echo requests between hosts on the local network.
2. Inspected Ethernet frame and IPv4 packet headers in Simulation Mode.
3. Recorded source and destination MAC and IP addresses.
4. Sent ICMP echo requests to a host on a remote network.
5. Examined inbound and outbound PDUs at the router.
6. Compared echo requests with echo replies.

## Key Findings

### Local Network Communication
- Devices on the same IP network can communicate directly at Layer 2.
- The destination MAC address identifies the receiving host.
- A default gateway is not required for communication between hosts on the same subnet.

### Remote Network Communication
- A host sends a frame to its default gateway when the destination is on a remote network.
- The router removes the incoming Layer 2 frame and forwards the IP packet in a new frame on the outgoing network.
- The MAC addresses change across routed network segments.
- The source and destination IPv4 addresses normally remain unchanged during routing without NAT.
- Echo replies reverse the source and destination IP addresses.

## OSI Model
- Layer 1 — Physical: cables and signal transmission.
- Layer 2 — Data Link: Ethernet frames and MAC addressing.
- Layer 3 — Network: IPv4 addressing and routing.

## Skills Demonstrated
- Network troubleshooting fundamentals
- MAC and IPv4 address analysis
- Packet and frame inspection
- Router forwarding concepts
- ICMP testing using ping
- Understanding local versus remote communication


## Conclusion
This lab demonstrates how MAC addresses and IPv4 addresses work together to deliver data across local and remote networks. It reinforces the role of Layer 2 switching, Layer 3 routing, and ICMP in network communication.
