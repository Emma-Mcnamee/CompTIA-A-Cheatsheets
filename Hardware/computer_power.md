# 🧠 Computer Power

> ⚠️ **Safety First:**  
> Always disconnect the power source before working on any computer.  
> Remove capacitors, as they can store power even when the device is unplugged.

---

## ⚡ Computer Power Supply

Computers use **DC voltage (Direct Current)**, but most power sources provide **AC (Alternating Current)**.  
Therefore, computers need a **power supply unit (PSU)** to **convert AC to DC**.

- Converts **120V AC** or **240V AC** into **3.3V DC**, **5V DC**, and **12V DC**.
- Provides appropriate voltages for different motherboard components.

---

## 🔢 Electrical Basics

### Ampere (A)
- Measures **rate of electron flow**.
- Think: size of the hose — more amps = more flow.

### Voltage (V)
- Measures **electrical pressure**.
- Think: pressure of the water in the hose.

### Watt (W)
- Measurement of **real power usage**.
- Formula:
- Volts × Amps = Watts
Example: 120V × 0.5A = 60W

---

## 🔄 Current Types

### AC (Alternating Current)
- Direction of current **constantly reverses**.
- Efficient for **long-distance distribution**.
- Frequency of cycle = **Hertz (Hz)**  
*(represented with a wavy line symbol)*

### DC (Direct Current)
- Current flows **in one direction** at a **constant voltage**.  
*(represented with a straight line symbol)*

---

## 🌍 Dual-Voltage Input Options

- **Voltage varies by country.**
- If traveling or moving internationally, make sure the power supply supports the **local voltage**.
- Use a **meter** to measure outlet voltage.
- Some PSUs include a **manual switch** to toggle between voltage ranges (e.g., 115V / 230V).

---

## 🔋 Power Supply Output

Each voltage rail powers different components:

| Voltage | Common Use |
|----------|-------------|
| +12V     | PCIe adapters, hard drives, cooling fans |
| +5V      | Some motherboard components (older standard) |
| +3.3V    | M.2 slots, RAM slots, logic circuits |
| +5VSB    | Standby voltage |
| -12V     | Integrated LAN, legacy serial ports |
| -5V      | Older adapter cards (mostly obsolete) |

---

## 🧩 24-Pin Motherboard Power Connector

- Main motherboard power.
- Provides **+3.3V**, **±5V**, and **±12V**.  
- **Replaced the older 20-pin connector**.

---

## 🧠 Redundant Power Supplies

- Found in **servers** and **critical systems**.
- Use **two or more power supplies** to ensure uptime.
- Typically run at **50% load** until one fails, then the other takes over automatically.

---

## 🔌 Power Supply Connectors

### Fixed Connectors
- Directly attached to the PSU.
- Cheaper, but **less flexible** and **messier cable management**.

### Modular Connectors
- Cables are **detachable**.
- Better airflow and easier cable management.
- Usually more **expensive**.

---

## 📏 Sizing the Power Supply

- PSUs are rated by **watts (W)**.
- Higher wattage = can handle more components, but doesn’t mean faster performance.
- **Physical size** is mostly standard across wattages.
- To size your PSU:
1. Add up the **wattage of all components**.
2. Choose a PSU that provides **slightly more** than your calculated total.

---

## 🌱 Energy Efficiency

- Converting AC → DC creates **waste heat**.
- Check the **efficiency rating** (e.g., *80 Plus Bronze, Gold, Platinum*).
- Higher efficiency =  
- More DC power output  
- Less energy loss  
- Less heat  
- Lower electricity cost

---

**Summary Tip:**  
> The power supply is the backbone of system stability.  
> Always size it correctly, prioritize efficiency, and know your voltage standards.

