# Troubleshooting Storage Devices

## Storage Failure Symptoms
- **Read/Write failure:** “Cannot read from source disk.”
- **Slow performance:** Constant LED activity, repeated retries.
- **Audible symptoms:** Loud clicking noise (Click of Death), grinding sounds.
  - Hard drives are mechanical with moving actuator arms.
  - Even minor issues can cause failure due to tight tolerances.
  - **Metal-on-metal contact = severe damage.**
- **Always ensure a recent backup is available.**

---

## Troubleshooting Disk Failures
1. **Get a backup first!**
2. Check for **loose or damaged cables.**
3. Check for **overheating**, especially if issues occur after startup.
4. Verify **power supply stability**, particularly after adding new devices.
5. **Run manufacturer diagnostics** for detailed drive health.

---

## Boot Failure System
- **Symptoms:**
  - Drive not recognized.
  - “Boot device not found” or “OS not found” errors.
  - Beeps, indicator lights, or on-screen error messages.
- **OS not found:** Indicates the drive is accessible but the OS is missing or corrupted.

### Troubleshooting Boot Failures
- Inspect **physical connections** and cables.
- Verify **boot configuration** in BIOS/UEFI.
  - Check for removable drives (USB, external) interfering with boot order.
  - Confirm storage interfaces (SATA/NVMe) are enabled.
- For new installations:
  - Recheck **data and power cables.**
  - Try **different SATA ports or cables.**

---

## Data Loss or Corruption
- **All drives eventually fail.**
- Recovery is **difficult and expensive.**
- SSDs may suddenly stop working — sometimes readable but **not writable.**
- Symptoms:
  - Files become inaccessible or corrupted.
  - System freezes during read/write.
- **Preventative measure:** Regular, verified backups.

---

## RAID Failures
- **Possible causes:**
  - Drive hardware failure.
  - Power or communication issues (bad cables, controller problems).
- **Symptoms:**
  - Error messages, email alerts, audible alarms.
- Always **identify the correct failed drive** before removal.

### RAID Recovery Tips
- Check the **RAID management console** before making changes.
- **RAID 0:** 2+ disks. *Single drive failure = total data loss.*
- **RAID 1:** 2+ disks. *Operates as long as one disk works.*
- **RAID 5:** 3+ disks. *Can lose one drive.*
- **RAID 6:** 4+ disks. *Can lose two drives.*
- **RAID 10:** 4+ disks. *Can lose one from each mirrored pair.*

---

## S.M.A.R.T. (Self-Monitoring, Analysis, and Reporting Technology)
- Predicts hardware failure by tracking drive health metrics.
- Use **third-party utilities** or built-in tools to check S.M.A.R.T. data.
- Schedule **regular disk checks** for early detection.
- If warning signs appear → **replace the drive immediately.**

### SMART Analysis
- Monitors drive metrics over time.
- Provides **automated alerts** for failing drives.
- Helps address issues *before* data loss occurs.

---

## Extended Read/Write Times
- **Delays** can occur due to mechanical wear or file system issues.
- **IOPS (Input/Output Operations Per Second):**
  - Key performance metric for storage devices.
  - Useful for comparing drive performance across systems.

---

## Missing Drives in OS
- May be **disabled in BIOS** or **not detected** properly.
- **Checkpoints:**
  - Can the BIOS see the drive?
  - Internal: bad or disconnected cable.
  - External: no power or faulty USB/data cable.
  - Network shares: verify proper connection and startup configuration.

---

## Array Missing
- Check **BIOS/UEFI settings** and RAID configuration.
- Rebuild array only after identifying the root cause.
