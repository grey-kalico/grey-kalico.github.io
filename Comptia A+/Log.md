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