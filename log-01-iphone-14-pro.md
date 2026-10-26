# DFD Study Log 01: iPhone 14 Pro (Engineering Redesign Architecture)

## 1. Target System Overview
* **Device Name:** iPhone 14 Pro
* **Current Repairability / DFD Score:** 6/10 (High adhesive density & multi-screw friction)
* **Target Sub-system:** Lithium-Ion Battery & Perimeter Housing Assembly
* **Primary Failure Modes in Teardown:**
  1. High risk of pull-tab snapping requiring chemical solvent (IPA).
  2. Multi-drive fastener clutter (Pentalobe, Tri-point Y000, Phillips #00) forcing tool switches.
  3. Continuous perimeter liquid glue requiring display thermal baking.

---

## 2. Redesign Concept Blueprint

```text
  [EXISTING DESIGN]                           [DFD REDESIGN SOLUTION]
┌─────────────────────────┐               ┌─────────────────────────┐
│ Outer Display Glass     │               │ Outer Display Glass     │
├─────────────────────────┤               ├─────────────────────────┤
│ Continuous Perimeter    │  ──────────►  │ EPDM Compression Gasket │
│ Liquid Glue (IP68)      │               │ + Internal Snap-Latches │
├─────────────────────────┤               ├─────────────────────────┤
│ Battery glued with      │  ──────────►  │ Mechanical Quick-Release│
│ Stretch-Pull Tabs       │               │ Battery Tray / Latch    │
└─────────────────────────┘               └─────────────────────────┘
