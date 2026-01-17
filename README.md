# Home Assistant Lab — Student Quick Start (v1.2.1)

You do NOT need Docker knowledge.

## What you need
- Raspberry Pi 4
- SD card (16 GB+)
- Network with internet (first boot downloads Home Assistant)

---

## Flash the SD (Raspberry Pi Imager 2.0.3)
1. Open **Raspberry Pi Imager**.
2. Click **⚙ App Options** → **Content repository** and paste:
   `https://raw.githubusercontent.com/jcs-consult/rpi-imager-lab/main/repo.json`
3. Click **Apply & Restart**.
4. **Choose Device** → Raspberry Pi 4
5. **Choose OS** → HA Lab (Clean) – 64-bit (Pi 4)
6. **Choose Storage** → your SD card
7. Click **Write**

---

## Boot and open Home Assistant
1. Insert SD into the Pi and power on.
2. Wait **5–10 minutes** (first boot downloads Home Assistant).
3. Find the Pi IP address (router DHCP list).
4. Open: `http://<PI_IP>:8123`
5. Complete onboarding.

---

## If it does not load after 10 minutes
1. Reboot once.
2. Ensure the network has internet access.
3. Ask the instructor to check the bootstrap service and Docker status.
