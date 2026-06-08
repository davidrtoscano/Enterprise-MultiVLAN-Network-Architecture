# Enterprise Multi-VLAN Architecture with Automated Network Services

## Project Overview
Designed and deployed a scalable. segmented Local Area Network (LAN) using a Router-on-a-Stick (RoaS) architecture within Cisco Packet Tracer. This configuration ensures strict departmental isolation for corporate security whil seamlessly enabling required inter-departmental communication and centralized network services.

## Key Techincal Implementations
** VLAN Segmentation & Trunking: Built distinct broadcast domains for HR (VLAN 10), Sales (VLAN 20), and IT (VLAN 30). Implemented an IEEE 802.1Q trunk link between the core switch and router to handle tagged traffic.
** Inter-VLAN Routing: Configured logical suninterfaces on a Cisco router interface to route line-rate traffic smoothly between different subnets.
** Dynamic IP Allocation (DHCP): Developedlocalized Cisco IOS DHCP scopes for each unique department. Designed custom exclusion boundaries to reserve static pools for critical infrastructure.
** Core Infrastructure Services (DNS): Integrated a static corporate server infrastructure running a local DNS daemon, allowing hosts across all VLANs to dynamically resolve standard domain names ('company.local') over the routed network.

## Troubleshooting & Engineering Insights
** Self-Managed ARP Resolution: Successfully troubleshot initial dynamic packet drops caused by standard layer-2 ARP/STP convergance delays, verifying end-to-end stability through iterative ICMP diagnostic testing.
** CLI Scope Alignment: Resolved initial DHCP nesting and interface configuration challenges by meticulousy auditing Cisco IOS command hierarchies and sub-menu contexts.
