# Memory — CompTIA A+

---

## Overview of Memory

### What is Memory?
- **RAM (Random Access Memory):** Temporary, high-speed storage.  
- Programs and data must be loaded into RAM to be used.  
- RAM is **volatile**; it resets when the device powers off.  

---

## RAM Slots

### DIMM (Dual Inline Memory Module)
- Electrical contacts on both sides.  
- 64-bit data width: amount of information read/written.  
- Easily installed or removed from motherboard.  
- **SO-DIMM (Small Outline DIMM):** Smaller form factor used in laptops and portable devices.  

---

## RAM Types

### DRAM
- **Dynamic RAM:** Needs constant refreshing.  
- **Random Access:** Any memory location can be accessed directly.  

### SDRAM
- **Synchronous DRAM:** Runs in sync with system clock for consistent data timing.  

### DDR (Double Data Rate)
- DDR improves SDR by transferring data twice per clock cycle.  
- Versions:
  - **DDR2:** Original DDR improvement.
  - **DDR3:** Twice the data rate of DDR2, higher capacity, not compatible with DDR2.
  - **DDR4:** Increased speed, not backwards compatible.
  - **DDR5:** Further improvement, not backwards compatible.

---

## Memory Technologies

### Error-Checking Memory
- Used in critical systems (VM servers, databases).  

#### Parity Memory
- Adds a **parity bit** (9th bit per byte) to detect errors.  
- Performs a parity check when retrieving data to ensure integrity.  

#### Error Correction Code (ECC)
- Detects and **corrects errors automatically**.  

---

## CPU to RAM Throughput

### Memory Bandwidth
- Measures speed of memory transfers.  
- Units: **MT/s (Megatransfers per second)**.  
- Higher bandwidth = faster data movement.  

### Multi-Channel Memory
- Maximizes throughput between CPU and RAM.  
- Configurations: Dual, Triple, Quad channel.  
- Modules must be same type and supported by motherboard for proper operation.  
