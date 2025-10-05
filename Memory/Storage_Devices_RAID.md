# Storage Devices — CompTIA A+

---

## Overview of Storage
- **RAM** is temporary; memory disappears when device powers off.  
- **Storage devices** are needed to save data permanently.  

---

## Hard Disk Drive (HDD)
- **Random-access**: Data can be stored anywhere on the drive.  
- **Magnetic storage**: Platters spin rapidly.  
- **Rotational speeds:** 15,000 / 10,000 / 7,200 / 5,400 RPM  

---

## Solid-State Drive (SSD)
- **Non-volatile memory**: No moving parts.  
- Very fast read/write performance.  

### Interfaces
- **PCIe (PCI Express):** Faster than SATA, modern standard.  
- **NVMe:** Connects directly to PCIe bus for high-speed storage.  
- **SATA:** Older standard, designed for hard drives.  
- **SAS (Serial Attached SCSI):** Latest generation, serial communication, higher throughput.  
- **mSATA:** Mini version of SATA for smaller devices.  

---

## Flash Drives
- Non-volatile memory, retains data without power.  
- Limited write cycles and capacity.  
- Not recommended for archival storage.  
- Examples: USB flash drives, SD cards.  

---

## Optical Drives
- Data read using laser beams and microscopic bumps.  
- Relatively slow archival media.  
- Examples: CD-ROM, DVD-ROM, Blu-Ray.  

---

## RAID (Redundant Array of Independent Disks)
- Combines multiple drives for **redundancy and/or performance**.  

### Common RAID Levels
- **RAID 0 (Striping):**  
  - Splits data across 2+ drives.  
  - Fast performance, **no redundancy**.  

- **RAID 1 (Mirroring):**  
  - Duplicate data on 2 drives.  
  - High redundancy, requires double disk space.  

- **RAID 5 (Striping with Parity):**  
  - File blocks split across 3+ drives with parity block.  
  - Data can be reconstructed from parity.  
  - Efficient space usage with high redundancy.  

- **RAID 6:**  
  - RAID 5 with **two parity drives**, requires at least 4 drives.  

- **RAID 10 (RAID 1+0):**  
  - Combines mirroring and striping.  
  - Speed of RAID 0 with redundancy of RAID 1.  
  - Stripe of mirrors configuration.  
