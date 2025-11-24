# Static Routing Lab Exercise
In this lab, it demonstrates how to set static routes between devices with transit route between MLS and also with VLAN segmentation.
# Overview
This repository contains a Cisco Packet Tracer lab demonstrating how to build a small enterprise network using:
- Layer-3 Switching
- SVI-based Inter-VLAN Routing
- Static Routing
- Trunking & VLAN segmentation
- Transit VLAN between multilayer switches

# Network Topology

![Diagram](diagram/Network_Topology.png)

# VLAN and IP Addressing

| VLAN	|      Subnet      |
|-------|------------------|
| 10	  |  192.168.10.0/24 |
| 20	  |  192.168.20.0/24 |
| 30	  |  192.168.30.0/24 |
| 40	  |  192.168.40.0/24 |
| 50	  |  192.168.50.0/24 |
| 60	  |  192.168.60.0/24 |
| 90	  |  192.168.90.0/24 |

# Key Configurations
- Create SVI for vlans which are connected on MLS.
-	Create common vlan 90 to setup transit routes.
-	Config trunk link for carry vlan 90 traffic between MLS
-	Create sub-interface on router for connected vlans.
-	Set static routing on reach MLS and Routers.

Note: Make sure give ip routing command in MLSes for enable inter vlan routing.

# Note on Basic Security Configurations
This lab intentionally does not include the following initial security configurations:
-	console / VTY passwords
-	MOTD banners
-	SSH setup
-	privilege mode protection
-	password encryptions

These were omitted because the objective of this lab is strictly:
-	VLAN creation
-	SVI routing
-	Static routing
-	Trunk configuration

# What This Lab Demonstrates
-	Difference between SVI routing and router-on-a-stick
-	How multilayer switches route between VLANs
-	How transit VLAN use to set routes between MLS devices
-	How to configure static routes on L3 switches and routers

## How to Use This Repository

-	Clone the repo
-	Open the .pkt file in Cisco Packet Tracer
-	Review configurations
-	Test connectivity between all VLANs
-	Modify, break, and rebuild the design to reinforce learning

