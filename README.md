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
| Verify EtherChannel configuration | `show interfaces port-channel 1`|
| Verify EtherChannel different channels | `show etherchannel summary`|
| Verify role of the interface in Etherchannel | `show interfaces f0/1 etherchannel`|
| Verify EtherChannel port channels | `show etherchannel port-channel`|
| Select desired interface range | `interface range f0/1-2`|
| Create port channel interface | `channel-group 1 mode active`|
| Enter port channel interface | `interface port-channel 1`|
| Verify HSRP configuration | `show standby brief`|
| Configure HSRP to use version 2 | `standby version 2`|
| Configure virtual IP that will be used by group | `standby 10 ip 192.168.1.1` |
| Configure priorty that will be used for group | `standby 10 priority 100`|
| Configure the router to preempt | `stadby 10 preempt`|
| Debug HSRP | `debug standby packets`|
| Debug HSRP | `debug standby terse`|

## Chapter5: Dynamic Routing

Enkel theorie

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
