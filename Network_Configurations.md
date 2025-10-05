# 🌐 Network Configurations

---

## 🔹 Overview

Network configurations define how devices communicate and are identified on a network.  
Two of the most critical services for configuration and connectivity are **DNS (Domain Name System)** and **DHCP (Dynamic Host Configuration Protocol)**.

---

## 🧭 DNS (Domain Name System)

DNS translates **domain names** (like `www.google.com`) into **IP addresses** and vice versa.  
It uses a **hierarchical system** that organizes all domain names across the internet.

> 🧠 Think of DNS as the “phonebook” of the internet — mapping names to numbers.

---

### 🔍 DNS Lookup

To view DNS records, use:

- **Linux/macOS:** `dig`
- **Windows:** `nslookup`

These commands query DNS servers and return information about domains, IPs, and record types.

---

### 📘 DNS Records

DNS **resource records (RRs)** store essential data such as IPs, mail servers, certificates, and aliases.  
There are over **30 record types**, but the most common include:

| Record Type | Description | Example |
|--------------|--------------|----------|
| **A** | Maps a domain to an **IPv4 address** | `example.com → 192.168.1.10` |
| **AAAA** | Maps a domain to an **IPv6 address** | `example.com → 2606:4700:4700::1111` |
| **CNAME** | Canonical name record. Used to alias one domain to another. | `shop.example.com → www.example.com` |
| **MX** | Mail Exchange record. Points to a domain’s mail server. | `example.com → mail.example.com` |
| **TXT** | Contains human-readable or verification data. | SPF, DKIM, DMARC info |

---

### 🔒 Common DNS Security / Verification Records

#### 🧩 DKIM (DomainKeys Identified Mail)
- Digitally signs a domain’s **outgoing email**.
- Receiving mail servers validate the signature using a **public key** stored as a **TXT record** in DNS.

#### 🧾 SPF (Sender Policy Framework)
- Lists **authorized mail servers** for a domain.
- Helps prevent **email spoofing** by rejecting mail from unauthorized servers.

#### 📊 DMARC (Domain-based Message Authentication, Reporting, and Conformance)
- Builds on **SPF** and **DKIM**.
- Defines how to **handle unverified emails** (reject, quarantine, or allow).
- Stored as a **TXT record** specifying policy details.

> 🔐 Example: `v=DMARC1; p=reject; rua=mailto:dmarc-reports@example.com`

---

## ⚙️ DHCP (Dynamic Host Configuration Protocol)

Introduced in **1997**, DHCP automates the process of assigning IP addresses and network parameters to devices.  
Before DHCP, every IP address had to be configured manually — which was not scalable.

> 📡 DHCP makes network setup **hands-free** and **error-free**.

---

### 🧩 What DHCP Configures

- IP Address  
- Subnet Mask  
- Default Gateway  
- DNS Server  
- NTP Server  
- VoIP Server (optional)

---

### 🔁 DHCP Lease Process (DORA)

DHCP uses a **4-step handshake** to assign an IP address automatically:

| Step | Action | Description |
|------|---------|-------------|
| **Discover** | Client → Broadcast | Device searches for available DHCP servers. |
| **Offer** | Server → Client | Server offers an available IP address. |
| **Request** | Client → Server | Client requests to lease the offered IP. |
| **Acknowledge** | Server → Client | Server confirms and leases the IP to the client. |

> ⏱️ Once acknowledged, the IP is reserved for that client until the lease expires or is renewed.

---

### 📦 DHCP Scopes

A **scope** is a predefined range of IP addresses a DHCP server can assign.  
Each scope includes:

- IP address range  
- Subnet mask  
- Lease duration  
- Default gateway  
- DNS and NTP servers  

> 🔠 Each subnet usually has its own scope.

---

### 🗂️ DHCP Pools

A **pool** is a group of addresses within a scope.  
Pools organize available IP addresses
