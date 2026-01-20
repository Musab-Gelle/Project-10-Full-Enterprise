# Project-10-Full-Enterprise
This is a realistic **enterprise network simulation** built in Cisco Packet Tracer.   It integrates multiple networking concepts learned across previous projects into a single fully functioning network:


-VLANs for HR, IT, Finance, and Branch
- Inter-VLAN routing on HQ router
- Centralized DHCP with relay for Branch
- OSPF dynamic routing between HQ and Branch
- ACLs enforcing access control between departments
- NAT for Internet connectivity
- Port security on all access ports
- DHCP/DNS server for network services

  
---

## IP Addressing & VLANs

| VLAN/Network | Devices       | Subnet            |
|--------------|---------------|-----------------|
| VLAN 10      | HR PCs        | 192.168.10.0/24 |
| VLAN 20      | IT PCs        | 192.168.20.0/24 |
| VLAN 30      | Finance PCs   | 192.168.30.0/24 |
| VLAN 40      | Branch PCs    | 192.168.40.0/24 |
| WAN          | HQ ↔ Branch   | 10.0.0.0/24     |
| NAT/Internet | ISP/HQ        | 203.0.113.0/24  |

---

## Key Configurations

- **VLANs & Inter-VLAN routing** on HQ router
- **DHCP & DHCP relay** for centralised IP assignment
- **OSPF** for dynamic routing between HQ & Branch
- **ACLs**: HR cannot reach IT; other rules applied per network security
- **NAT** on HQ router for Internet access
- **Switch port security** on all access ports (sticky MAC, single device, shutdown on violation)

---

## Verification

1. PCs receive IP addresses via DHCP (HR/IT/Finance/Branch)
2. Branch PC can reach HQ PCs and Internet
3. ACLs block/allow traffic as expected
4. OSPF neighbors are established:
5. NAT works:
6. Port security prevents rogue devices

---

## Skills Demonstrated

- Enterprise VLAN and subnet design
- Inter-VLAN routing configuration
- Centralized DHCP and relay
- Dynamic routing with OSPF
- ACL-based security and traffic control
- NAT for Internet access
- Switch port security and access control
- Realistic troubleshooting scenarios

---

## Tools Used

- Cisco Packet Tracer
- Cisco IOS CLI
