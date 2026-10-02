# 📁 06-Enterprise-Network

```markdown
# Project 06: Enterprise Core Architecture, Edge Routing & Internet Egress

## 📌 Overview
Comprehensive enterprise network infrastructure integrating hierarchical Layer 3 Core distribution, Access layer switching, border routing (`R-EDGE-01`), and Internet egress. Features full Inter-VLAN routing, dynamic multi-pool DHCP, Layer 3 P2P transit links, and Network Address Translation (NAT/PAT).

## 📐 Network Architecture & Subnetting
```text
[ Access Layer ]  ─── (Trunks / Native VLAN 99) ─── [ DSW-CORE-01 ]
ASW-ACC-01 / 02                                            │ P2P Link: 10.10.100.0/30
                                                    [ R-EDGE-01 ]
                                                           │ WAN / NAT / PAT
                                                     [ ISP / Internet ]