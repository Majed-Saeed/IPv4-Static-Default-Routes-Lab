# IPv4-Static-Default-Routes-Lab
Cisco Packet Tracer project demonstrating IPv4 static and default route configuration.
IPv4 Static and Default Routes Lab

This project demonstrates the configuration of IPv4 static routes (recursive and directly connected) and a default route using Cisco Packet Tracer. The lab includes IP addressing, router configuration, connectivity verification, and troubleshooting.

Objectives

Configure IPv4 addressing on routers and PCs.

Implement recursive and directly connected static routes.

Configure a default route (“quad zero”).

Verify LAN and inter-network connectivity.

Test and troubleshoot routing issues.

Topology

(Insert your topology screenshot here once uploaded)

Addressing Table
Device	Interface	IP Address	Subnet Mask	Default Gateway
R1	G0/1	192.168.0.1	255.255.255.0	N/A
R1	S0/0/1	10.1.1.1	255.255.255.252	N/A
R3	G0/1	192.168.1.1	255.255.255.0	N/A
R3	S0/0/0	10.1.1.2	255.255.255.252	N/A
PC-A	NIC	192.168.0.10	255.255.255.0	192.168.0.1
PC-C	NIC	192.168.1.10	255.255.255.0	192.168.1.1
Commands Used (Examples)
ip route 192.168.1.0 255.255.255.0 10.1.1.2
ip route 0.0.0.0 0.0.0.0 10.1.1.2

Results

Successful pings between PC-A and PC-C after static routes were configured.

Default route allowed access to remote loopback networks.

Tools Used

Cisco Packet Tracer (v8.x recommended)

Cisco IOS 15.x
