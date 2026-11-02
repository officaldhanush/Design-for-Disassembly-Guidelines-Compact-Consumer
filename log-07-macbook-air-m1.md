# DFD Study Log 07: MacBook Air 13" Late 2020 (M1) (Engineering Redesign Architecture)

## 1. Target System Overview
* **Device Name:** MacBook Air 13" Late 2020 (M1)
* **Repairability Score:** 7.5/10 | **DFD Grade:** B (Unibody Shell Architecture with Bonded Battery Cells)
* **Estimated Disassembly Time & Labor Friction:** ~25–35 minutes | Low-Moderate
* **Target Sub-system:** Main Logic Board & Lithium-Polymer Battery Pack Assembly
* **Primary Structural Flaws:**
  1. **Flaw 1:** High-strength adhesive strips securing the multi-cell lithium-polymer battery directly to the aluminum unibody well.
  2. **Flaw 2:** Proprietary Pentalobe (P5) perimeter casing screws requiring specialized driver bits.
  3. **Flaw 3:** Multi-bracket internal EMI shielding arrays requiring meticulous screw sequencing during logic board extraction.
  4. **Flaw 4:** Tightly integrated internal keyboard and trackpad cable ribbons routed beneath structural stiffeners.

---

## 2. Redesign Concept Blueprint

```text
  [EXISTING DESIGN]                           [DFD REDESIGN SOLUTION]
┌─────────────────────────┐               ┌─────────────────────────┐
│ Adhesive-Bonded Battery │               │ Mechanically Secured    │
│ Cells via Pull-Strips   │  ──────────►  │ Drop-In Sliding Battery │
├─────────────────────────┤               │ Tray with Captive Screws│
│ P5 Pentalobe Outer Case │               ├─────────────────────────┤
│ Fastener Profile        │               │ Uniform Micro-Torx (T3) │
└─────────────────────────┘               └─────────────────────────┘
