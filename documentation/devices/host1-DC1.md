# host1-DC1
# Table of Contents

- [Management](#management)
- [Authentication](#authentication)
- [Monitoring](#monitoring)
- [Internal VLAN Allocation Policy](#internal-vlan-allocation-policy)
  - [Internal VLAN Allocation Policy Summary](#internal-vlan-allocation-policy-summary)
- [Interfaces](#interfaces)
  - [Ethernet Interfaces](#ethernet-interfaces)
  - [Port-Channel Interfaces](#port-channel-interfaces)
- [Routing](#routing)
  - [IP Routing](#ip-routing)
  - [IPv6 Routing](#ipv6-routing)
  - [Static Routes](#static-routes)
- [Multicast](#multicast)
- [Filters](#filters)
- [ACL](#acl)
- [Quality Of Service](#quality-of-service)

# Management

# Authentication

# Monitoring

# Internal VLAN Allocation Policy

## Internal VLAN Allocation Policy Summary

**Default Allocation Policy**

| Policy Allocation | Range Beginning | Range Ending |
| ------------------| --------------- | ------------ |
| ascending | 1006 | 4094 |

# Interfaces

## Ethernet Interfaces

### Ethernet Interfaces Summary

#### L2

| Interface | Description | Mode | VLANs | Native VLAN | Trunk Group | Channel-Group |
| --------- | ----------- | ---- | ----- | ----------- | ----------- | ------------- |

*Inherited from Port-Channel Interface

#### IPv4

| Interface | Description | Type | Channel Group | IP Address | VRF |  MTU | Shutdown | ACL In | ACL Out |
| --------- | ----------- | -----| ------------- | ---------- | ----| ---- | -------- | ------ | ------- |
| Ethernet1 | Port Channel1 member | *routed | 1 | *10.1.10.11/24 | **default | **- | *False | **- | **- |
| Ethernet2 | Port Channel1 member | *routed | 1 | *10.1.10.11/24 | **default | **- | *False | **- | **- |
| Ethernet3 | Port Channel1 member | *routed | 1 | *10.1.10.11/24 | **default | **- | *False | **- | **- |
| Ethernet4 | Port Channel1 member | *routed | 1 | *10.1.10.11/24 | **default | **- | *False | **- | **- |
*Inherited from Port-Channel Interface

### Ethernet Interfaces Device Configuration

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

## Port-Channel Interfaces

### Port-Channel Interfaces Summary

#### L2

| Interface | Description | Type | Mode | VLANs | Native VLAN | Trunk Group | LACP Fallback Timeout | LACP Fallback Mode | MLAG ID | EVPN ESI |
| --------- | ----------- | ---- | ---- | ----- | ----------- | ------------| --------------------- | ------------------ | ------- | -------- |

#### IPv4

| Interface | Description | Type | MLAG ID | IP Address | VRF | MTU | Shutdown | ACL In | ACL Out |
| --------- | ----------- | ---- | ------- | ---------- | --- | --- | -------- | ------ | ------- |
| Port-Channel1 | LAG to leaf1-DC1 and leaf2-DC1 | routed | - | 10.1.10.11/24 | default | - | False | - | - |

### Port-Channel Interfaces Device Configuration

```eos
!
interface Port-Channel1
   description LAG to leaf1-DC1 and leaf2-DC1
   no shutdown
   no switchport
   ip address 10.1.10.11/24
```

# Routing

## IP Routing

### IP Routing Summary

| VRF | Routing Enabled |
| --- | --------------- |
| default | False |

### IP Routing Device Configuration

```eos
```
## IPv6 Routing

### IPv6 Routing Summary

| VRF | Routing Enabled |
| --- | --------------- |
| default | False |

## Static Routes

### Static Routes Summary

| VRF | Destination Prefix | Next Hop IP             | Exit interface      | Administrative Distance       | Tag               | Route Name                    | Metric         |
| --- | ------------------ | ----------------------- | ------------------- | ----------------------------- | ----------------- | ----------------------------- | -------------- |
| default | 10.1.20.0/24 | 10.1.10.1 | - | 1 | - | - | - |

### Static Routes Device Configuration

```eos
!
ip route 10.1.20.0/24 10.1.10.1
```

# Multicast

# Filters

# ACL

# Quality Of Service