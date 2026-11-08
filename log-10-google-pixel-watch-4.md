# DFD Study Log 10: Google Pixel Watch 4 (Engineering Redesign Architecture)

## 1. Target System Overview
* **Device Name:** Google Pixel Watch 4
* **Repairability Score:** 4/10 | **DFD Grade:** D (Curved 3D Display Adhesive & High Fracture Risk)
* **Estimated Disassembly Time & Labor Friction:** ~40–50 minutes | High (Requires precise localized thermal softening and high-risk glass separation)
* **Target Sub-system:** Curved 3D AMOLED Display Glass, Internal Chassis Carrier & Mainboard Assembly
* **Primary Structural Flaws:**
  1. **Flaw 1:** High-density structural perimeter liquid adhesive bonding the curved 3D glass display directly to the metal housing rim, creating severe fracture risks during prying.
  2. **Flaw 2:** Ultra-short display flex ribbon cables coupled tightly to the chassis, leaving zero slack for safe lifting during unbonding.
  3. **Flaw 3:** Complete absence of mechanical fasteners or retaining rings for the primary watch face assembly.
  4. **Flaw 4:** Liquid silicone rubber (LSR) and adhesive seals tightly binding internal sensor modules to the chassis floor.

---

## 2. Redesign Concept Blueprint

```text
  [EXISTING DESIGN]                           [DFD REDESIGN SOLUTION]
┌─────────────────────────┐               ┌─────────────────────────┐
│ Curved 3D Glass Bonded  │               │ Twist-Lock Mechanical   │
│ with Perimeter Adhesive │  ──────────►  │ Retaining Ring & Bezel  │
├─────────────────────────┤               ├─────────────────────────┤
│ Glued Internal Sensor   │               │ Silicone O-Ring         │
│ Modules & Tight Flex    │               │ Compression Seal & ZIFs │
└─────────────────────────┘               └─────────────────────────┘
