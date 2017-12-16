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
| Enable router configuration mode to eigrp and begin configuration process | `router eigrp 1` |
| Disable router configuration mode from eigrp| `no router eigrp 1`|
| Set router-id | `eigrp router-id 1.1.1.1` |
| Enable eigrp for the interfaces on a specific subnet| `network 172.16.0.0` |
| Enable eigrp for the interfaces on a specific subnet, but only allow allow some| `network 192.168.10.8 0.0.0.3` |
| Set interface to passive | `passive-interface g0/0` |
| Examine neighbors | `show ip eigrp neighbors` |
| Verifying eigrp active | `show ip protocols` |
| Examine routing table | `show ip route`|
| Adjust metric weight (waarschijnlijk niet nodig) | `metric weights tos k1 k2 k3 k4 k5` |
| Adjust bandwidth | `interface s0/0/0 && bandwidth 64` |
| Configure Link-local adress | `ipv6 address fe80::1 link-local` |
| Enable router configuration mode for ivp6 | `ipv6 router eigrp 2` |
| Configure unicast-routing | `ipv6 unicast-routing` |
| Configure router-id | `eigrp router-id 1.0.0.0 && no shutdown` |
| Enable eigrp on an interface | `ipv6 eigrp 2` |
| Examine ipv6 eigrp neighbors | `show ipv6 eigrp neighbors` |
| Verify ipv6 eigrp active | `show ipv6 protocols` |
| Verify ipv6 routes active | `show ipv6 route` |
| Enable auto-summary | `auto-summary` |
| Propagate (ipv6) static route | `redestribute static` |
| Configure hello timers | `ip hello-interval eigrp 1 50|
| Configure hold timers | `ip hold-time eigrp 1 150` |
| Set interface to passive | `passive interface s0/0/0` |

## Chapter7: EIGRP Tuning and Troubleshooting

| Description       | Command       |
|:-----------------|:-------------|
| Zit hierboven vanaf propagate | `command`     |

## Chapter8: Single-Area OSPF

| Description       | Command       |
|:-----------------|:-------------|
| Enable configuration mode to ospf and begin configuration process | `router ospf 10` |
| Disable router configuration mode from ospf| `no router ospf 10` |
| Set router-id | `router-id 1.1.1.1` |
| Lookback interface as router ID | `interface loopback 0 && ip address 1.1.1.1 255.255.255.255` |
| Assigning interfaces to an ospf area | `network 172.16.1.0 0.0.0.255 area 0` |
| Configure passive interfaces | `passive-interface g0/0` |
| Adjust interface bandwidth | `bandwidth 64` |
| Manually set cost | `ip ospf cost 15625` |
| Verify ospf neighbors | `show ip ospf neighbor` |
| Verify ospf settings | `show ip protocols` |
| Verify interface settings | `show ip ospf interface brief` |

## Chapter9: Multiarea OSPF

| Description       | Command       |
|:-----------------|:-------------|
| Multiarea ospf | `network 10.1.1.1 0.0.0.0 area 1 && network 192.168.10.1 0.0.0.0 area 0`     |

## Chapter10: OSPF Tuning and Troubleshooting

| Description       | Command       |
|:-----------------|:-------------|
| Propogate a Default Static route            | `default-information originate`     |
| Hello/Hold interval | `Zie eigrp` |
