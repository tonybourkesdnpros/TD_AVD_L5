# DCI

## Table of Contents

- [Interfaces](#interfaces)
  - [Ethernet Interfaces](#ethernet-interfaces)
  - [Loopback Interfaces](#loopback-interfaces)
- [Routing](#routing)
  - [Router BGP](#router-bgp)

## Interfaces

### Ethernet Interfaces

#### Ethernet Interfaces Summary

##### L2

| Interface | Description | Mode | VLANs | Native VLAN | Trunk Group | Channel-Group |
| --------- | ----------- | ---- | ----- | ----------- | ----------- | ------------- |

*Inherited from Port-Channel Interface

##### IPv4

| Interface | Description | Type | Channel Group | IP Address | VRF |  MTU | Shutdown | ACL In | ACL Out |
| --------- | ----------- | -----| ------------- | ---------- | ----| ---- | -------- | ------ | ------- |
| Ethernet1 | To borderleaf1-DC1 | routed | - | 192.168.99.1/31 | default | - | False | - | - |
| Ethernet2 | To borderleaf2-DC1 | routed | - | 192.168.99.3/31 | default | - | False | - | - |
| Ethernet3 | To borderleaf1-DC2 | routed | - | 192.168.99.5/31 | default | - | False | - | - |
| Ethernet4 | To borderleaf2-DC2 | routed | - | 192.168.99.7/31 | default | - | False | - | - |

#### Ethernet Interfaces Device Configuration

```eos
!
interface Ethernet1
   description To borderleaf1-DC1
   no shutdown
   no switchport
   ip address 192.168.99.1/31
!
interface Ethernet2
   description To borderleaf2-DC1
   no shutdown
   no switchport
   ip address 192.168.99.3/31
!
interface Ethernet3
   description To borderleaf1-DC2
   no shutdown
   no switchport
   ip address 192.168.99.5/31
!
interface Ethernet4
   description To borderleaf2-DC2
   no shutdown
   no switchport
   ip address 192.168.99.7/31
```

### Loopback Interfaces

#### Loopback Interfaces Summary

##### IPv4

| Interface | Description | VRF | IP Address |
| --------- | ----------- | --- | ---------- |
| Loopback99 | - | default | 192.168.99.255/32 |

##### IPv6

| Interface | Description | VRF | IPv6 Address |
| --------- | ----------- | --- | ------------ |
| Loopback99 | - | default | - |


#### Loopback Interfaces Device Configuration

```eos
!
interface Loopback99
   no shutdown
   ip address 192.168.99.255/32
```

## Routing

### Router BGP

#### Router BGP Summary

| BGP AS | Router ID |
| ------ | --------- |
| 65000|  192.168.99.255 |

#### Router BGP Peer Groups

##### UNDERLAY

| Settings | Value |
| -------- | ----- |

#### BGP Neighbors

| Neighbor | Remote AS | VRF | Shutdown | Send-community | Maximum-routes | Allowas-in | BFD | RIB Pre-Policy Retain | Route-Reflector Client | Passive |
| -------- | --------- | --- | -------- | -------------- | -------------- | ---------- | --- | --------------------- | ---------------------- | ------- |
| 192.168.99.0 | 65104 | default | - | - | - | - | - | - | - | - |
| 192.168.99.2 | 65104 | default | - | - | - | - | - | - | - | - |
| 192.168.99.4 | 65204 | default | - | - | - | - | - | - | - | - |
| 192.168.99.6 | 65204 | default | - | - | - | - | - | - | - | - |

#### Router BGP Device Configuration

```eos
!
router bgp 65000
   router-id 192.168.99.255
   neighbor UNDERLAY peer group
   neighbor 192.168.99.0 remote-as 65104
   neighbor 192.168.99.2 remote-as 65104
   neighbor 192.168.99.4 remote-as 65204
   neighbor 192.168.99.6 remote-as 65204
```
