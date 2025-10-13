# Virtualization

## 🧠 Virtualization Concepts

### 🖥️ Virtualization
- One **physical device**, multiple **operating systems**.
- Each OS has its own **CPU, memory, and network**, but shares the same hardware.
- This is known as **host-based virtualization** — your normal desktop can run multiple environments.
- Concept dates back to **1967 IBM mainframes**.

---

### 🧪 Sandboxing
- An **isolated testing environment** with no connection to the real world.
- A technical **safe space** for testing code or changes.
- Used for:
  - Developing and testing applications in a VM.
  - Preventing test code from affecting live systems.

---

### 💾 Legacy Software & Operating Systems
- Run **different versions** of applications on the same system using multiple VMs.
- Enables **legacy app support** by creating a VM with an older OS.
- Keeps outdated software functional without affecting the main system.

---

### 🔁 Cross-Platform Virtualization
- Run **Windows, macOS, and Linux** simultaneously.
- Saves **time, hardware, and resources**.
- Ideal for developers and testers who need multi-OS access.

---

## ⚙️ Virtualization Services

### 🧩 The Hypervisor
- Acts as a **Virtual Machine Manager**, controlling VMs and their resources.
- Requires **CPU support for virtualization** to efficiently manage resources.
- Adds some **overhead and complexity**, so a capable CPU is important.

---

### 🧱 Hypervisor Types
- **Type 1 (Bare Metal):**  
  - The hypervisor runs **directly on the hardware**.  
  - Example: VMware ESXi, Microsoft Hyper-V Server.  
- **Type 2 (Hosted):**  
  - The hypervisor runs **within an existing OS**, and VMs run on top.  
  - Example: VirtualBox, VMware Workstation.

---

### 💽 Resource Requirements
- **CPU Support:**
  - AMD → `AMD-V`  
  - Intel → `Virtualization Technology (VT-x)`
- Each VM needs:
  - Sufficient **CPU, memory, and storage** for a full OS.
- Overcommitting resources can cause instability or lag.

---

### 🌐 Network Requirements
- Most VM managers have **internal virtual networks**.
- Common network modes:
  - **Shared Network Address (NAT):**  
    - VM shares the host’s IP address using internal private IPs.  
    - NAT translates traffic to the host IP.
  - **Bridged Network:**  
    - VM behaves as a separate device on the physical network.
  - **Private Network:**  
    - VM is isolated; no external communication.

---

### 🔒 Hypervisor Security
- The hypervisor can be a **vulnerability target**.
- **VM escaping:** Malware moves from one VM to another via shared resources.
- **Guest OS Security:**
  - Each VM should be treated as a **separate system**.
  - Apply **traditional security controls** (firewalls, antivirus, patching).
- Be cautious of **pre-built public VMs** — attackers may distribute infected ones.
- Best practice: **build your own VMs**.

---

## 💻 Virtual Desktop Infrastructure (VDI)

- Applications **run on a remote server**, not the local device.
- The user’s device acts only as a **keyboard, mouse, and display**.
- Known as **DaaS (Desktop as a Service)**.
- Benefits:
  - Minimal local hardware requirements.
  - Easy management and updates.
- Limitation:
  - Requires **strong, stable network connectivity**.

---

## 📦 Application Containerization

### 🔍 Overview
- Different from VMs — containers share the **host OS kernel**.
- Cannot run **multiple operating systems** simultaneously.
- Focuses on **virtualizing the application**, not the full OS.

### 🧰 Container Characteristics
- Contains **everything needed** to run an app (dependencies, libraries, config files).
- **Self-contained, portable, and lightweight.**
- Containers:
  - Don’t interact with each other directly.
  - Run **identically in any environment**.
  - Solve “it works on my machine” issues.

---

## 🆚 VMs vs. Containers

| Feature | Virtual Machines | Containers |
|----------|------------------|-------------|
| **Virtualization Level** | Hardware (via Hypervisor) | Software (above OS) |
| **OS Requirement** | Each VM runs its own OS | Share host OS |
| **Performance** | More overhead | Lightweight |
| **Isolation** | Strong, full-system isolation | Process-level isolation |
| **Startup Speed** | Slower | Very fast |
| **Use Case** | Multiple OS environments | Rapid app deployment |

---

**End of Notes**
