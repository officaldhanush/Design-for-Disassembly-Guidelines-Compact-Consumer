# DFD Study Log 03: PlayStation 5 (Engineering Redesign Architecture)

## 1. Target System Overview
* **Device Name:** PlayStation 5 (Base Model)
* **Repairability Score:** 8.5/10 | **DFD Grade:** A- (Tool-Free Outer Shell, High Modular Isolation)
* **Estimated Disassembly Time & Labor Friction:** ~20–30 minutes | Low-Moderate
* **Target Sub-system:** Cooling Fan, Power Supply Unit (PSU) & Main Heatsink Assembly
* **Primary Structural Flaws:**
  1. **Flaw 1:** High fastener count securing the primary internal EMI/thermal shielding plates.
  2. **Flaw 2:** Deep structural placement of the internal power supply requiring extensive screw sequencing.
  3. **Flaw 3:** Fine dust accumulation paths requiring manual disassembly beyond the outer panels for deep heat exchanger cleaning.

---

## 2. Redesign Concept Blueprint

```text
  [EXISTING DESIGN]                           [DFD REDESIGN SOLUTION]
┌─────────────────────────┐               ┌─────────────────────────┐
│ Tool-Free Outer Covers  │               │ Tool-Free Outer Covers  │
├─────────────────────────┤               ├─────────────────────────┤
│ Multi-Torx Shielding    │  ──────────►  │ Toolless Captive Thumb- │
│ Plate Screws            │               │ Screws & Lever Latches  │
├─────────────────────────┤               ├─────────────────────────┤
│ Embedded Deep Internal  │  ──────────►  │ Quick-Release Modular   │
│ Power Supply Connector  │               │ PSU Slide Channel       │
└─────────────────────────┘               └─────────────────────────┘
