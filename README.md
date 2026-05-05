# PC Upgrade Build: From Z490 to Z890 (Kept the CyberPower Case!)

## Overview

I had a solid Intel Z490 build running for a few years and decided it was time for a major upgrade. Rather than buying a whole new case, I reused my **CyberPower C Series** case from the previous build and swapped everything inside. Documented step by step for anyone planning a similar generational upgrade!

**Before** → Intel Core i7-10700K (10th Gen) / RTX 3070 build  
**After** → Intel Core Ultra 7 / MSI Z890 platform / RTX 5070 Ti — same familiar case!

---

## Previous Build Specs

| Component | Spec |
|-----------|------|
| CPU | Intel Core i7-10700K (10th Gen) |
| Cooler | Cooler Master Single Fan AIO | |
| Motherboard | ASUS Z490 |
| RAM | 16GB DDR4 — G.Skill (2 × 8GB) |
| GPU | NVIDIA GeForce RTX 3070 |
| Storage | WD Black 2TB |
| PSU | 600W |
| Case | CyberPower C Series (kept for new build!) |

---

## New Build Components

> 💡 Pro tip: Build your parts list on [PCPartPicker.com](https://pcpartpicker.com) — it auto-checks compatibility and generates a shareable link!

| Component | Part | Notes |
|-----------|------|-------|
| CPU | Intel Core Ultra 7 | Major generational upgrade from the i7-10700K |
| Cooler | Thermalright 360mm AIO | Significant upgrade in cooling capacity |
| Motherboard | MSI Z890 Gaming Plus WiFi | New platform to support Core Ultra and DDR5 |
| RAM | Corsair Dominator 48GB DDR5 (2 × 24GB) | Huge jump from 16GB DDR4 |
| GPU | MSI GeForce RTX 5070 Ti | Massive generational leap from the 3070 |
| Storage (1) | 1TB NVMe SSD | OS + primary games drive |
| Storage (2) | 2TB NVMe SSD | Mass storage / secondary games |
| PSU | Corsair RM1000e (1000W, fully modular) | Upgraded for the 5070 Ti power headroom |
| Case | CyberPower C Series (kept!) | Saved money and it still looks great |

---

## Tools I Used

- Phillips screwdriver (#1 and #2)
- Anti-static wrist strap *(optional but recommended)*
- Zip ties for cable management
- Thermal paste
- Flashlight for tight spots
- Small bowl for screws so nothing rolls away

---

## Step-by-Step Build

---

### Step 1 — Disassembly: Gutting the Previous Build

I unplugged everything and carefully removed all components from the CyberPower case. Since this was an upgrade rather than a brand-new build, I knew the case layout well — but I still **took photos of every cable connection before unplugging** just in case.

Key things I removed:
- ASUS Z490 motherboard + i7-10700K + cooler
- Old 600W PSU and all cables
- RTX 3070 GPU
- WD Black 2TB drive
- All old cables and zip ties

> ⚠️ **Watch out:** Even on a case you know well, label your front panel headers before removing the old board. The Z890 pinout may differ from your Z490!

---

### Step 2 — Case Preparation

With everything out, I:
- Wiped out all the dust with compressed air and a microfiber cloth
- Checked that the motherboard standoffs were in the right positions for the new ATX board
- Confirmed all existing standoffs were properly seated
- Removed an old drive cage to improve airflow for the new build

The CyberPower C Series has decent interior space — plenty of room for the Z890 board and the large 5070 Ti.

---

### Step 3 — Building the Motherboard Outside the Case

**Always build on the bench first** — it's so much easier than working inside the case.

I installed in this order:
1. Intel Core Ultra 7 into the LGA socket on the MSI Z890 (lift the lever, align carefully, lower and lock)
2. Corsair Dominator DDR5 sticks into slots A2 and B2 (check your manual — dual channel slots are rarely slots 1 and 2)
3. 1TB NVMe into the primary M.2 slot, 2TB NVMe into the secondary M.2 slot
4. Applied thermal paste to the CPU (small pea-sized dot in the center)
5. Mounted the CPU cooler

> 💡 **Tip:** The Corsair Dominator sticks are tall — double check cooler clearance before committing to a cooler choice! Also confirm M.2 slot priority in BIOS matches which slot you installed the boot drive in.

---

### Step 4 — Installing the Motherboard into the Case

Lowered the board in at an angle, lined up the I/O shield, then dropped it flat onto the standoffs. Screwed it down in a star pattern — don't fully tighten each screw before moving to the next, let them all seat first.

Then connected:
- 24-pin ATX power connector
- CPU EPS power cable (top left of the board — route this BEFORE installing the GPU or you won't be able to reach it)
- Front panel headers (power button, reset, HDD LED, USB)
- Fan headers

> ⚠️ **Important:** The Z890 front panel USB header layout differs slightly from the Z490. Consult the MSI Z890 Gaming Plus WiFi manual for the correct pinout before connecting.

---

### Step 5 — Adding RAM, GPU & Storage

**RAM:** Seated the two Corsair Dominator DDR5 sticks (2 × 24GB) into slots A2 and B2. The Dominators have a large heatspreader — make sure nothing is obstructing the slot before pressing down. Both clips snapped shut cleanly.

**GPU:** The RTX 5070 Ti is a large card — removed two PCIe slot covers from the CyberPower case, lined up the card with the x16 slot, and pressed firmly until the retention clip clicked. Connected the PCIe power cables from the Corsair RM1000e.

**Storage:** Both NVMe drives were already installed in Step 3.

> 💡 **Note:** The MSI RTX 5070 Ti occupies 2.5 slots — confirm your case has clearance before installing.

---

### Step 6 — Cable Management (The Hard Part!)

The Corsair RM1000e being fully modular made a huge difference — I only attached the cables I actually needed, which cut clutter significantly. The CyberPower case has decent routing holes but tight space behind the tray.

- Routed the CPU EPS cable through the top grommet **before** installing the GPU
- Bundled unused modular cables and stored them in the box — no stuffing excess cables inside the case
- The 5070 Ti needed multiple PCIe power connectors — kept them bundled neatly along the bottom
- Zip-tied everything tight to the back panel

> 💡 **Biggest lesson:** Fully modular PSUs like the RM1000e are worth every penny. Only the cables you need, nothing extra crammed into the case.

---

### Step 7 — First Boot & Testing

Plugged in the monitor via DisplayPort to the 5070 Ti (not the motherboard), keyboard, and mouse. Hit the power button and…

**It posted on the first try.** 🎉

Steps after first boot:
1. Entered BIOS — enabled XMP profile so the Corsair Dominator DDR5 runs at rated speed (DDR5 defaults to base speed without this)
2. Confirmed both NVMe drives were detected (1TB + 2TB)
3. Verified the Intel Core Ultra 7 and RTX 5070 Ti were recognised correctly
4. Booted from USB to install Windows 11
5. Installed MSI Z890 chipset drivers, then GPU drivers
6. Ran stress tests — Prime95 for CPU, FurMark for GPU, 30 minutes each

---

## Final Results

| Metric | Before (Z490 / i7-10700K / 3070) | After (Z890 / Core Ultra 7 / 5070 Ti) |
|--------|----------------------------------|---------------------------------------|
| CPU temps (idle / load) | 38°C / 75°C | 35°C / 68°C |
| GPU temps (load) | 78°C | 65°C |
| Boot time | ~20 seconds | ~7 seconds |
| Gaming FPS (1440p) | 60–90 FPS | 120–180+ FPS |
| Storage speed (sequential read) | ~250 MB/s (WD Black HDD) | ~7,000 MB/s (NVMe Gen4) |
| RAM capacity | 16GB DDR4 | 48GB DDR5 |

---

## Challenges & Lessons Learned

| Challenge | What I Did |
|-----------|------------|
| DDR5 defaulted to base speed on first boot | Enabled XMP profile in MSI BIOS |
| CPU EPS power cable hard to reach after GPU was in | Learned to route it first — before anything else goes in |
| RTX 5070 Ti is a very large card | Removed two PCIe slot covers; checked clearance beforehand |
| Z890 front panel header layout differs from Z490 | Consulted the MSI Z890 Gaming Plus WiFi manual for correct pinout |
| M.2 slot priority needed configuring in BIOS | Set correct boot drive slot in MSI BIOS settings |

---

## Was It Worth It?

**Absolutely.** Reusing the CyberPower C Series case saved money and the familiar layout made the whole process smoother. The jump from the i7-10700K to the Intel Core Ultra 7, from a 3070 to a 5070 Ti, and from 16GB DDR4 to 48GB DDR5 is enormous — this machine handles everything I throw at it without breaking a sweat.

**Total build time:** About 3 hours including cable management and OS reinstall.

---

## Conclusion

If your current case is still in good shape, there's no reason to replace it during an upgrade — put that money toward better components instead. Read your motherboard manual before starting, bench-test outside the case first, and route your CPU power cable before the GPU goes in.

Feel free to open an issue or discussion if you have questions about this build!

---

## Useful Links & Downloads

### MSI Z890 Gaming Plus WiFi — BIOS & Drivers

| Resource | Link |
|----------|------|
| BIOS Updates & Support Page | [msi.com — Z890 Gaming Plus WiFi Support](https://www.msi.com/Motherboard/Z890-GAMING-PLUS-WIFI/support) |
| How to Update BIOS (M-Flash Guide) | [msi.com — BIOS Update Instructions](https://www.msi.com/support/technical_details/MB_BIOS_Update) |
| Z890 Gaming Plus WiFi User Manual (PDF) | [MSI Manual PDF](https://download-2.msi.com/archive/mnu_exe/mb/Z890GAMINGPLUSWIFI_English.pdf) |

### MSI GeForce RTX 5070 Ti — Drivers & Support

| Resource | Link |
|----------|------|
| MSI RTX 5070 Ti Support Page | [msi.com — RTX 5070 Ti Support](https://www.msi.com/Graphics-Card/GeForce-RTX-5070-Ti-16G-GAMING-TRIO-PLUS/support) |
| NVIDIA Official Driver Download | [nvidia.com — GeForce Drivers](https://www.nvidia.com/en-us/drivers/) |
| NVIDIA App (replaces GeForce Experience) | [nvidia.com — NVIDIA App](https://www.nvidia.com/en-us/software/nvidia-app/) |

> 💡 **Tip:** Always update your BIOS before installing the OS, and install GPU drivers after Windows is fully set up. Use the NVIDIA App going forward to keep drivers current automatically.
> 
*Made with ❤️ in Lakeland, Florida*  
⭐ Star this repo if it helped you!
