# DFD Study Log 14: Nintendo Switch Joy-Con (Engineering Redesign Architecture)

## 1. Target System Overview
* **Device Name:** Nintendo Switch Left Joy-Con
* **Repairability Score:** 7.5/10 | **DFD Grade:** B+ (Low-Moderate Friction, High Wear Frequency)
* **Estimated Disassembly Time & Labor Friction:** ~15–25 minutes | Low-Moderate (Simple internal layout, but hindered by soft Y00 screws and delicate ZIF flex cables)
* **Target Sub-system:** Analog Joystick Assembly & Internal Midframe Bracket
* **Primary Structural Flaws:**
  1. **Flaw 1:** Soft external Tri-Point (Y00) housing screws strip easily under incorrect driver torque.
  2. **Flaw 2:** Resistive carbon-track potentiometer wipers wear down over time, causing permanent analog stick drift.
  3. **Flaw 3:** Ultra-dense spatial packaging forces sensitive control elements into close proximity with high-power haptic electromagnets.

---

## 2. Redesign Concept Blueprint

```text
  [EXISTING DESIGN]                           [DFD REDESIGN SOLUTION]
┌─────────────────────────┐               ┌─────────────────────────┐
│ Soft Tri-Point (Y00)    │               │ Standard Torx (T3) or   │
│ Screws & Carbon Track   │  ──────────►  │ Phillips Fasteners &    │
├─────────────────────────┤               ├─────────────────────────┤
│ Potentiometer Joysticks │               │ Magnetically Shielded   │
│ Prone to Drift          │               │ TMR / Hall Modules      │
└─────────────────────────┴               └─────────────────────────┘
