# 🧭 Ports & Protocols

---

## 🔹 Intro to IP

- **Internet Protocol (IP)** controls how data travels across networks — think of it like trucks carrying boxes.  
- Data is transferred using **TCP** or **UDP**.  
- Inside those are the layers of the **OSI model** (this process is called **encapsulation**).  
- **Payload** = actual data being transferred.  
- Packets contain:
  - **Header** – routing info  
  - **Payload** – data  
  - **Trailer** – error checking info  
- **Ethernet frames** can contain multiple layers, depending on the protocol.  
- **Encapsulation**: Data is *transported in IP* (wrapped inside IP protocol).  

---

## 🔹 TCP vs UDP (Transport Layer - Layer 4)

| Feature | TCP | UDP |
|----------|-----|-----|
| Type | Connection-oriented | Connectionless |
| Reliability | Reliable, error detection, uses ACK | Unreliable, no guarantee |
| Speed | Slower | Faster |
| Use Cases | Web, SSH, email | Streaming, gaming, VoIP |
| Example Protocols | HTTPS, SSH | DHCP, TFTP |

> TCP = Reliability  
> UDP = Speed

---

## 🔹 Connection-Oriented Communication (TCP)

- Protocols like **HTTPS** and **SSH** use TCP for reliability.  
- TCP uses **ACK (acknowledgment)** to confirm data was received.  
- These protocols handle **error checking internally**, not the app.  

---

## 🔹 Ports Overview

- **IP Address** = “Home address” of a device.  
- **Port Number** = The *specific room or service* inside the house.  
- Ports + IP + Protocol identify exactly *where* data is going.  

### Port Types
- **Non-ephemeral ports**: Permanent / fixed.  
- **Ephemeral ports**: Temporary, usually used by clients.  
- ⚠️ Ports are for *communication*, **not security**.

---

## 🔹 Common Ports & Protocols

| Protocol | Port(s) | Transport | Description |
|-----------|----------|------------|--------------|
| **FTP** | 20 (data), 21 (control) | TCP | File Transfer Protocol — transfers files between systems. Authenticates with username/password. |
| **SSH** | 22 | TCP | Secure Shell — encrypted remote login (not in the clear). |
| **Telnet** | 23 | TCP | Remote login protocol (unencrypted). |
| **SMTP** | 25 | TCP | Simple Mail Transfer Protocol — sends mail between servers. |
| **DNS** | 53 | UDP | Domain Name System — converts names to IP addresses. |
| **DHCP** | 67, 68 | UDP | Dynamic Host Configuration Protocol — auto assigns IPs, gateways, masks. |
| **HTTP** | 80 | TCP | Web browsing (unencrypted). |
| **HTTPS** | 443 | TCP | Secure web browsing (encrypted). |
| **POP3** | 110 | TCP | Post Office Protocol v3 — retrieves emails. |
| **IMAP4** | 143 | TCP | Internet Message Access Protocol — retrieves and syncs emails. |
| **SMB** | 445 | TCP | Server Message Block — file sharing on Windows. |
| **LDAP** | 389 | TCP | Lightweight Directory Access Protocol — access directory info. |
| **LDAPS** | 636 | TCP | Secure version of LDAP. |
| **RDP** | 3389 | TCP | Remote Desktop Protocol — remote control of desktops. |

---

## 🔹 Quick Notes

- **Connectionless protocols** (like UDP, DHCP, TFTP) don’t verify delivery — it’s up to the *application* to handle errors.  
- **Connection-oriented protocols** (like TCP, HTTPS, SSH) verify delivery automatically.  
- Ports are **identifiers**, not **security mechanisms**.  
