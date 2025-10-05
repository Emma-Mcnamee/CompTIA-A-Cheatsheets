# VLANs & VPNs

## LANs (Local Area Network)
- A group of devices in the same **broadcast domain**.  
- A broadcast domain refers to the devices able to see a broadcast on a certain network/switch.  
- Some switches may have many interfaces but not many devices — this is fine for security but not efficient use of a switch.  
- **VLANs (Virtual Local Area Networks)** allow you to split interfaces into different broadcast domains while still using the same switch efficiently.  

---

## VLANs (Virtual Local Area Network)
- VLANs keep certain interfaces on one broadcast domain and others on another.  
- This maintains **security**, improves **organization**, and makes full use of the switch.  
- A switch separates VLANs, but different VLANs **cannot communicate directly**.  
- A **router** (or Layer 3 switch) is needed to route data between VLANs.  
- Common setup: VLAN 10 (Accounting), VLAN 20 (Sales), VLAN 30 (Guests).  

**Key Points**
- Each VLAN = separate broadcast domain.  
- VLANs improve performance, scalability, and security.  
- VLANs are configured at the switch level.  

---

## VPNs (Virtual Private Networks)
- A **VPN** allows encrypted data to traverse a **public network** securely.  
- Commonly implemented as **hardware**, but there are also **software-based** VPNs.  
- Sometimes VPN functionality is **built into an OS** for client devices.  

### VPN Concentrator
- Handles **encryption/decryption** and **authentication** for VPN connections.  
- Often integrated into **firewalls**.  
- Used in both client-based and site-based VPN setups.  

---

## Types of VPNs

### Client-to-Site VPN
- Used for **on-demand access** from a remote device (ex: work from home).  
- VPN software on the remote device connects to the concentrator.  
- Encrypts and decrypts traffic between the client and network.  

### Site-to-Site VPN
- Used for **permanent or nearly permanent** connections between sites.  
- Example: Corporate HQ ↔ Branch office.  
- Each site has a **VPN concentrator, router, or firewall**.  
- Provides secure encrypted communication between networks.  

---

## Summary
| Concept | Function | Hardware | Use Case |
|----------|-----------|-----------|-----------|
| VLAN | Segments a LAN into logical groups | Switch (Layer 2/3) | Separate network traffic by department or purpose |
| VPN | Encrypts traffic across public networks | Firewall / Router / Software | Secure remote or inter-site connections |
| Client-to-Site | Remote user access | VPN client + concentrator | Work-from-home or mobile users |
| Site-to-Site | Connects two networks | Routers / Firewalls | Connect branch offices securely |
