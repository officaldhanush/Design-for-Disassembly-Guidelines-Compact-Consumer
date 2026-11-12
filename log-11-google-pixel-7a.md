# DFD Study Log 11: Google Pixel 7a (Engineering Redesign Architecture)

## 1. Target System Overview
* **Device Name:** Google Pixel 7a
* **Repairability Score:** 5/10 | **DFD Grade:** D+ (Adhesive Plastic Back Panel & Fragile Battery Pull Tabs)
* **Estimated Disassembly Time & Labor Friction:** ~35–45 minutes | Moderate-High (Requires thermal softening and careful adhesive management)
* **Target Sub-system:** Thermoformed Plastic Rear Cover, Wireless Charging Coil & Internal Battery Well
* **Primary Structural Flaws:**
  1. **Flaw 1:** High-density perimeter adhesive bonding the thermoformed plastic rear panel directly to the aluminum midframe.
  2. **Flaw 2:** Brittle battery stretch-release pull tabs that frequently tear under tension, requiring chemical solvent (IPA) intervention.
  3. **Flaw 3:** Wireless charging coil and display flex cables routed tightly across structural pathways above the battery tray.
  4. **Flaw 4:** Multi-step entry friction requiring a combination of thermal pad application and Torx unfastening.

---

## 2. Redesign Concept Blueprint

```text
  [EXISTING DESIGN]                           [DFD REDESIGN SOLUTION]
┌─────────────────────────┐               ┌─────────────────────────┐
│ Adhesive-Bonded Plastic │               │ Mechanically Secured    │
│ Rear Panel Cover        │  ──────────►  │ Rear Cover + EPDM Gasket│
├─────────────────────────┤               ├─────────────────────────┤
│ Brittle Battery Pull    │               │ Stamped Sliding Battery │
│ Tabs Prone to Tearing   │               │ Tray with Latch Release │
└─────────────────────────┘               └─────────────────────────┘
