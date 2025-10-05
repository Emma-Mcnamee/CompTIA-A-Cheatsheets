# Network Configurations

## Overview
Network configurations define how devices communicate within and beyond local networks.  
The main components involve **IP addressing**, **subnetting**, and **gateway configuration** — using either **IPv4** or **IPv6**.

---

## IPv4 and IPv6

### IPv4
- **Internet Protocol Version 4 (IPv4)** operates at **OSI Layer 3 (Network Layer)**.  
- An IPv4 address consists of **4 octets (32 bits total)**.  
  - **8 bits = 1 byte = 1 octet**  
  - Example: `192.168.1.1`
- There are **4.29 billion** total IPv4 addresses available — not enough for modern demand.  
- To compensate, **private IP ranges** were introduced, and **NAT (Network Address Translation)** allows private devices to access public networks.

#### Public vs. Private IPv4 Addresses
| Type | Description | Can Connect To | Example Ranges |
|-------|--------------|----------------|----------------|
| **Public** | Globally unique; routable on the internet | Other public IPs | Assigned by ISPs |
| **Private** | Used within LANs; not routable on the internet | Other private IPs | 10.0.0.0/8, 172.16.0.0/12, 192.168.0.0/16 |

**NAT** translates between private and public IPs, keeping internal addresses hidden and reusable.

---

### IPv6
- Introduced to solve IPv4 exhaustion with a **128-bit address size**.  
- Supports **vastly more** unique addresses — roughly `3.4 x 10^38`.  
- Written in **hexadecimal**, divided into **8 groups** of **16 bits (two octets per group)**.  
  - Example: `2001:0db8:85a3:0000:0000:8a2e:0370:7334`
- The **first half** typically defines the **network/subnet**, and the **second half** defines the **host**.  

| Comparison | IPv4 | IPv6 |
|-------------|------|------|
| Address Length | 32-bit | 128-bit |
| Format | Decimal (4 octets) | Hexadecimal (8 groups) |
| Example | `192.168.1.1` | `2001:db8::7334` |
| NAT Required | Yes | No (each device gets a unique global address) |
| Built-in Security | No | IPsec mandatory |

---

## Assigning IP Addresses

### Networking with IPv4
Every device on a network requires:
- **IP Address** — Unique identifier within the subnet  
- **Subnet Mask** — Determines which portion of the IP represents the network  
- **Default Gateway** — IP of the router that allows communication outside the local network  

Example configuration:
IP Address: 192.168.1.10
Subnet Mask: 255.255.255.0
Default Gateway: 192.168.1.1
DNS Server: 8.8.8.8

---

## Static vs Dynamic Addressing

### Static IP Addressing
- Manually configured, does **not change** unless modified.  
- Ideal for servers, printers, or network devices that require consistent addressing.  
- Instead of manually assigning, best practice is to configure a **DHCP reservation** via the DNS/DHCP server.

### Dynamic IP Addressing
- Automatically assigned by **DHCP (Dynamic Host Configuration Protocol)**.  
- Easier for managing large networks.  
- IPs can change over time or when devices reconnect.

---

## Automatic Private IP Addressing (APIPA)
- Used when **DHCP is unavailable** and no static IP is set.  
- Automatically assigns an address in the **169.254.x.x** range.  
- Allows local subnet communication **only** (no routing through gateways).  
- Useful for basic local connectivity and troubleshooting DHCP issues.

---

## Turning Dynamic into Static
You can convert a dynamically assigned IP into a static one by:
1. **Disabling DHCP** on the device and manually setting IP information, **or**
2. **Creating a DHCP reservation** on the server so the same IP is always leased to that device.

---

## Quick Reference

| Configuration Term | Description | Example |
|--------------------|-------------|----------|
| **IP Address** | Unique identifier of a device on the network | `192.168.1.10` |
| **Subnet Mask** | Defines the size of the network | `255.255.255.0` |
| **Default Gateway** | Routes traffic outside the local network | `192.168.1.1` |
| **DNS Server** | Resolves domain names to IPs | `8.8.8.8` |
| **APIPA Range** | Self-assigned local IP | `169.254.0.0/16` |

---

**Pro Tip:**  
Use **IPv6** awareness and configuration in your labs — most enterprises are transitioning to dual-stack (IPv4 + IPv6) environments for scalability and compatibility.
