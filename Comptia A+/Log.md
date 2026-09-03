## 📅 Day 2 — September 3, 2026

**Topic:** 1.1 — Laptop Keyboard Troubleshooting

### What I learned

**Software-first troubleshooting steps for a laptop keyboard before touching hardware:**

Uninstall the keyboard driver (Device Manager) then reboot — Windows reinstalls a fresh copy automatically, which clears out a corrupted driver
Update the driver manually if a reinstall alone doesn't fix it, in case a newer version resolves the issue

**Physical steps once software is ruled out:**

Remove the keycap to check for debris, a broken retention clip, or damage under the key
Unseat and reseat the keyboard itself — disconnecting the ribbon cable/connector from the motherboard and reconnecting it, since a loose or dirty connection is a common cause of dead keys or an unresponsive keyboard
Something that clicked

The troubleshooting order mirrors the general "simplest/least invasive first" logic from CompTIA's troubleshooting methodology — rule out software (drivers) before jumping to hardware (keycaps, connectors). It's the same instinct as checking cables before assuming a part is broken.

### Next up

Want to study keycap replacement on a peripheral/desktop PC keyboard next — different mechanism than a laptop (no ribbon cable to unseat, but mechanical switches, stabilizers, and keycap pullers come into play).

### Real-world connection

This is a classic Tier 1 helpdesk flow: try the free/software fix first (driver reinstall), then move to a quick physical check (keycap, reseating) before escalating to hardware replacement or depot repair.

### Practice / resources used
Video walkthrough on laptop keyboard troubleshooting (driver uninstall/update, keycap removal, unseating/reseating the keyboard)

---

## 📅 Day 1 — September 1, 2026

**Topic:** 1.1 — Monitor Mobile Device Hardware + Replacement Techniques (Battery Health)

### What I learned
- **Form factor** = the physical shape/size of a battery, built to match a specific laptop model (like a phone case only fitting one phone)
- **Modular** = easy to remove/replace without tools, like a LEGO piece snapping in and out. Non-modular batteries are glued/soldered in and much harder to service
- Checked battery health using:
  - `powercfg /batteryreport` (command prompt) — generates an HTML report with Design Capacity vs. Full Charge Capacity
  - `powercfg.cpl` — opens Power Options GUI
- Other ways techs check battery health:
  - BIOS/UEFI diagnostics screen (before Windows even loads)
  - Manufacturer tools (Dell SupportAssist, HP Support Assistant, Lenovo Vantage)
  - Physical inspection (swelling, excess heat)
  - Third-party tools (BatteryInfoView, HWiNFO)

### Something that clicked
Design Capacity vs. Full Charge Capacity is the real "proof" a battery is degrading — not just how it *feels* day to day. If Full Charge Capacity has dropped way below Design Capacity, that's hard evidence of wear.

### Still fuzzy on
- Exact cycle count thresholds where a battery is officially "end of life"

### Real-world connection
Helpdesk (Tier 1) usually just diagnoses (report, charger swap, reseat) — actual battery replacement on non-modular laptops often gets escalated to a repair tier or authorized service center.

### Practice / resources used
- Hands-on: ran `powercfg /batteryreport` and `powercfg.cpl` myself

---

