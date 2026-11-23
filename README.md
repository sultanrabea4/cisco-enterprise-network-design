# Enterprise Network Design & Security (Cisco Packet Tracer)

A collection of **Cisco Packet Tracer** network designs, from campus networks to a **multi-site enterprise network** with a **Wireless LAN Controller (WLC)**, **RADIUS**, **HSRP**, a **server farm** and **Layer 2 security hardening**.

---

## 1. Multi-Site Enterprise Network with WLC (main project)
**File:** `packet-tracer/enterprise-multisite-wlc.pkt`

An IT upgrade design for a fictional company with a **Kuala Lumpur HQ** (Management, HR, Design, Delivery) and a remote **Krung Thep (KT) branch** (R&D, WLC management, server farm).

> System & Network Engineering group project (5 members). **I was the team leader** and built **~70% of the KT branch** and **a share of the WAN**.

**Technologies**
| Area | Implementation |
|---|---|
| Segmentation | VLANs per department, **inter-VLAN routing**, trunking, native VLAN 99 |
| Wireless (KT) | **Wireless LAN Controller** managed from an admin PC, **RADIUS** authentication, custom WLANs |
| Redundancy | **EtherChannel**, **HSRP** gateway redundancy |
| Services | Server farm with **DNS**, **Web**, **FTP** and DHCP |
| Voice | IP phone configuration |
| WAN | Inter-site routing between HQ and branch |
| Verification | End-to-end `ping` / `tracert` testing |

**Layer 2 security (KT branch)**
- **Black-hole VLAN 100** for unused ports
- **Port security** with sticky MAC addresses and `restrict` violation mode
- **DHCP snooping** and **Dynamic ARP Inspection**
- **SSH-only** VTY access with passwords
- **Extended ACL** limiting access to admin servers

## 2. DHCP Lab
**File:** `packet-tracer/dhcp-lab.pkt`. Centralised DHCP addressing for multiple network segments.

## 3. Multi-Site Network (group, year 1)
**File:** `packet-tracer/multisite-network-group.pkt`. Multi-site design with **VLSM subnetting** and routing between sites.

## 4. Campus Network (individual, year 1)
**File:** `packet-tracer/campus-network-individual.pkt`. A campus LAN with structured addressing.

## 5. NAT / PAT Labs
Completed the Cisco NetAcad Packet Tracer activities for **Static NAT**, **Dynamic NAT** and **PAT (NAT overload)**: inside/outside interfaces, NAT pools, ACL-based translation and verification with `show ip nat translations`. The activity files belong to Cisco NetAcad, so they are not included here.

---

## Skills Demonstrated
VLAN design · inter-VLAN routing · WLC/WLAN · RADIUS · EtherChannel · HSRP · DHCP / DNS / FTP / Web services · NAT/PAT · port security · DHCP snooping · DAI · ACLs · troubleshooting

## How to Open
Install **Cisco Packet Tracer 8.x or newer** (free through Cisco NetAcad) and open any `.pkt` file.

## Author
**Sultan Mohammed Rabea** · [LinkedIn](https://www.linkedin.com/in/sultan-rabea/) · [GitHub](https://github.com/sultanrabea4)
