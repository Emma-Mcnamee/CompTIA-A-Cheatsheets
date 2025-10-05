# Network Devices

## Overview
Network devices form the backbone of any network infrastructure.  
Each has distinct roles and capabilities — though many modern devices combine multiple functions (e.g., wireless router + switch + firewall).

---

## Routers
- **Purpose:** Routes traffic between **IP subnets**.  
- Operates primarily at **Layer 3 (Network Layer)**.  
- Connects diverse network types such as **LAN**, **WAN**, **Copper**, and **Fiber**.  
- **Layer 3 Switches** are switches with built-in routing functionality.  
- Can also perform **NAT**, **firewalling**, and **VPN** tasks in enterprise setups.

---

## Switches
- **Purpose:** Forwards traffic within a LAN based on **MAC (Data Link) addresses**.  
- Operates at **Layer 2 (Data Link Layer)**.  
- Provides **wired access** to the network; commonly features **multiple ports**.  
- May support **Power over Ethernet (PoE)** to power devices through network cables.  
- **Multilayer switches** can also perform routing functions.

### Unmanaged Switches
- No configuration or management interface.  
- No VLAN support or traffic control.  
- Simple, inexpensive, plug-and-play option.  

### Managed Switches
- Support **VLANs** and **802.1Q trunking**.  
- Offer **traffic prioritization**, **redundancy**, and **monitoring**.  
- Support **port mirroring** (used to duplicate traffic for protocol analysis).  
- Enable fine-tuned control and integration in enterprise environments.

---

## Access Points (APs)
- Extend a **wired network** into a **wireless network**.  
- **Not a router** — acts as a bridge between wired and wireless segments.  
- Makes forwarding decisions using **MAC addresses**.  
- Typically operates at **Layer 2**.  

---

## Cable Infrastructure

### Patch Panels
- Combination of **punchdown** blocks and **RJ45 connectors**.  
- Provide organized, centralized connection points for network cables.  

---

## Firewalls
- Filter traffic based on **port numbers**, **protocols**, or **applications**.  
- Operate at **OSI Layer 4 (Transport)** or higher (some at Layer 7).  
- Can act as:
  - **VPN concentrators** (for encrypted traffic)
  - **Proxies** (to inspect or filter content)
- Often integrated into **routers** or **UTM appliances**.  
- Essential for **network security and segmentation**.  

---

## Power over Ethernet (PoE)
- Provides **electrical power** and **network connectivity** through a single Ethernet cable.  
- Useful for powering **access points, cameras, VoIP phones**, etc.  

| Specification | Power Output | Max Current | Typical Use |
|----------------|---------------|---------------|--------------|
| PoE (Type 1) | 15.4W DC | 350mA | Small devices |
| PoE+ (Type 2) | 25.5W DC | 600mA | Medium devices |
| PoE++ (Type 3) | 51W DC | 600mA | Larger APs, cameras |
| PoE++ (Type 4) | 71.3W DC | 960mA | High-power devices |

- **Injector:** Adds PoE capability to non-PoE switches.  
- Always confirm your switch supports the power level required by your devices.  

---

## Modems

### Cable Modem
- Provides **broadband** connectivity via **coaxial cable**.  
- Uses the **DOCSIS (Data Over Cable Service Interface Specification)** standard.  
- Common in residential and enterprise high-speed networks.  

### DSL Modem
- Uses **telephone lines** to deliver digital internet (DSL).  
- Can share the same wiring as landline voice service.  

### ONT (Optical Network Terminal)
- Connects **fiber optic** service from the ISP to a **copper** network inside the building.  
- Typically housed in a **terminal box** on the premises.  

---

## Network Interface Card (NIC)
- A hardware component that enables network connectivity for a device.  
- May be **integrated** or **add-on** via PCIe or USB.  
- Contains the device’s **MAC address**.  
- Provides **Ethernet**, **Fiber**, or **Wireless** connectivity options.  
- Allows extended networking capabilities (e.g., multiple interfaces per host).  

---

## Summary

| Device | OSI Layer | Primary Function | Key Features |
|--------|------------|------------------|---------------|
| Router | 3 | Routes traffic between subnets | Connects LAN/WAN, NAT, VPN |
| Switch | 2 | Forwards traffic within LAN | VLANs, PoE, redundancy |
| Access Point | 2 | Extends wired to wireless | Wireless bridging |
| Firewall | 4-7 | Filters and secures traffic | Application filtering, VPN |
| PoE Injector | 1-2 | Adds power over Ethernet | Powers devices via cable |
| Modem | 1 | Converts signals for internet | Cable, DSL, Fiber |
| NIC | 1-2 | Enables network connectivity | MAC address, multiple ports |

---

**Pro Tip:**  
In enterprise setups, devices are often **hybrid** (e.g., a router with built-in firewall and VPN concentrator).  
Understanding each function separately helps troubleshoot complex environments more effectively.
