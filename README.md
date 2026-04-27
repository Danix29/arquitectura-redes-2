<img src="https://capsule-render.vercel.app/api?type=waving&color=1BA0D7&height=160&section=header&text=arquitectura-redes-2&fontSize=28&fontColor=FFFFFF&fontAlignY=40&desc=Arquitectura%20de%20Redes%20II%20%7C%20UAH%202025-26&descAlignY=60&descColor=9FE1CB" width="100%"/>

<div align="center">

![Cisco](https://img.shields.io/badge/Cisco%20IOS-1BA0D7?style=for-the-badge&logo=cisco&logoColor=white)
![Wireshark](https://img.shields.io/badge/Wireshark-1679A7?style=for-the-badge&logo=wireshark&logoColor=white)
![UAH](https://img.shields.io/badge/UAH-GII-085041?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Active-1D9E75?style=for-the-badge)

</div>

---

## About

**Asignatura:** Arquitectura de Redes II · UAH GII · Curso 2025-26

Advanced networking: dynamic routing protocols, network redundancy, traffic engineering, security and quality of service. Continuation of Arquitectura de Redes I with enterprise-level scenarios.

---

## Topics covered

| Topic | Content |
|-------|---------|
| OSPF | Link-state routing, areas, LSA types, DR/BDR election |
| EIGRP | Cisco proprietary, DUAL algorithm, feasible successors |
| BGP | Path vector, eBGP vs iBGP, AS numbers, policy routing |
| VLANs advanced | Inter-VLAN routing, Layer 3 switches, trunking protocols |
| Spanning Tree | STP, RSTP, PVST+, loop prevention |
| Network security | ACLs, NAT/PAT, port security, DHCP snooping |
| Traffic engineering | QoS, bandwidth management, traffic shaping |

---

## Practices

| # | Name | Description |
|---|------|-------------|
| P1 | OSPF single area | OSPF configuration and convergence analysis |
| P2 | OSPF multi-area | ABR configuration, route summarisation |
| P3 | BGP | eBGP peering between autonomous systems |
| P4 | Network security | ACL design and NAT configuration |
| P5 | Spanning Tree | RSTP and loop prevention in redundant topology |

---

## Key configuration snippets

```bash
# OSPF
Router(config)# router ospf 1
Router(config-router)# network 10.0.0.0 0.0.0.255 area 0
Router(config-router)# router-id 1.1.1.1

# BGP
Router(config)# router bgp 65001
Router(config-router)# neighbor 203.0.113.1 remote-as 65002
Router(config-router)# network 10.0.0.0 mask 255.255.255.0

# Standard ACL
Router(config)# access-list 10 permit 192.168.1.0 0.0.0.255
Router(config)# interface GigabitEthernet0/1
Router(config-if)# ip access-group 10 in
```

---

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=1BA0D7&height=100&section=footer" width="100%"/>

*Arquitectura de Redes II · UAH GII · 2025-26*
</div>
