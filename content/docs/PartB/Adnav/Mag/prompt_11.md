---
title: Correcting errors of magnetic compass;
type: docs
sidebar:
  open: true
---

Of course. Correcting the errors of a magnetic compass is a fundamental skill in navigation, whether on a ship or in an aircraft. The errors can be broken down into two primary types that must be corrected through calculation, and several others that are either compensated for mechanically or anticipated by the navigator.

Here is a comprehensive guide to understanding and correcting magnetic compass errors.

---

### The Two Main Errors: Variation and Deviation

The core of compass correction involves accounting for **Variation** and **Deviation**. The goal is to convert a **Compass Heading (C)** into a **True Heading (T)**, which can be plotted on a map or chart.

A popular mnemonic to remember the order of correction is:
**"Can Dead Men Vote Twice At Elections?"**

This stands for:
**C**ompass -> **D**eviation -> **M**agnetic -> **V**ariation -> **T**rue (**A**dd **E**ast)

To go the other way (from a True course on a chart to the Compass course you need to steer):
**"True Virgins Make Dull Company"**

This stands for:
**T**rue -> **V**ariation -> **M**agnetic -> **D**eviation -> **C**ompass

---

### 1. Variation (or Declination)

*   **What it is:** The angular difference between **True North** (the geographic North Pole) and **Magnetic North** (where the Earth's magnetic field lines point). This difference exists because the two poles are not in the same location, and the magnetic pole wanders over time.
*   **Where you find it:** Variation is printed on all nautical and aeronautical charts. It is shown on the **compass rose** on the chart, stating the variation for a specific year and the annual rate of change.
    *   Example: `12° W (2020), annual change 6' E` (6 minutes of a degree east).
*   **How you correct for it:** Variation is a purely geographical error that you correct for with simple arithmetic.
    *   If Variation is **West**, you **ADD** it to the Magnetic Heading to get True Heading. (**West is Best**)
    *   If Variation is **East**, you **SUBTRACT** it from the Magnetic Heading to get True Heading. (**East is Least**)

### 2. Deviation

*   **What it is:** The error caused by the magnetic fields of your own vessel or aircraft. This includes the engine block, steel hull, radios, wiring, and other metallic or electronic equipment. This "local" magnetic field deflects the compass from pointing to Magnetic North.
*   **How you find it:** Deviation is unique to each vessel and even changes depending on which direction the vessel is pointing. It is determined by a process called **"Swinging the Compass"**:
    1.  The vessel is turned to known magnetic headings (e.g., North, 30°, 60°, East, etc.).
    2.  At each point, the reading on the ship's compass is compared to the known magnetic heading.
    3.  The difference is the deviation for that specific heading.
*   **How you correct for it:**
    *   **Step 1: Compensation (Physical Correction):** A professional compass adjuster will place small magnets and pieces of soft iron (Flinders bar, quadrantal spheres) near the compass to counteract the ship's magnetic field as much as possible. This reduces, but rarely eliminates, deviation.
    *   **Step 2: The Deviation Card (Calculation):** After compensation, the remaining error is recorded on a **Deviation Card**. This card lists the deviation for various headings (e.g., every 15 or 30 degrees). The navigator uses this card to find the deviation for their current heading and apply it.
        *   If Deviation is **West**, you **ADD** it to the Compass Heading.
        *   If Deviation is **East**, you **SUBTRACT** it from the Compass Heading.

---

### The Full Correction Process: A Worked Example

Let's use the mnemonic **"Can Dead Men Vote Twice" (CDMV T)**.
The rule for the calculation is **ADD WESTERLY** errors and **SUBTRACT EASTERLY** errors as you go from Compass to True.

**Scenario:**
*   You are steering a course that reads **115°** on your ship's compass.
*   You look at your deviation card and for a heading of ~115°, the deviation is **3° E**.
*   You look at the compass rose on your nautical chart and it says the variation is **12° W**.

**Let's calculate your True Heading:**

1.  **C**ompass Heading: **115°**
2.  **D**eviation: **3° E** (Easterly, so we subtract)
    *   `115° - 3° = 112°`
3.  **M**agnetic Heading: **112°**
4.  **V**ariation: **12° W** (Westerly, so we add)
    *   `112° + 12° = 124°`
5.  **T**rue Heading: **124° T**

Your actual course over the ground, which you would plot on the chart, is **124°**.

---

### Other Compass Errors (Especially Important in Aviation)

These are transient errors caused by the physical properties of the compass. You don't "correct" them with a calculation, but rather anticipate them while maneuvering. They are caused by **Magnetic Dip**.

*   **What is Magnetic Dip?** Near the magnetic poles, the Earth's magnetic field lines point down into the Earth, not parallel to the surface. This vertical pull causes the compass card to tilt.

This tilt leads to two main turning/acceleration errors in the Northern Hemisphere (the rules are reversed in the Southern Hemisphere):

#### 3. Northerly/Southerly Turning Errors

*   When turning **from a northerly heading**, the compass will initially lag or indicate a turn in the opposite direction.
*   When turning **from a southerly heading**, the compass will lead the turn, showing the turn faster than it is actually happening.
*   **Mnemonic (Pilots): UNOS** - **U**ndershoot **N**orth, **O**vershoot **S**outh. When planning a turn to a northerly heading, you must stop the turn *before* you reach it. When turning to a southerly heading, you must turn *past* it.

#### 4. Acceleration/Deceleration Errors

*   This error is most apparent on **East** or **West** headings.
*   **Mnemonic (Pilots): ANDS** - **A**ccelerate **N**orth, **D**ecelerate **S**outh.
    *   If you are on an East or West heading and **accelerate**, the compass will swing toward **North**.
    *   If you are on an East or West heading and **decelerate**, the compass will swing toward **South**.

### Summary Table

| Error Type | Cause | How to Correct |
| :--- | :--- | :--- |
| **Variation** | Difference between True & Magnetic North. | **Calculation:** Found on a chart. Add West/Subtract East to get True. |
| **Deviation** | The vessel's/aircraft's own magnetic field. | **1. Compensation:** Physical magnets to reduce the error. <br> **2. Calculation:** Use a Deviation Card. Add West/Subtract East to get Magnetic. |
| **Magnetic Dip** | Vertical pull of Earth's magnetic field. | **Anticipation:** Understand its effects (turning and acceleration errors). You don't calculate for it in real time. |
| **Oscillation** | Rough seas or air turbulence. | **Practical:** Wait for it to settle or average the swings. Proper fluid damping in the compass helps. |