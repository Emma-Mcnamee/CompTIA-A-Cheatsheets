# 🔐 HSM & TPM

## 🧠 Keeping Secrets

Information Technology relies heavily on **trust and confidentiality**.  
- Systems and applications must **keep secrets** safe.  
- **Encryption** is used to protect those secrets — but encryption is only as strong as how securely the **keys** are stored.  

This is where **TPMs** and **HSMs** come in.

---

## 🧱 Trusted Platform Module (TPM)

### 🧩 Overview
- A **hardware-based** encryption component built into individual systems.  
- Acts as a **cryptographic processor** that securely generates and stores keys.  
- Designed to ensure encryption keys are **unique and device-bound**.  

### ⚙️ TPM Functions
- Includes:
  - **Random Number Generator (RNG)** for secure key generation.  
  - **Persistent and versatile memory** for storing burned-in and user keys.  
- Each TPM contains a **unique key** tied to that specific computer.  
  - Prevents encrypted drives from being moved to another system.  
- Acts as a **Root of Trust** — verifies the integrity of the hardware and firmware.  

### 🔧 BIOS Configuration
- TPM options can be managed through the **BIOS/UEFI**:
  - Enable or disable TPM functions.  
  - Clear TPM data (wipe stored keys).  
  - Configure deletion and reset parameters.  

---

## 🧰 Hardware Security Module (HSM)

### 🏢 Overview
- A **dedicated hardware device** used in large-scale or enterprise environments.  
- Provides **secure key storage** for multiple systems (like servers or data centers).  
- Often used to protect the **certificate authority (CA)** and other critical cryptographic operations.  

### 💾 Key Features
- Offers **key backup and recovery** for high availability.  
- **Centralized** and highly secure — often physically tamper-resistant.  
- Can store **encryption, signing, and authentication keys** for multiple servers.  

### ⚖️ TPM vs HSM
| Feature | TPM | HSM |
|----------|-----|-----|
| Scope | Single device | Multi-system / enterprise |
| Key Storage | Built into motherboard | External secure module |
| Use Case | Endpoint encryption, BitLocker, system trust | Certificate management, large-scale encryption |
| Managed Through | BIOS/UEFI | Dedicated management interface |

---

## 🧩 Key Takeaways
- **TPM** = local encryption hardware that binds keys to one device.  
- **HSM** = centralized, enterprise-grade key management hardware.  
- Both ensure **encryption integrity** and **hardware-level security**.  
