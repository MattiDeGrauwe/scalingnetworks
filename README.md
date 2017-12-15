# Scaling Networks Cheat Sheet
Cheat sheet for CCNA4 - Scaling Networks

## Chapter1: Lan Design

| Description       | Command       |
|:-----------------|:-------------|
| Blabla            | `command`     |

## Chapter2: Scaling VLANs

| Description       | Command       |
|:-----------------|:-------------|
| Verify VTP status | `show vtp status`     |
| Set VTP mode client | `vtp mode client` |
| Configure VTP domain name | `vtp domain CCNA` |
| Set VTP password | `vtp password cisco12345` |
| Create VLAN | `vlan 10` |
| delete VLAN | `no vlan 10` |
| Assign name to VLAN | `name SALES` |
| Verify configured VLANs | `show vlan brief` |
| Set port to access mode | `switchport mode access` |
| Assign the port to a VLAN | `switchport access vlan 30` |
| Set port to trunk mode | `switchport mode trunk` |
| Allow VLANs to trunk | `switchport trunk allowed vlan 10, 30` |
| Assign subinterface to VLAN (routers) | `encapsulation dot1q 10` |
| Assign default gateway | `ip default-gateway 10.1.1.1` |

## Chapter3: STP

| Description       | Command       |
|:-----------------|:-------------|
| Verify Spanning Tree | `show spanning-tree` |
| Verify Spanning Tree on VLAN | `show spanning-tree vlan`|
| Enter the spanning-tree cost | `spanning-tree cost 25` |
| Reset spanning-tree cost to default | `no spanning-tree cost` |
| Ensure lowest bridge priority method 1| `spanning-tree VLAN 1 root primary`|
| Ensure root bridge method 2| `spanning-tree VLAN 1 priority 24576`|
| Ensure alternate root bridge method 1| `spanning-tree VLAN 1 root secondary`|
| Configure portfast on switch port | `spanning-tree portfast`|
| Configure BPDU guard on interface | `spanning-tree bpduguard enable`|
| Configure Rapid PVST+ mode | `spanning-tree mode rapid-pvst`|
| Specify point-to-point link type | `spanning-tree link-type point-to-point` |



## Chapter4: EtherChannel and HSRP

| Description       | Command       |
|:-----------------|:-------------|
| Blabla            | `command`     |

## Chapter5: Dynamic Routing

| Description       | Command       |
|:-----------------|:-------------|
| Blabla            | `command`     |

## Chapter6: EIGRP

| Description       | Command       |
|:-----------------|:-------------|
| Blabla            | `command`     |

## Chapter7: EIGRP Tuning and Troubleshooting

| Description       | Command       |
|:-----------------|:-------------|
| Blabla            | `command`     |

## Chapter8: Single-Area OSPF

| Description       | Command       |
|:-----------------|:-------------|
| Blabla            | `command`     |

## Chapter9: Multiarea OSPF

| Description       | Command       |
|:-----------------|:-------------|
| Blabla            | `command`     |

## Chapter10: OSPF Tuning and Troubleshooting

| Description       | Command       |
|:-----------------|:-------------|
| Blabla            | `command`     |
