
# Validate State Report

**Table of Contents:**

- [Validate State Report](validate-state-report)
  - [Test Results Summary](#test-results-summary)
  - [Failed Test Results Summary](#failed-test-results-summary)
  - [All Test Results](#all-test-results)

## Test Results Summary

### Summary Totals

| Total Tests | Total Tests Passed | Total Tests Failed |
| ----------- | ------------------ | ------------------ |
| 263 | 211 | 52 |

### Summary Totals Devices Under Tests

| DUT | Total Tests | Tests Passed | Tests Failed | Categories Failed |
| --- | ----------- | ------------ | ------------ | ----------------- |
| leaf1-DC1 |  50 | 40 | 10 | IP Reachability, Loopback0 Reachability |
| leaf2-DC1 |  50 | 40 | 10 | IP Reachability, Loopback0 Reachability |
| leaf3-DC1 |  47 | 37 | 10 | IP Reachability, Loopback0 Reachability |
| leaf4-DC1 |  47 | 37 | 10 | IP Reachability, Loopback0 Reachability |
| spine1-DC1 |  23 | 19 | 4 | IP Reachability |
| spine2-DC1 |  23 | 19 | 4 | IP Reachability |
| spine3-DC1 |  23 | 19 | 4 | IP Reachability |

### Summary Totals Per Category

| Test Category | Total Tests | Tests Passed | Tests Failed |
| ------------- | ----------- | ------------ | ------------ |
| NTP |  7 | 7 | 0 |
| Interface State |  73 | 73 | 0 |
| LLDP Topology |  32 | 32 | 0 |
| MLAG |  4 | 4 | 0 |
| IP Reachability |  24 | 0 | 24 |
| BGP |  59 | 59 | 0 |
| Routing Table |  36 | 36 | 0 |
| Loopback0 Reachability |  28 | 0 | 28 |

## Failed Test Results Summary

| Test ID | Node | Test Category | Test Description | Test | Test Result | Failure Reason |
| ------- | ---- | ------------- | ---------------- | ---- | ----------- | -------------- |
| 117 | leaf1-DC1 | IP Reachability | ip reachability test p2p links | Source: leaf1-DC1_Ethernet3 - Destination: spine1-DC1_Ethernet2 | FAIL | 100% packet loss |
| 118 | leaf1-DC1 | IP Reachability | ip reachability test p2p links | Source: leaf1-DC1_Ethernet4 - Destination: spine2-DC1_Ethernet2 | FAIL | 100% packet loss |
| 119 | leaf1-DC1 | IP Reachability | ip reachability test p2p links | Source: leaf1-DC1_Ethernet5 - Destination: spine3-DC1_Ethernet2 | FAIL | 100% packet loss |
| 120 | leaf2-DC1 | IP Reachability | ip reachability test p2p links | Source: leaf2-DC1_Ethernet3 - Destination: spine1-DC1_Ethernet3 | FAIL | 100% packet loss |
| 121 | leaf2-DC1 | IP Reachability | ip reachability test p2p links | Source: leaf2-DC1_Ethernet4 - Destination: spine2-DC1_Ethernet3 | FAIL | 100% packet loss |
| 122 | leaf2-DC1 | IP Reachability | ip reachability test p2p links | Source: leaf2-DC1_Ethernet5 - Destination: spine3-DC1_Ethernet3 | FAIL | 100% packet loss |
| 123 | leaf3-DC1 | IP Reachability | ip reachability test p2p links | Source: leaf3-DC1_Ethernet3 - Destination: spine1-DC1_Ethernet4 | FAIL | 100% packet loss |
| 124 | leaf3-DC1 | IP Reachability | ip reachability test p2p links | Source: leaf3-DC1_Ethernet4 - Destination: spine2-DC1_Ethernet4 | FAIL | 100% packet loss |
| 125 | leaf3-DC1 | IP Reachability | ip reachability test p2p links | Source: leaf3-DC1_Ethernet5 - Destination: spine3-DC1_Ethernet4 | FAIL | 100% packet loss |
| 126 | leaf4-DC1 | IP Reachability | ip reachability test p2p links | Source: leaf4-DC1_Ethernet3 - Destination: spine1-DC1_Ethernet5 | FAIL | 100% packet loss |
| 127 | leaf4-DC1 | IP Reachability | ip reachability test p2p links | Source: leaf4-DC1_Ethernet4 - Destination: spine2-DC1_Ethernet5 | FAIL | 100% packet loss |
| 128 | leaf4-DC1 | IP Reachability | ip reachability test p2p links | Source: leaf4-DC1_Ethernet5 - Destination: spine3-DC1_Ethernet5 | FAIL | 100% packet loss |
| 129 | spine1-DC1 | IP Reachability | ip reachability test p2p links | Source: spine1-DC1_Ethernet2 - Destination: leaf1-DC1_Ethernet3 | FAIL | 100% packet loss |
| 130 | spine1-DC1 | IP Reachability | ip reachability test p2p links | Source: spine1-DC1_Ethernet3 - Destination: leaf2-DC1_Ethernet3 | FAIL | 100% packet loss |
| 131 | spine1-DC1 | IP Reachability | ip reachability test p2p links | Source: spine1-DC1_Ethernet4 - Destination: leaf3-DC1_Ethernet3 | FAIL | 100% packet loss |
| 132 | spine1-DC1 | IP Reachability | ip reachability test p2p links | Source: spine1-DC1_Ethernet5 - Destination: leaf4-DC1_Ethernet3 | FAIL | 100% packet loss |
| 133 | spine2-DC1 | IP Reachability | ip reachability test p2p links | Source: spine2-DC1_Ethernet2 - Destination: leaf1-DC1_Ethernet4 | FAIL | 100% packet loss |
| 134 | spine2-DC1 | IP Reachability | ip reachability test p2p links | Source: spine2-DC1_Ethernet3 - Destination: leaf2-DC1_Ethernet4 | FAIL | 100% packet loss |
| 135 | spine2-DC1 | IP Reachability | ip reachability test p2p links | Source: spine2-DC1_Ethernet4 - Destination: leaf3-DC1_Ethernet4 | FAIL | 100% packet loss |
| 136 | spine2-DC1 | IP Reachability | ip reachability test p2p links | Source: spine2-DC1_Ethernet5 - Destination: leaf4-DC1_Ethernet4 | FAIL | 100% packet loss |
| 137 | spine3-DC1 | IP Reachability | ip reachability test p2p links | Source: spine3-DC1_Ethernet2 - Destination: leaf1-DC1_Ethernet5 | FAIL | 100% packet loss |
| 138 | spine3-DC1 | IP Reachability | ip reachability test p2p links | Source: spine3-DC1_Ethernet3 - Destination: leaf2-DC1_Ethernet5 | FAIL | 100% packet loss |
| 139 | spine3-DC1 | IP Reachability | ip reachability test p2p links | Source: spine3-DC1_Ethernet4 - Destination: leaf3-DC1_Ethernet5 | FAIL | 100% packet loss |
| 140 | spine3-DC1 | IP Reachability | ip reachability test p2p links | Source: spine3-DC1_Ethernet5 - Destination: leaf4-DC1_Ethernet5 | FAIL | 100% packet loss |
| 236 | leaf1-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf1-DC1 - 192.168.101.1 Destination: 192.168.101.1 | FAIL | 100% packet loss |
| 237 | leaf1-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf1-DC1 - 192.168.101.1 Destination: 192.168.101.2 | FAIL | 100% packet loss |
| 238 | leaf1-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf1-DC1 - 192.168.101.1 Destination: 192.168.101.3 | FAIL | 100% packet loss |
| 239 | leaf1-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf1-DC1 - 192.168.101.1 Destination: 192.168.101.4 | FAIL | 100% packet loss |
| 240 | leaf1-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf1-DC1 - 192.168.101.1 Destination: 192.168.101.11 | FAIL | 100% packet loss |
| 241 | leaf1-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf1-DC1 - 192.168.101.1 Destination: 192.168.101.12 | FAIL | 100% packet loss |
| 242 | leaf1-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf1-DC1 - 192.168.101.1 Destination: 192.168.101.13 | FAIL | 100% packet loss |
| 243 | leaf2-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf2-DC1 - 192.168.101.2 Destination: 192.168.101.1 | FAIL | 100% packet loss |
| 244 | leaf2-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf2-DC1 - 192.168.101.2 Destination: 192.168.101.2 | FAIL | 100% packet loss |
| 245 | leaf2-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf2-DC1 - 192.168.101.2 Destination: 192.168.101.3 | FAIL | 100% packet loss |
| 246 | leaf2-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf2-DC1 - 192.168.101.2 Destination: 192.168.101.4 | FAIL | 100% packet loss |
| 247 | leaf2-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf2-DC1 - 192.168.101.2 Destination: 192.168.101.11 | FAIL | 100% packet loss |
| 248 | leaf2-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf2-DC1 - 192.168.101.2 Destination: 192.168.101.12 | FAIL | 100% packet loss |
| 249 | leaf2-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf2-DC1 - 192.168.101.2 Destination: 192.168.101.13 | FAIL | 100% packet loss |
| 250 | leaf3-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf3-DC1 - 192.168.101.3 Destination: 192.168.101.1 | FAIL | 100% packet loss |
| 251 | leaf3-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf3-DC1 - 192.168.101.3 Destination: 192.168.101.2 | FAIL | 100% packet loss |
| 252 | leaf3-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf3-DC1 - 192.168.101.3 Destination: 192.168.101.3 | FAIL | 100% packet loss |
| 253 | leaf3-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf3-DC1 - 192.168.101.3 Destination: 192.168.101.4 | FAIL | 100% packet loss |
| 254 | leaf3-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf3-DC1 - 192.168.101.3 Destination: 192.168.101.11 | FAIL | 100% packet loss |
| 255 | leaf3-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf3-DC1 - 192.168.101.3 Destination: 192.168.101.12 | FAIL | 100% packet loss |
| 256 | leaf3-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf3-DC1 - 192.168.101.3 Destination: 192.168.101.13 | FAIL | 100% packet loss |
| 257 | leaf4-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf4-DC1 - 192.168.101.4 Destination: 192.168.101.1 | FAIL | 100% packet loss |
| 258 | leaf4-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf4-DC1 - 192.168.101.4 Destination: 192.168.101.2 | FAIL | 100% packet loss |
| 259 | leaf4-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf4-DC1 - 192.168.101.4 Destination: 192.168.101.3 | FAIL | 100% packet loss |
| 260 | leaf4-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf4-DC1 - 192.168.101.4 Destination: 192.168.101.4 | FAIL | 100% packet loss |
| 261 | leaf4-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf4-DC1 - 192.168.101.4 Destination: 192.168.101.11 | FAIL | 100% packet loss |
| 262 | leaf4-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf4-DC1 - 192.168.101.4 Destination: 192.168.101.12 | FAIL | 100% packet loss |
| 263 | leaf4-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf4-DC1 - 192.168.101.4 Destination: 192.168.101.13 | FAIL | 100% packet loss |

## All Test Results

| Test ID | Node | Test Category | Test Description | Test | Test Result | Failure Reason |
| ------- | ---- | ------------- | ---------------- | ---- | ----------- | -------------- |
| 1 | leaf1-DC1 | NTP | Synchronised with NTP server | NTP | PASS | - |
| 2 | leaf2-DC1 | NTP | Synchronised with NTP server | NTP | PASS | - |
| 3 | leaf3-DC1 | NTP | Synchronised with NTP server | NTP | PASS | - |
| 4 | leaf4-DC1 | NTP | Synchronised with NTP server | NTP | PASS | - |
| 5 | spine1-DC1 | NTP | Synchronised with NTP server | NTP | PASS | - |
| 6 | spine2-DC1 | NTP | Synchronised with NTP server | NTP | PASS | - |
| 7 | spine3-DC1 | NTP | Synchronised with NTP server | NTP | PASS | - |
| 8 | leaf1-DC1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet1 - MLAG_PEER_leaf2-DC1_Ethernet1 | PASS | - |
| 9 | leaf1-DC1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet2 - MLAG_PEER_leaf2-DC1_Ethernet2 | PASS | - |
| 10 | leaf1-DC1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet3 - P2P_LINK_TO_SPINE1-DC1_Ethernet2 | PASS | - |
| 11 | leaf1-DC1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet4 - P2P_LINK_TO_SPINE2-DC1_Ethernet2 | PASS | - |
| 12 | leaf1-DC1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet5 - P2P_LINK_TO_SPINE3-DC1_Ethernet2 | PASS | - |
| 13 | leaf1-DC1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet6 - host1-DC1_Ethernet1 | PASS | - |
| 14 | leaf1-DC1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet7 - host1-DC1_Ethernet2 | PASS | - |
| 15 | leaf2-DC1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet1 - MLAG_PEER_leaf1-DC1_Ethernet1 | PASS | - |
| 16 | leaf2-DC1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet2 - MLAG_PEER_leaf1-DC1_Ethernet2 | PASS | - |
| 17 | leaf2-DC1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet3 - P2P_LINK_TO_SPINE1-DC1_Ethernet3 | PASS | - |
| 18 | leaf2-DC1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet4 - P2P_LINK_TO_SPINE2-DC1_Ethernet3 | PASS | - |
| 19 | leaf2-DC1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet5 - P2P_LINK_TO_SPINE3-DC1_Ethernet3 | PASS | - |
| 20 | leaf2-DC1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet6 - host1-DC1_Ethernet3 | PASS | - |
| 21 | leaf2-DC1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet7 - host1-DC1_Ethernet4 | PASS | - |
| 22 | leaf3-DC1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet1 - MLAG_PEER_leaf4-DC1_Ethernet1 | PASS | - |
| 23 | leaf3-DC1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet2 - MLAG_PEER_leaf4-DC1_Ethernet2 | PASS | - |
| 24 | leaf3-DC1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet3 - P2P_LINK_TO_SPINE1-DC1_Ethernet4 | PASS | - |
| 25 | leaf3-DC1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet4 - P2P_LINK_TO_SPINE2-DC1_Ethernet4 | PASS | - |
| 26 | leaf3-DC1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet5 - P2P_LINK_TO_SPINE3-DC1_Ethernet4 | PASS | - |
| 27 | leaf4-DC1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet1 - MLAG_PEER_leaf3-DC1_Ethernet1 | PASS | - |
| 28 | leaf4-DC1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet2 - MLAG_PEER_leaf3-DC1_Ethernet2 | PASS | - |
| 29 | leaf4-DC1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet3 - P2P_LINK_TO_SPINE1-DC1_Ethernet5 | PASS | - |
| 30 | leaf4-DC1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet4 - P2P_LINK_TO_SPINE2-DC1_Ethernet5 | PASS | - |
| 31 | leaf4-DC1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet5 - P2P_LINK_TO_SPINE3-DC1_Ethernet5 | PASS | - |
| 32 | spine1-DC1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet2 - P2P_LINK_TO_LEAF1-DC1_Ethernet3 | PASS | - |
| 33 | spine1-DC1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet3 - P2P_LINK_TO_LEAF2-DC1_Ethernet3 | PASS | - |
| 34 | spine1-DC1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet4 - P2P_LINK_TO_LEAF3-DC1_Ethernet3 | PASS | - |
| 35 | spine1-DC1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet5 - P2P_LINK_TO_LEAF4-DC1_Ethernet3 | PASS | - |
| 36 | spine2-DC1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet2 - P2P_LINK_TO_LEAF1-DC1_Ethernet4 | PASS | - |
| 37 | spine2-DC1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet3 - P2P_LINK_TO_LEAF2-DC1_Ethernet4 | PASS | - |
| 38 | spine2-DC1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet4 - P2P_LINK_TO_LEAF3-DC1_Ethernet4 | PASS | - |
| 39 | spine2-DC1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet5 - P2P_LINK_TO_LEAF4-DC1_Ethernet4 | PASS | - |
| 40 | spine3-DC1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet2 - P2P_LINK_TO_LEAF1-DC1_Ethernet5 | PASS | - |
| 41 | spine3-DC1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet3 - P2P_LINK_TO_LEAF2-DC1_Ethernet5 | PASS | - |
| 42 | spine3-DC1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet4 - P2P_LINK_TO_LEAF3-DC1_Ethernet5 | PASS | - |
| 43 | spine3-DC1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet5 - P2P_LINK_TO_LEAF4-DC1_Ethernet5 | PASS | - |
| 44 | leaf1-DC1 | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel1 - MLAG_PEER_leaf2-DC1_Po1 | PASS | - |
| 45 | leaf1-DC1 | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel6 - host1-DC1_PortChannel host1 | PASS | - |
| 46 | leaf2-DC1 | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel1 - MLAG_PEER_leaf1-DC1_Po1 | PASS | - |
| 47 | leaf2-DC1 | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel6 - host1-DC1_PortChannel host1 | PASS | - |
| 48 | leaf3-DC1 | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel1 - MLAG_PEER_leaf4-DC1_Po1 | PASS | - |
| 49 | leaf4-DC1 | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel1 - MLAG_PEER_leaf3-DC1_Po1 | PASS | - |
| 50 | leaf1-DC1 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4093 - MLAG_PEER_L3_PEERING | PASS | - |
| 51 | leaf1-DC1 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4094 - MLAG_PEER | PASS | - |
| 52 | leaf1-DC1 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan10 - DMZ | PASS | - |
| 53 | leaf1-DC1 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan3009 - MLAG_PEER_L3_iBGP: vrf VRF_A | PASS | - |
| 54 | leaf2-DC1 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4093 - MLAG_PEER_L3_PEERING | PASS | - |
| 55 | leaf2-DC1 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4094 - MLAG_PEER | PASS | - |
| 56 | leaf2-DC1 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan10 - DMZ | PASS | - |
| 57 | leaf2-DC1 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan3009 - MLAG_PEER_L3_iBGP: vrf VRF_A | PASS | - |
| 58 | leaf3-DC1 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4093 - MLAG_PEER_L3_PEERING | PASS | - |
| 59 | leaf3-DC1 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4094 - MLAG_PEER | PASS | - |
| 60 | leaf3-DC1 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan10 - DMZ | PASS | - |
| 61 | leaf3-DC1 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan3009 - MLAG_PEER_L3_iBGP: vrf VRF_A | PASS | - |
| 62 | leaf4-DC1 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4093 - MLAG_PEER_L3_PEERING | PASS | - |
| 63 | leaf4-DC1 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4094 - MLAG_PEER | PASS | - |
| 64 | leaf4-DC1 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan10 - DMZ | PASS | - |
| 65 | leaf4-DC1 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan3009 - MLAG_PEER_L3_iBGP: vrf VRF_A | PASS | - |
| 66 | leaf1-DC1 | Interface State | Vxlan Interface Status & Line Protocol == "up" | Vxlan1 | PASS | - |
| 67 | leaf2-DC1 | Interface State | Vxlan Interface Status & Line Protocol == "up" | Vxlan1 | PASS | - |
| 68 | leaf3-DC1 | Interface State | Vxlan Interface Status & Line Protocol == "up" | Vxlan1 | PASS | - |
| 69 | leaf4-DC1 | Interface State | Vxlan Interface Status & Line Protocol == "up" | Vxlan1 | PASS | - |
| 70 | leaf1-DC1 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - EVPN_Overlay_Peering | PASS | - |
| 71 | leaf1-DC1 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback1 - VTEP_VXLAN_Tunnel_Source | PASS | - |
| 72 | leaf2-DC1 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - EVPN_Overlay_Peering | PASS | - |
| 73 | leaf2-DC1 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback1 - VTEP_VXLAN_Tunnel_Source | PASS | - |
| 74 | leaf3-DC1 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - EVPN_Overlay_Peering | PASS | - |
| 75 | leaf3-DC1 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback1 - VTEP_VXLAN_Tunnel_Source | PASS | - |
| 76 | leaf4-DC1 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - EVPN_Overlay_Peering | PASS | - |
| 77 | leaf4-DC1 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback1 - VTEP_VXLAN_Tunnel_Source | PASS | - |
| 78 | spine1-DC1 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - EVPN_Overlay_Peering | PASS | - |
| 79 | spine2-DC1 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - EVPN_Overlay_Peering | PASS | - |
| 80 | spine3-DC1 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - EVPN_Overlay_Peering | PASS | - |
| 81 | leaf1-DC1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet1 - remote: leaf2-DC1_Ethernet1 | PASS | - |
| 82 | leaf1-DC1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet2 - remote: leaf2-DC1_Ethernet2 | PASS | - |
| 83 | leaf1-DC1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet3 - remote: spine1-DC1_Ethernet2 | PASS | - |
| 84 | leaf1-DC1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet4 - remote: spine2-DC1_Ethernet2 | PASS | - |
| 85 | leaf1-DC1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet5 - remote: spine3-DC1_Ethernet2 | PASS | - |
| 86 | leaf2-DC1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet1 - remote: leaf1-DC1_Ethernet1 | PASS | - |
| 87 | leaf2-DC1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet2 - remote: leaf1-DC1_Ethernet2 | PASS | - |
| 88 | leaf2-DC1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet3 - remote: spine1-DC1_Ethernet3 | PASS | - |
| 89 | leaf2-DC1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet4 - remote: spine2-DC1_Ethernet3 | PASS | - |
| 90 | leaf2-DC1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet5 - remote: spine3-DC1_Ethernet3 | PASS | - |
| 91 | leaf3-DC1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet1 - remote: leaf4-DC1_Ethernet1 | PASS | - |
| 92 | leaf3-DC1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet2 - remote: leaf4-DC1_Ethernet2 | PASS | - |
| 93 | leaf3-DC1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet3 - remote: spine1-DC1_Ethernet4 | PASS | - |
| 94 | leaf3-DC1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet4 - remote: spine2-DC1_Ethernet4 | PASS | - |
| 95 | leaf3-DC1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet5 - remote: spine3-DC1_Ethernet4 | PASS | - |
| 96 | leaf4-DC1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet1 - remote: leaf3-DC1_Ethernet1 | PASS | - |
| 97 | leaf4-DC1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet2 - remote: leaf3-DC1_Ethernet2 | PASS | - |
| 98 | leaf4-DC1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet3 - remote: spine1-DC1_Ethernet5 | PASS | - |
| 99 | leaf4-DC1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet4 - remote: spine2-DC1_Ethernet5 | PASS | - |
| 100 | leaf4-DC1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet5 - remote: spine3-DC1_Ethernet5 | PASS | - |
| 101 | spine1-DC1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet2 - remote: leaf1-DC1_Ethernet3 | PASS | - |
| 102 | spine1-DC1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet3 - remote: leaf2-DC1_Ethernet3 | PASS | - |
| 103 | spine1-DC1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet4 - remote: leaf3-DC1_Ethernet3 | PASS | - |
| 104 | spine1-DC1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet5 - remote: leaf4-DC1_Ethernet3 | PASS | - |
| 105 | spine2-DC1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet2 - remote: leaf1-DC1_Ethernet4 | PASS | - |
| 106 | spine2-DC1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet3 - remote: leaf2-DC1_Ethernet4 | PASS | - |
| 107 | spine2-DC1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet4 - remote: leaf3-DC1_Ethernet4 | PASS | - |
| 108 | spine2-DC1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet5 - remote: leaf4-DC1_Ethernet4 | PASS | - |
| 109 | spine3-DC1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet2 - remote: leaf1-DC1_Ethernet5 | PASS | - |
| 110 | spine3-DC1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet3 - remote: leaf2-DC1_Ethernet5 | PASS | - |
| 111 | spine3-DC1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet4 - remote: leaf3-DC1_Ethernet5 | PASS | - |
| 112 | spine3-DC1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet5 - remote: leaf4-DC1_Ethernet5 | PASS | - |
| 113 | leaf1-DC1 | MLAG | MLAG State active & Status connected | MLAG | PASS | - |
| 114 | leaf2-DC1 | MLAG | MLAG State active & Status connected | MLAG | PASS | - |
| 115 | leaf3-DC1 | MLAG | MLAG State active & Status connected | MLAG | PASS | - |
| 116 | leaf4-DC1 | MLAG | MLAG State active & Status connected | MLAG | PASS | - |
| 117 | leaf1-DC1 | IP Reachability | ip reachability test p2p links | Source: leaf1-DC1_Ethernet3 - Destination: spine1-DC1_Ethernet2 | FAIL | 100% packet loss |
| 118 | leaf1-DC1 | IP Reachability | ip reachability test p2p links | Source: leaf1-DC1_Ethernet4 - Destination: spine2-DC1_Ethernet2 | FAIL | 100% packet loss |
| 119 | leaf1-DC1 | IP Reachability | ip reachability test p2p links | Source: leaf1-DC1_Ethernet5 - Destination: spine3-DC1_Ethernet2 | FAIL | 100% packet loss |
| 120 | leaf2-DC1 | IP Reachability | ip reachability test p2p links | Source: leaf2-DC1_Ethernet3 - Destination: spine1-DC1_Ethernet3 | FAIL | 100% packet loss |
| 121 | leaf2-DC1 | IP Reachability | ip reachability test p2p links | Source: leaf2-DC1_Ethernet4 - Destination: spine2-DC1_Ethernet3 | FAIL | 100% packet loss |
| 122 | leaf2-DC1 | IP Reachability | ip reachability test p2p links | Source: leaf2-DC1_Ethernet5 - Destination: spine3-DC1_Ethernet3 | FAIL | 100% packet loss |
| 123 | leaf3-DC1 | IP Reachability | ip reachability test p2p links | Source: leaf3-DC1_Ethernet3 - Destination: spine1-DC1_Ethernet4 | FAIL | 100% packet loss |
| 124 | leaf3-DC1 | IP Reachability | ip reachability test p2p links | Source: leaf3-DC1_Ethernet4 - Destination: spine2-DC1_Ethernet4 | FAIL | 100% packet loss |
| 125 | leaf3-DC1 | IP Reachability | ip reachability test p2p links | Source: leaf3-DC1_Ethernet5 - Destination: spine3-DC1_Ethernet4 | FAIL | 100% packet loss |
| 126 | leaf4-DC1 | IP Reachability | ip reachability test p2p links | Source: leaf4-DC1_Ethernet3 - Destination: spine1-DC1_Ethernet5 | FAIL | 100% packet loss |
| 127 | leaf4-DC1 | IP Reachability | ip reachability test p2p links | Source: leaf4-DC1_Ethernet4 - Destination: spine2-DC1_Ethernet5 | FAIL | 100% packet loss |
| 128 | leaf4-DC1 | IP Reachability | ip reachability test p2p links | Source: leaf4-DC1_Ethernet5 - Destination: spine3-DC1_Ethernet5 | FAIL | 100% packet loss |
| 129 | spine1-DC1 | IP Reachability | ip reachability test p2p links | Source: spine1-DC1_Ethernet2 - Destination: leaf1-DC1_Ethernet3 | FAIL | 100% packet loss |
| 130 | spine1-DC1 | IP Reachability | ip reachability test p2p links | Source: spine1-DC1_Ethernet3 - Destination: leaf2-DC1_Ethernet3 | FAIL | 100% packet loss |
| 131 | spine1-DC1 | IP Reachability | ip reachability test p2p links | Source: spine1-DC1_Ethernet4 - Destination: leaf3-DC1_Ethernet3 | FAIL | 100% packet loss |
| 132 | spine1-DC1 | IP Reachability | ip reachability test p2p links | Source: spine1-DC1_Ethernet5 - Destination: leaf4-DC1_Ethernet3 | FAIL | 100% packet loss |
| 133 | spine2-DC1 | IP Reachability | ip reachability test p2p links | Source: spine2-DC1_Ethernet2 - Destination: leaf1-DC1_Ethernet4 | FAIL | 100% packet loss |
| 134 | spine2-DC1 | IP Reachability | ip reachability test p2p links | Source: spine2-DC1_Ethernet3 - Destination: leaf2-DC1_Ethernet4 | FAIL | 100% packet loss |
| 135 | spine2-DC1 | IP Reachability | ip reachability test p2p links | Source: spine2-DC1_Ethernet4 - Destination: leaf3-DC1_Ethernet4 | FAIL | 100% packet loss |
| 136 | spine2-DC1 | IP Reachability | ip reachability test p2p links | Source: spine2-DC1_Ethernet5 - Destination: leaf4-DC1_Ethernet4 | FAIL | 100% packet loss |
| 137 | spine3-DC1 | IP Reachability | ip reachability test p2p links | Source: spine3-DC1_Ethernet2 - Destination: leaf1-DC1_Ethernet5 | FAIL | 100% packet loss |
| 138 | spine3-DC1 | IP Reachability | ip reachability test p2p links | Source: spine3-DC1_Ethernet3 - Destination: leaf2-DC1_Ethernet5 | FAIL | 100% packet loss |
| 139 | spine3-DC1 | IP Reachability | ip reachability test p2p links | Source: spine3-DC1_Ethernet4 - Destination: leaf3-DC1_Ethernet5 | FAIL | 100% packet loss |
| 140 | spine3-DC1 | IP Reachability | ip reachability test p2p links | Source: spine3-DC1_Ethernet5 - Destination: leaf4-DC1_Ethernet5 | FAIL | 100% packet loss |
| 141 | leaf1-DC1 | BGP | ArBGP is configured and operating | ArBGP | PASS | - |
| 142 | leaf2-DC1 | BGP | ArBGP is configured and operating | ArBGP | PASS | - |
| 143 | leaf3-DC1 | BGP | ArBGP is configured and operating | ArBGP | PASS | - |
| 144 | leaf4-DC1 | BGP | ArBGP is configured and operating | ArBGP | PASS | - |
| 145 | spine1-DC1 | BGP | ArBGP is configured and operating | ArBGP | PASS | - |
| 146 | spine2-DC1 | BGP | ArBGP is configured and operating | ArBGP | PASS | - |
| 147 | spine3-DC1 | BGP | ArBGP is configured and operating | ArBGP | PASS | - |
| 148 | leaf1-DC1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.255.251.1 | PASS | - |
| 149 | leaf1-DC1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 192.168.103.0 | PASS | - |
| 150 | leaf1-DC1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 192.168.103.2 | PASS | - |
| 151 | leaf1-DC1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 192.168.103.4 | PASS | - |
| 152 | leaf2-DC1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.255.251.0 | PASS | - |
| 153 | leaf2-DC1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 192.168.103.6 | PASS | - |
| 154 | leaf2-DC1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 192.168.103.8 | PASS | - |
| 155 | leaf2-DC1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 192.168.103.10 | PASS | - |
| 156 | leaf3-DC1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.255.251.5 | PASS | - |
| 157 | leaf3-DC1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 192.168.103.12 | PASS | - |
| 158 | leaf3-DC1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 192.168.103.14 | PASS | - |
| 159 | leaf3-DC1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 192.168.103.16 | PASS | - |
| 160 | leaf4-DC1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.255.251.4 | PASS | - |
| 161 | leaf4-DC1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 192.168.103.18 | PASS | - |
| 162 | leaf4-DC1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 192.168.103.20 | PASS | - |
| 163 | leaf4-DC1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 192.168.103.22 | PASS | - |
| 164 | spine1-DC1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 192.168.103.1 | PASS | - |
| 165 | spine1-DC1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 192.168.103.7 | PASS | - |
| 166 | spine1-DC1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 192.168.103.13 | PASS | - |
| 167 | spine1-DC1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 192.168.103.19 | PASS | - |
| 168 | spine2-DC1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 192.168.103.3 | PASS | - |
| 169 | spine2-DC1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 192.168.103.9 | PASS | - |
| 170 | spine2-DC1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 192.168.103.15 | PASS | - |
| 171 | spine2-DC1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 192.168.103.21 | PASS | - |
| 172 | spine3-DC1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 192.168.103.5 | PASS | - |
| 173 | spine3-DC1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 192.168.103.11 | PASS | - |
| 174 | spine3-DC1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 192.168.103.17 | PASS | - |
| 175 | spine3-DC1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 192.168.103.23 | PASS | - |
| 176 | leaf1-DC1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 192.168.101.11 | PASS | - |
| 177 | leaf1-DC1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 192.168.101.12 | PASS | - |
| 178 | leaf1-DC1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 192.168.101.13 | PASS | - |
| 179 | leaf2-DC1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 192.168.101.11 | PASS | - |
| 180 | leaf2-DC1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 192.168.101.12 | PASS | - |
| 181 | leaf2-DC1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 192.168.101.13 | PASS | - |
| 182 | leaf3-DC1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 192.168.101.11 | PASS | - |
| 183 | leaf3-DC1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 192.168.101.12 | PASS | - |
| 184 | leaf3-DC1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 192.168.101.13 | PASS | - |
| 185 | leaf4-DC1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 192.168.101.11 | PASS | - |
| 186 | leaf4-DC1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 192.168.101.12 | PASS | - |
| 187 | leaf4-DC1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 192.168.101.13 | PASS | - |
| 188 | spine1-DC1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 192.168.101.1 | PASS | - |
| 189 | spine1-DC1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 192.168.101.2 | PASS | - |
| 190 | spine1-DC1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 192.168.101.3 | PASS | - |
| 191 | spine1-DC1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 192.168.101.4 | PASS | - |
| 192 | spine2-DC1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 192.168.101.1 | PASS | - |
| 193 | spine2-DC1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 192.168.101.2 | PASS | - |
| 194 | spine2-DC1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 192.168.101.3 | PASS | - |
| 195 | spine2-DC1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 192.168.101.4 | PASS | - |
| 196 | spine3-DC1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 192.168.101.1 | PASS | - |
| 197 | spine3-DC1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 192.168.101.2 | PASS | - |
| 198 | spine3-DC1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 192.168.101.3 | PASS | - |
| 199 | spine3-DC1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 192.168.101.4 | PASS | - |
| 200 | leaf1-DC1 | Routing Table | Remote VTEP address | 192.168.102.1 | PASS | - |
| 201 | leaf1-DC1 | Routing Table | Remote VTEP address | 192.168.102.3 | PASS | - |
| 202 | leaf2-DC1 | Routing Table | Remote VTEP address | 192.168.102.1 | PASS | - |
| 203 | leaf2-DC1 | Routing Table | Remote VTEP address | 192.168.102.3 | PASS | - |
| 204 | leaf3-DC1 | Routing Table | Remote VTEP address | 192.168.102.1 | PASS | - |
| 205 | leaf3-DC1 | Routing Table | Remote VTEP address | 192.168.102.3 | PASS | - |
| 206 | leaf4-DC1 | Routing Table | Remote VTEP address | 192.168.102.1 | PASS | - |
| 207 | leaf4-DC1 | Routing Table | Remote VTEP address | 192.168.102.3 | PASS | - |
| 208 | leaf1-DC1 | Routing Table | Remote Lo0 address | 192.168.101.1 | PASS | - |
| 209 | leaf1-DC1 | Routing Table | Remote Lo0 address | 192.168.101.2 | PASS | - |
| 210 | leaf1-DC1 | Routing Table | Remote Lo0 address | 192.168.101.3 | PASS | - |
| 211 | leaf1-DC1 | Routing Table | Remote Lo0 address | 192.168.101.4 | PASS | - |
| 212 | leaf1-DC1 | Routing Table | Remote Lo0 address | 192.168.101.11 | PASS | - |
| 213 | leaf1-DC1 | Routing Table | Remote Lo0 address | 192.168.101.12 | PASS | - |
| 214 | leaf1-DC1 | Routing Table | Remote Lo0 address | 192.168.101.13 | PASS | - |
| 215 | leaf2-DC1 | Routing Table | Remote Lo0 address | 192.168.101.1 | PASS | - |
| 216 | leaf2-DC1 | Routing Table | Remote Lo0 address | 192.168.101.2 | PASS | - |
| 217 | leaf2-DC1 | Routing Table | Remote Lo0 address | 192.168.101.3 | PASS | - |
| 218 | leaf2-DC1 | Routing Table | Remote Lo0 address | 192.168.101.4 | PASS | - |
| 219 | leaf2-DC1 | Routing Table | Remote Lo0 address | 192.168.101.11 | PASS | - |
| 220 | leaf2-DC1 | Routing Table | Remote Lo0 address | 192.168.101.12 | PASS | - |
| 221 | leaf2-DC1 | Routing Table | Remote Lo0 address | 192.168.101.13 | PASS | - |
| 222 | leaf3-DC1 | Routing Table | Remote Lo0 address | 192.168.101.1 | PASS | - |
| 223 | leaf3-DC1 | Routing Table | Remote Lo0 address | 192.168.101.2 | PASS | - |
| 224 | leaf3-DC1 | Routing Table | Remote Lo0 address | 192.168.101.3 | PASS | - |
| 225 | leaf3-DC1 | Routing Table | Remote Lo0 address | 192.168.101.4 | PASS | - |
| 226 | leaf3-DC1 | Routing Table | Remote Lo0 address | 192.168.101.11 | PASS | - |
| 227 | leaf3-DC1 | Routing Table | Remote Lo0 address | 192.168.101.12 | PASS | - |
| 228 | leaf3-DC1 | Routing Table | Remote Lo0 address | 192.168.101.13 | PASS | - |
| 229 | leaf4-DC1 | Routing Table | Remote Lo0 address | 192.168.101.1 | PASS | - |
| 230 | leaf4-DC1 | Routing Table | Remote Lo0 address | 192.168.101.2 | PASS | - |
| 231 | leaf4-DC1 | Routing Table | Remote Lo0 address | 192.168.101.3 | PASS | - |
| 232 | leaf4-DC1 | Routing Table | Remote Lo0 address | 192.168.101.4 | PASS | - |
| 233 | leaf4-DC1 | Routing Table | Remote Lo0 address | 192.168.101.11 | PASS | - |
| 234 | leaf4-DC1 | Routing Table | Remote Lo0 address | 192.168.101.12 | PASS | - |
| 235 | leaf4-DC1 | Routing Table | Remote Lo0 address | 192.168.101.13 | PASS | - |
| 236 | leaf1-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf1-DC1 - 192.168.101.1 Destination: 192.168.101.1 | FAIL | 100% packet loss |
| 237 | leaf1-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf1-DC1 - 192.168.101.1 Destination: 192.168.101.2 | FAIL | 100% packet loss |
| 238 | leaf1-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf1-DC1 - 192.168.101.1 Destination: 192.168.101.3 | FAIL | 100% packet loss |
| 239 | leaf1-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf1-DC1 - 192.168.101.1 Destination: 192.168.101.4 | FAIL | 100% packet loss |
| 240 | leaf1-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf1-DC1 - 192.168.101.1 Destination: 192.168.101.11 | FAIL | 100% packet loss |
| 241 | leaf1-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf1-DC1 - 192.168.101.1 Destination: 192.168.101.12 | FAIL | 100% packet loss |
| 242 | leaf1-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf1-DC1 - 192.168.101.1 Destination: 192.168.101.13 | FAIL | 100% packet loss |
| 243 | leaf2-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf2-DC1 - 192.168.101.2 Destination: 192.168.101.1 | FAIL | 100% packet loss |
| 244 | leaf2-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf2-DC1 - 192.168.101.2 Destination: 192.168.101.2 | FAIL | 100% packet loss |
| 245 | leaf2-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf2-DC1 - 192.168.101.2 Destination: 192.168.101.3 | FAIL | 100% packet loss |
| 246 | leaf2-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf2-DC1 - 192.168.101.2 Destination: 192.168.101.4 | FAIL | 100% packet loss |
| 247 | leaf2-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf2-DC1 - 192.168.101.2 Destination: 192.168.101.11 | FAIL | 100% packet loss |
| 248 | leaf2-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf2-DC1 - 192.168.101.2 Destination: 192.168.101.12 | FAIL | 100% packet loss |
| 249 | leaf2-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf2-DC1 - 192.168.101.2 Destination: 192.168.101.13 | FAIL | 100% packet loss |
| 250 | leaf3-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf3-DC1 - 192.168.101.3 Destination: 192.168.101.1 | FAIL | 100% packet loss |
| 251 | leaf3-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf3-DC1 - 192.168.101.3 Destination: 192.168.101.2 | FAIL | 100% packet loss |
| 252 | leaf3-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf3-DC1 - 192.168.101.3 Destination: 192.168.101.3 | FAIL | 100% packet loss |
| 253 | leaf3-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf3-DC1 - 192.168.101.3 Destination: 192.168.101.4 | FAIL | 100% packet loss |
| 254 | leaf3-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf3-DC1 - 192.168.101.3 Destination: 192.168.101.11 | FAIL | 100% packet loss |
| 255 | leaf3-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf3-DC1 - 192.168.101.3 Destination: 192.168.101.12 | FAIL | 100% packet loss |
| 256 | leaf3-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf3-DC1 - 192.168.101.3 Destination: 192.168.101.13 | FAIL | 100% packet loss |
| 257 | leaf4-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf4-DC1 - 192.168.101.4 Destination: 192.168.101.1 | FAIL | 100% packet loss |
| 258 | leaf4-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf4-DC1 - 192.168.101.4 Destination: 192.168.101.2 | FAIL | 100% packet loss |
| 259 | leaf4-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf4-DC1 - 192.168.101.4 Destination: 192.168.101.3 | FAIL | 100% packet loss |
| 260 | leaf4-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf4-DC1 - 192.168.101.4 Destination: 192.168.101.4 | FAIL | 100% packet loss |
| 261 | leaf4-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf4-DC1 - 192.168.101.4 Destination: 192.168.101.11 | FAIL | 100% packet loss |
| 262 | leaf4-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf4-DC1 - 192.168.101.4 Destination: 192.168.101.12 | FAIL | 100% packet loss |
| 263 | leaf4-DC1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf4-DC1 - 192.168.101.4 Destination: 192.168.101.13 | FAIL | 100% packet loss |