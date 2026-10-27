# DFD Study Log 02: iPhone 15 (Engineering Redesign Architecture)

## 1. Target System Overview
* **Device Name:** iPhone 15 (Base Model)
* **Repairability Score:** 7/10 | **DFD Grade:** B- (Dual-Entry Glass Architecture & High Fastener/Cable Clutter)
* **Estimated Disassembly Time & Labor Friction:** ~30–40 minutes | Moderate
* **Target Sub-system:** Logic Board (Motherboard), Shielding Brackets & Flex Cable Harness
* **Primary Structural Flaws:**
  1. **Flaw 1:** High fastener complexity combining proprietary standoff screws, Tri-point Y000, and Pentalobe profiles.
  2. **Flaw 2:** Deep internal placement requiring the removal of almost all major sub-components before accessing the logic board.
  3. **Flaw 3:** Excessive overlapping delicate flex cables crossing the board, raising ribbon-tear risks.
  4. **Flaw 4:** Cryptographic part-pairing restrictions limiting independent third-party board swaps.

---

## 2. Redesign Concept Blueprint

```text
  [EXISTING DESIGN]                           [DFD REDESIGN SOLUTION]
┌─────────────────────────┐               ┌─────────────────────────┐
│ Multi-Drive Fasteners   │               │ Single-Profile Fasteners│
│ (Standoff + Tri-Point)  │  ──────────►  │ (Uniform Micro-Torx T2) │
├─────────────────────────┤               ├─────────────────────────┤
│ Overlapping Individual  │  ──────────►  │ Consolidated High-Density│
│ Flex Cable Harnesses    │               │ Main Bus Ribbon Connect │
└─────────────────────────┘               └─────────────────────────┘
