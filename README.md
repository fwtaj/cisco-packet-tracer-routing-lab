Cisco Packet Tracer – Multi-Router Network Lab (In Progress)
Overview

This project documents the setup of a small multi-site network using Cisco Packet Tracer. The lab simulates two locations (NY and LA) connected via a transit network, with each site hosting its own local area network (LAN).

This project is being continuously built on to demonstrate progressive learning in networking. At the current stage, device configuration and IP addressing have been completed. Routing and additional networking features will be implemented in future updates.

Network Topology

2 Routers

NY Router

LA Router

2 Switches

2 End Devices (PCs)

1 Transit Network connecting both routers

Each site operates on its own subnet and connects to the transit network through its local router.

IP Addressing Scheme
NY Site

Router NY

G0/1 → 192.168.10.1 /24 (NY LAN)

G0/0 → 192.168.20.1 /24 (Transit Network)

PC1

IP Address → 192.168.10.10

Subnet Mask → 255.255.255.0

Default Gateway → 192.168.10.1

LA Site

Router LA

G0/1 → 192.168.30.1 /24 (LA LAN)

G0/0 → 192.168.20.2 /24 (Transit Network)

PC2

IP Address → 192.168.30.10

Subnet Mask → 255.255.255.0

Default Gateway → 192.168.30.1

Configurations Completed

Router hostnames configured (NY, LA)

IP addresses assigned to router interfaces

Interfaces enabled using no shutdown

End devices statically configured with correct default gateways

Current Limitations

Routing between NY and LA has not yet been implemented

PCs on separate LANs cannot communicate at this stage

Planned Next Steps

Implement static routing between NY and LA routers

Verify end-to-end connectivity using ping tests

Validate routing tables using show ip route

Optionally implement a dynamic routing protocol (RIP or OSPF)

Tools & Technologies

Cisco Packet Tracer

Cisco IOS CLI

IPv4 addressing

Skills Demonstrated So Far

Interface and device configuration

IPv4 subnetting and addressing

Default gateway configuration

Basic network topology design

Project Status

Active / Work in Progress
This repository will be continuously updated as new networking concepts are implemented and tested.
