# Troubleshooting Networks

## Network Connectivity
- **Check physical connections:** is the cable plugged in?  
  - A **link light** indicates a good connection.  
- **Ping tests:**
  - `127.0.0.1` (loopback) — verifies the local TCP/IP stack is functioning.  
  - Local IP address — tests local configuration, adapter, and link signal.  
  - Default gateway — confirms connectivity to the local network.  
  - External address (e.g., `8.8.8.8`) — verifies connection beyond the router.  

---

## Intermittent Wireless Connectivity
- **Interference:** other devices may be using the same frequency (e.g., microwaves, cordless phones).  
- **Signal strength:** check the antenna placement and obstructions.  
- **Incorrect channel:** usually set to automatic; verify or manually adjust if necessary.  
- **Multipath interference:** signal reflections from flat surfaces can cause bounce and latency.  
- **Access point issues:** consider replacing or relocating the AP.  

---

## Slow Network Speed
- Not always the network! Verify before assuming.  
- Run **ping or speed tests** to confirm end-to-end connectivity.  
- Evaluate **network hops** for:
  - High utilization  
  - Errors or packet loss  
  - Throughput issues  
  - Filtering, ACLs, or firewall restrictions  
- May require a **packet capture** for deep analysis.  

---

## Limited or No Connectivity
- Windows system tray alerts:  
  - “Limited or no connectivity”  
  - “No internet access”  
- Check **local IP configuration:**  
  - If address begins with `169.254.x.x`, it’s **APIPA** — only local connectivity.  
  - Confirm you have a **DHCP-assigned IP** for full network access.  
- Perform ping tests to:
  - Local gateway  
  - Remote IP address  

---

## Jitter
- Real-time media (voice, video) is **sensitive to delay.**  
- Jitter = variation in **packet arrival time.**  
- Excessive jitter causes **choppy audio** or **video dropouts.**  
- Measure jitter using network monitoring tools to identify inconsistencies.  

---

## Poor VoIP Quality
- VoIP requires **high speed** and **low latency.**  
- Check **internet connection** with a speed test.  
- Inspect **local networking equipment:**  
  - Old or underpowered routers/switches can cause performance issues.  
  - Replace outdated hardware if necessary.  

---

## Port Flapping
- **Link light turns on/off repeatedly.**  
- Often caused by:
  - Faulty or damaged cable → **replace cable.**  
  - Failing switch port → **move to a different interface.**  
- If the problem persists, **run new cabling** across the full path.  

---

## High Latency
- **Delay between request and response.**  
- Some latency is expected, but excessive delay affects performance.  
- Use **ping and traceroute** to identify where latency occurs.  
- **Packet captures** provide detailed timing and response analysis.  

---

## External Interference
- **Predictable sources:** fluorescent lights, microwaves, cordless phones.  
- **Unpredictable sources:** multi-tenant buildings, overlapping Wi-Fi networks.  
- Use **Signal-to-Noise Ratio (SNR)** measurements to monitor performance.  

### Signal-to-Noise Ratio (SNR)
- **Signal:** the desired network transmission.  
- **Noise:** interference and unwanted signals.  
- Higher SNR = better performance.  
  - Aim for a **large ratio** (strong signal, minimal noise).  

---

## Authentication Issues
- **Access denied** or **login failure** to network resources.  
- Verify:
  - Active session or credentials — may need to reauthenticate.  
  - User permissions and group policies.  
- **Packet captures** can reveal failed authentication attempts or protocol errors.  

---

## Intermittent Internet Connectivity
- Determine the **scope of the outage:**
  - Continuous **ping** tests to monitor packet loss.  
  - **Traceroute** to identify where connectivity drops.  
  - **Speed tests** to verify performance.  
- If the issue is external, coordinate with the **ISP or third-party provider.**  
- Review your **Service Level Agreement (SLA)** for uptime guarantees and escalation procedures.  
