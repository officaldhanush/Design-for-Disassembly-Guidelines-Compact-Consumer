# DFD Study Log 08: iPad Pro 11" 4th Gen (M2) (Engineering Redesign Architecture)

## 1. Target System Overview
* **Device Name:** iPad Pro 11" 4th Gen (M2)
* **Repairability Score:** 4/10 | **DFD Grade:** D (Heavy Perimeter Display Adhesive & High Glass Fracture Risk)
* **Estimated Disassembly Time & Labor Friction:** ~50–60 minutes | High (Requires prolonged thermal blanket softening and careful shimming)
* **Target Sub-system:** Display Panel Assembly, Battery Pack & Internal Chassis Frame
* **Primary Structural Flaws:**
  1. **Flaw 1:** High-density industrial perimeter adhesive bonding the glass display panel directly to the unibody frame, creating severe glass fracture risks during thermal unbonding.
  2. **Flaw 2:** Bonded lithium-polymer battery cells requiring chemical solvents and thermal plates for extraction.
  3. **Flaw 3:** Delicate FaceID sensor and camera cabling routed tightly across perimeter edges, vulnerable to tooling damage.
  4. **Flaw 4:** Complete lack of mechanical fasteners on the primary display assembly, forcing destructive thermal-entry workflows.

---

## 2. Redesign Concept Blueprint

```text
  [EXISTING DESIGN]                           [DFD REDESIGN SOLUTION]
┌─────────────────────────┐               ┌─────────────────────────┐
│ Industrial Perimeter    │               │ Mechanically Secured    │
│ Display Adhesive Tape   │  ──────────►  │ Frame Bezel + EPDM Seal │
├─────────────────────────┤               ├─────────────────────────┤
│ Glued Battery Cells     │               │ Stamped Sliding Battery │
│ Requiring Thermal Heat  │               │ Tray with Latch Release │
└─────────────────────────┘               └─────────────────────────┘
