# host2-DC1

## Table of Contents

- [Interfaces](#interfaces)
  - [Ethernet Interfaces](#ethernet-interfaces)
  - [Port-Channel Interfaces](#port-channel-interfaces)
- [Routing](#routing)
  - [Static Routes](#static-routes)

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
| Ethernet1 | Port Channel1 member | *routed | 1 | *10.1.20.12/24 | **default | **- | *False | **- | **- |
| Ethernet2 | Port Channel1 member | *routed | 1 | *10.1.20.12/24 | **default | **- | *False | **- | **- |
| Ethernet3 | Port Channel1 member | *routed | 1 | *10.1.20.12/24 | **default | **- | *False | **- | **- |
| Ethernet4 | Port Channel1 member | *routed | 1 | *10.1.20.12/24 | **default | **- | *False | **- | **- |
*Inherited from Port-Channel Interface

#### Ethernet Interfaces Device Configuration

```eos
!
interface Ethernet1
   description Port Channel1 member
   no shutdown
   channel-group 1 mode active
!
interface Ethernet2
   description Port Channel1 member
   no shutdown
   channel-group 1 mode active
!
interface Ethernet3
   description Port Channel1 member
   no shutdown
   channel-group 1 mode active
!
interface Ethernet4
   description Port Channel1 member
   no shutdown
   channel-group 1 mode active
```

### Port-Channel Interfaces

#### Port-Channel Interfaces Summary

##### L2

| Interface | Description | Type | Mode | VLANs | Native VLAN | Trunk Group | LACP Fallback Timeout | LACP Fallback Mode | MLAG ID | EVPN ESI |
| --------- | ----------- | ---- | ---- | ----- | ----------- | ------------| --------------------- | ------------------ | ------- | -------- |

##### IPv4

| Interface | Description | Type | MLAG ID | IP Address | VRF | MTU | Shutdown | ACL In | ACL Out |
| --------- | ----------- | ---- | ------- | ---------- | --- | --- | -------- | ------ | ------- |
| Port-Channel1 | LAG to leaf3-DC1 and leaf4-DC1 | routed | - | 10.1.20.12/24 | default | - | False | - | - |

#### Port-Channel Interfaces Device Configuration

```eos
!
interface Port-Channel1
   description LAG to leaf3-DC1 and leaf4-DC1
   no shutdown
   no switchport
   ip address 10.1.20.12/24
```

## Routing

### Static Routes

#### Static Routes Summary

| VRF | Destination Prefix | Next Hop IP             | Exit interface      | Administrative Distance       | Tag               | Route Name                    | Metric         |
| --- | ------------------ | ----------------------- | ------------------- | ----------------------------- | ----------------- | ----------------------------- | -------------- |
| default | 10.1.10.0/24 | 10.1.20.1 | - | 1 | - | - | - |

#### Static Routes Device Configuration

```eos
!
ip route 10.1.10.0/24 10.1.20.1
```
