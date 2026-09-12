# Enterprise Network Routing with OSPF

## 1. Project Overview

This project demonstrates the design, configuration, and testing of a small enterprise network using Cisco Packet Tracer.

The network consists of three Cisco routers, three switches, and three PCs. The routers are connected using point-to-point links, while each router provides connectivity to a separate LAN.

OSPF (Open Shortest Path First) is configured as the dynamic routing protocol to allow the routers to automatically exchange routing information.

The project includes IP addressing, OSPF configuration, OSPF neighbor verification, routing-table verification, OSPF cost testing, connectivity testing, and link-failure testing.

---

## 2. Project Objectives

The main objectives of this project are:

- Design a small enterprise network topology.
- Configure Cisco routers and switches.
- Configure IPv4 addressing.
- Configure LAN and point-to-point networks.
- Configure OSPF dynamic routing.
- Configure unique OSPF Router IDs.
- Establish OSPF neighbor relationships.
- Verify dynamically learned routes.
- Test end-to-end network connectivity.
- Demonstrate the effect of OSPF interface cost.
- Test network behavior during a link failure.
- Verify network recovery after restoring a failed link.
- Document router configurations and verification results.

---

## 3. Network Topology

![Network Topology](images/topology.png)

The network contains three routers connected in a linear topology.

```text
                         ENTERPRISE NETWORK

       LAN 1                  WAN Links                    LAN 3

       PC1                                             PC3
        |                                               |
        |                                               |
       S1                                               S3
        |                                               |
        |                                               |
       R1 ---------------- R2 ---------------- R3
        |                  |                  |
        |                  |                  |
   192.168.10.0/24   192.168.20.0/24    192.168.30.0/24

          R1-R2: 192.168.1.0/30
          R2-R3: 192.168.2.0/30
