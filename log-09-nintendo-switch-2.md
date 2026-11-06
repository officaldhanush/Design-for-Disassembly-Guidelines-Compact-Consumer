# DFD Study Log 09: Nintendo Switch 2 (Engineering Redesign Architecture)

## 1. Target System Overview
* **Device Name:** Nintendo Switch 2 (Console Handheld Unit)
* **Repairability Score:** 7.5/10 | **DFD Grade:** B (Mixed-Drive Fasteners & Adhesive Battery Anchors)
* **Estimated Disassembly Time & Labor Friction:** ~35–45 minutes | Moderate (Requires specialized driver bits and careful shell separation)
* **Target Sub-system:** Console Outer Casing Shells, Rail Brackets & Internal Lithium-Ion Battery Pack
* **Primary Structural Flaws:**
  1. **Flaw 1:** Mixed fastener profiles (Y-wing security screws and Phillips/Torx drives) increasing tool-switching friction during outer shell entry.
  2. **Flaw 2:** High-strength pressure-sensitive adhesive (PSA) anchoring the internal battery cell without reliable pull-tabs, increasing puncture risks.
  3. **Flaw 3:** Rigid snap-fit housing tabs prone to plastic deformation or cracking under high mechanical prying force.
  4. **Flaw 4:** Joy-Con rail flex cables routed tightly across primary housing parting lines, risking accidental shear during disassembly.

---

## 2. Redesign Concept Blueprint

```text
  [EXISTING DESIGN]                           [DFD REDESIGN SOLUTION]
┌─────────────────────────┐               ┌─────────────────────────┐
│ Mixed Y-Wing / Phillips │               │ Uniform Micro-Torx (T4) │
│ Fastener Matrix         │  ──────────►  │ Enclosure Fasteners     │
├─────────────────────────┤               ├─────────────────────────┤
│ PSA-Glued Battery Cell  │               │ Stamped Sliding Battery │
│ Without Pull-Tabs       │               │ Tray with Latch Release │
└─────────────────────────┘               └─────────────────────────┘
