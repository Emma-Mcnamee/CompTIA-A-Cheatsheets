# 🧰 Troubleshooting Hardware

## ⚙️ Power-On Self Test (POST)

### 🔍 Overview
- **POST (Power-On Self Test)** checks major hardware components before booting the OS.  
- Failures are indicated by **beep codes** or **error displays**.  
- Note: **Beep codes differ** between manufacturers.

---

## 🧾 POST and Boot Issues

### 🖥️ Blank Screen on Boot
- Listen for **beep codes** (indicating hardware failures).  
- Possible causes:
  - Bad **video card**, **RAM**, or **CPU**  
  - **BIOS misconfiguration**  
- Check the **BIOS** and **hardware connections** on the motherboard.

### 🕒 BIOS Time & Settings
- BIOS settings are maintained with the **motherboard battery (CMOS battery)**.  
- If time or settings reset, **replace the battery**.

### 💿 Incorrect Boot Device
- Set **boot order** in BIOS.  
- Confirm startup device has a **valid OS**.  
- Ensure **all drives are properly connected**.

---

## 💥 Crash Screens & System Failures

### 🧩 Windows Stop Error (BSOD)
- Known as the **Blue Screen of Death (BSOD)**.  
- System restarts and **unsaved data is lost**.  
- The **stop code** provides key diagnostic info.

### 💀 Blue Screens & Shutdowns
- Common causes:
  - **Bad hardware**
  - **Corrupted drivers**
  - **Faulty applications**  
- Try:
  - **Last Known Good Configuration**  
  - **System Restore / Rollback Driver**  
  - **Safe Mode Startup**  
  - **Reseat or remove hardware**
  - **Run manufacturer diagnostics**

### 🧾 Proprietary Crash Screens
- Apps may display their own error messages.  
- Gather details for support or help desk:
  - Ask for **screenshots**  
  - Review **ticket instructions**

---

## ⚫ Blank Screen (No Display)

### 🔌 Check Monitor & Connections
- Verify **monitor power and signal cables** (HDMI, DisplayPort, power).  
- Ensure **correct input selection** on the monitor.  
- If image is **dim**, check **brightness controls**.  
- **Test with a known good monitor** to isolate if it’s a monitor or PC issue.

---

## ⚡ No Power

- Check **power at the source** and **power supply output** (use a **multimeter**).  
- If **fans spin but no POST**, suspect:
  - **Bad motherboard**
  - **Insufficient power to components**  
- Fans can spin even if the system isn’t receiving full power (they require low voltage).

---

## 🐢 Sluggish Performance

- Open **Task Manager** to check **CPU, memory, and disk** usage.  
- Confirm the **OS is up to date**.  
- Check for:
  - **Low disk space**  
  - **Fragmentation**  
  - **Power-saving mode (laptops)** — can throttle CPU performance.  
- Run **antivirus/anti-malware scans** for infections.

---

## 🌡️ Overheating

- Computers generate significant **heat** during operation.  
- Check:
  - **Fans, airflow, and heat sinks**  
  - **Dust buildup** (restricts cooling)  
- Use **hardware monitoring software** or **BIOS temperature readings**.  
- Clean dust and ensure **proper ventilation**.

---

## 🔥 Smoke or Burning Smell

- Indicates **electrical failure**.  
- **Immediately disconnect power** and allow smoke to clear.  
- Locate and **replace damaged components**.  
- Never power on a smoking device.

---

## 💤 Random Shutdowns

- Sudden shutdowns with **no warning** or **black screen**.  
- Check:
  - **Event Viewer** for logs  
  - **Temperature** (common cause: overheating)  
  - **Fan and heat sink status** in BIOS  
  - **Thermal paste condition**
- May also be caused by **failing hardware** — run diagnostics.

---

## 💥 Application Crashes

- Symptoms:
  - App stops responding, disappears, or shows error.  
- Troubleshoot by checking:
  - **Event Viewer logs**  
  - **Reliability Monitor** (app history and stability)  
- Try **reinstalling the app** or contacting **vendor support**.

---

## 🔊 Unusual Noises

- Computers should **hum softly**, not make harsh mechanical sounds.

| Sound | Possible Cause |
|--------|----------------|
| **Rattling** | Loose components or heat sinks |
| **Scraping** | Hard drive platter issues |
| **Clicking** | Failing fan bearings |
| **Popping** | Failing capacitors |

---

## ⏰ Inaccurate System Date/Time

- Usually caused by a **bad CMOS battery** on the motherboard.  
- Replace the **button-style battery**.  
- Older systems may reset BIOS configs when removed; modern ones typically do not.

---

**End of Notes**
