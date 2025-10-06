# 🧠 The BIOS

## Overview

**BIOS (Basic Input/Output System)**  
- Software used to start the computer — the system’s *firmware*.  
- Stored on the motherboard in **flash memory**.  
- Initializes the **CPU** and **memory** (called the *Power-On Self Test* or POST).  
- Launches the **Operating System (OS)** after startup.  

### 🧩 Legacy BIOS
- The original BIOS found on older systems.  
- Limited hardware support.  
- Being phased out in favor of UEFI.  

### 🚀 UEFI BIOS
- **Unified Extensible Firmware Interface**.  
- Standard on all modern systems.  
- Replaces Legacy BIOS with modern hardware support and features.

---

## ⚙️ BIOS Settings

### 🔑 Accessing BIOS
- Common keys: **Del**, **F1**, **F2**, or similar during startup.  
- Some hypervisors allow pausing boot to enter setup.  
- Online **UEFI simulators** are available for practice.  

### ⚡ Fast Startup (Windows 10/11)
- Windows doesn’t fully shut down to allow faster boot times.  
- This may **prevent BIOS access**.  
- To bypass:
  - Hold **Shift** while clicking “Restart.”  
  - Or go through **Settings → Advanced Startup**.  
  - Interrupt the boot process **3 times** to force BIOS entry.  

---

## 🧩 Key Configuration Options

### 🧾 Boot Options
- BIOS controls what happens at power-on.  
- You can **modify boot order** (USB, SSD, HDD, etc).  

### 🔐 USB Permissions
- USB storage can pose **security risks**.  
- Enable or disable access in BIOS.  

### 🌡️ Temperature Monitoring
- Motherboards have **built-in sensors**.  
- BIOS monitors internal temperatures (hardware only, not software).

### 💨 Fans and Cooling
- Fan settings allow **intelligent cooling** control.  
- Found under **hardware monitor** or similar menus.  

---

## 🛡️ Security and Virtualization

### 🔒 Secure Boot
- Verifies digitally signed, trusted software before boot.  
- BIOS includes the **manufacturer’s public key** for signature checks.  
- Ensures only **trusted bootloaders** and OS components run.  
- Typically found under **Security → Secure Boot**.  

### 🧑‍💻 Boot Password Management
- Prevents unauthorized system startup without credentials.  

### 🧠 Virtualization Support
- Allows multiple operating systems to share hardware.  
- Setting found under **CPU configuration** or **advanced features**.  

---

## ⚠️ BIOS Configuration Tips
- Always **backup your BIOS settings** before making changes.  
- Don’t change anything unless you’re **100% sure** what it does.  
- Incorrect BIOS settings can prevent your system from booting.

---

🧩 **Key Takeaways**
- BIOS = firmware bridge between hardware and OS.  
- UEFI = modern, secure replacement for legacy BIOS.  
- Secure Boot, Virtualization, and Fan Control = essential BIOS settings.  
