# DFD Study Log 06: iPhone 13 Pro Max (Engineering Redesign Architecture)

## 1. Target System Overview
* **Device Name:** iPhone 13 Pro Max
* **Repairability Score:** 6/10 | **DFD Grade:** C+ (Adhesive Perimeter & Tied Biometric Assembly)
* **Estimated Disassembly Time & Labor Friction:** ~35–45 minutes | Moderate-High (Requires thermal softening and careful sensor ribbon clearance)
* **Target Sub-system:** Display Panel, Battery Subassembly & FaceID Sensor Array
* **Primary Structural Flaws:**
  1. **Flaw 1:** High-density continuous perimeter adhesive securing the display assembly to the stainless steel frame.
  2. **Flaw 2:** FaceID ear-speaker and sensor array tightly bound directly to the rear of the display panel, complicating screen replacement.
  3. **Flaw 3:** Stretch-release adhesive pull-tabs under the high-capacity battery cell prone to snapping during manual extraction.
  4. **Flaw 4:** Multi-bracket shielding plates requiring multiple specialized driver profiles (Tri-point, Standoff, Pentalobe).

---

## 2. Redesign Concept Blueprint

```text
  [EXISTING DESIGN]                           [DFD REDESIGN SOLUTION]
┌─────────────────────────┐               ┌─────────────────────────┐
│ Adhesive Perimeter Seal │               │ Molded EPDM Gasket +    │
│ + Display-Bound FaceID  │  ──────────►  │ Frame-Mounted Biometrics│
├─────────────────────────┤               ├─────────────────────────┤
│ Stretch-Release Glue    │               │ Stamped Sliding Battery │
│ Pull-Tabs Under Cell    │               │ Tray with Latch Release │
└─────────────────────────┘               └─────────────────────────┘
