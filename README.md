# IP Network Design Infrastructure (Cisco Packet Tracer)

### Project Overview
This project involves designing and configuring a network for ABC Research Company using Cisco Packet Tracer. The network is designed according to the provided topology and includes multiple departments with varying network requirements. Key tasks include IP addressing with VLSM, dynamic and static routing, VLAN configuration, and NAT implementation.

![topology](https://github.com/user-attachments/assets/2c26c3ee-70bb-4418-a5cd-a426771d2506)

### Network Configuration Details

#### 1. **IP Configuration Using VLSM**
   - Assigned IP configurations for the entire network using Variable Length Subnet Masking (VLSM).
   - Ensured optimal IP address allocation starting from networks with the maximum number of hosts.
   - Built and documented a comprehensive IP allocation table for all departments.

#### 2. **Dynamic Routing with RIPv2**
   - Configured RIPv2 as the dynamic routing protocol on all routers, unless specified otherwise.
   - Device names and router configurations align with the network topology diagram.
   - Implemented console line passwords as per security standards.

#### 3. **DHCP Configuration**
   - **DEPT-1**: Configured the department's router as a DHCP server to dynamically allocate IP addresses to 512 hosts. The switch in this department operates as a transparent device, with all hosts belonging to a single VLAN.

#### 4. **Advanced Routing Configuration**
   - **DEPT-2**: Connected to both DEPT-1 and CAMPUS routers. Configured for both RIPv2 and OSPF routing protocols, with OSPF routes redistributed to DEPT-1.
   - Configured inter-VLAN routing using 802.1q encapsulation on sub-interfaces, enabling connectivity between VLANs 10, 20, and 30.

#### 5. **VLAN Configuration**
   - **DEPT-2**: Configured switches to accommodate three VLANs (VLAN 10, 20, 30) along with a management VLAN. Implemented trunking on Fast Ethernet 0/0 to carry traffic for all VLANs.

#### 6. **NAT and ISP Configuration**
   - **CAMPUS Router**: Configured as the exit point for internal traffic to the external network via the ISP router. Implemented a static route (quad zero) to route traffic to the ISP (200.150.100.2/30).
   - Configured NAT (Network Address Translation) to translate incoming traffic to a single private IP address (197.77.111.1), using NAT overload for efficient IP management.

#### 7. **ISP Configuration**
   - Configured the ISP router to connect seamlessly with the rest of the network, ensuring proper routing and interface configurations.

### Project Deliverables
- **Packet Tracer File**: The .pkt file containing the entire network configuration.
- **Documentation**: A PDF or Word file with snapshots of routing tables (`show IP route`), interface summaries (`show IP interface brief`), and the running configuration for all routers.


### Tools Used
- **Cisco Packet Tracer**: For network simulation and configuration.
- **Text Editor**: For documenting the network configuration and snapshots.
