---
title: Marine Magnetic Compass adjustment:analysis of a table of deviations;
type: docs
sidebar:
  open: true
---

Excellent question. Analyzing a table of deviations is the core of marine magnetic compass adjustment. It's how a compass adjuster diagnoses the ship's magnetic "illness" before prescribing the "cure" with magnets and soft iron correctors.

Let's break it down step-by-step, from the basics to a full analysis of a sample table.

---

### **1. The Fundamentals: Why We Need This**

A ship is a large steel mass, creating its own magnetic field that interferes with the Earth's magnetic field. This interference causes the ship's compass to point to a direction called **Compass North (CN)** instead of **Magnetic North (MN)**.

The angular difference between Magnetic North and what the compass shows is called **Deviation (D)**.

*   **Goal of Adjustment:** To reduce the deviation to a minimum (ideally less than 2-3 degrees on any heading).
*   **The Tool:** The **Table of Deviations**, created by "swinging the ship" (turning it in a full circle and recording the compass heading against a known magnetic heading at regular intervals, e.g., every 15 or 30 degrees).

### **2. The Sources of Deviation**

Deviation isn't a simple, constant error. It's a complex sum of errors caused by two types of magnetism on the ship:

1.  **Permanent Magnetism (Hard Iron):** Magnetism "baked into" the ship's steel during construction (due to hammering, welding, and sitting in one orientation in the Earth's magnetic field). This causes **Semicircular Deviation**, meaning the error is maximum on two opposite headings and zero on the two headings 90° away.
2.  **Induced Magnetism (Soft Iron):** Temporary magnetism induced in the ship's soft iron components by the Earth's magnetic field. This magnetism changes as the ship changes heading. This causes **Quadrantal Deviation**, meaning the error is maximum on the four intercardinal headings (NE, SE, SW, NW) and zero on the cardinal headings (N, S, E, W).

### **3. The Analysis: Deconstructing Deviation with Coefficients**

To analyze the deviation table, we use a mathematical technique (a simplified Fourier analysis) to break down the total deviation into its component parts. These parts are known as **Coefficients A, B, C, D, and E**.

The approximate formula for deviation (δ) on any compass heading (H_c) is:

**δ ≈ A + B·sin(H_c) + C·cos(H_c) + D·sin(2H_c) + E·cos(2H_c)**

By calculating these coefficients from our table, we can understand the exact nature of the ship's magnetic field and how to correct it.

---

### **4. Example: Analysis of a Table of Deviations**

Let's imagine we have just swung the ship and produced the following table. The deviation is found by subtracting the Compass Heading from the known Magnetic Heading (`Dev = Mag - Comp`).

| Ship's Head (by Compass) | Known Magnetic Heading | **Deviation (Dev)** |
| :----------------------- | :--------------------- | :------------------ |
| 000° (N)                 | 358°                   | **2° W (-2°)**      |
| 045° (NE)                | 043°                   | **2° W (-2°)**      |
| 090° (E)                 | 084°                   | **6° W (-6°)**      |
| 135° (SE)                | 137°                   | **2° E (+2°)**      |
| 180° (S)                 | 184°                   | **4° E (+4°)**      |
| 225° (SW)                | 223°                   | **2° W (-2°)**      |
| 270° (W)                 | 275°                   | **5° E (+5°)**      |
| 315° (NW)                | 317°                   | **2° E (+2°)**      |

*(Note: West deviation is negative (-), East deviation is positive (+). This is crucial for calculations.)*

### **Calculating the Coefficients**

Here’s what each coefficient means and how to calculate it from our table.

#### **Coefficient A (Constant Deviation)**

*   **What it is:** A constant error on all headings.
*   **Cause:** Misalignment of the compass bowl, lubber line not parallel to the keel, or asymmetrical arrangement of soft iron.
*   **Calculation:** The average of all deviations.
    *   `A = (-2 + -2 + -6 + 2 + 4 + -2 + 5 + 2) / 8`
    *   `A = 1 / 8`
    *   **`A = +0.125°`**
*   **Analysis:** This is a very small constant error. It can be physically corrected by rotating the compass bowl slightly. If small enough, it's often left uncorrected.

#### **Coefficient B (Semicircular Deviation)**

*   **What it is:** Deviation that is maximum on East and West headings.
*   **Cause:** **Permanent** fore-and-aft magnetism in the ship.
*   **Calculation:** The average deviation on East minus the average deviation on West, all divided by 2.
    *   `B = (Dev on E - Dev on W) / 2`
    *   `B = (-6 - (+5)) / 2`
    *   `B = -11 / 2`
    *   **`B = -5.5°`**
*   **Analysis:** This is a large negative value. A **negative B** indicates that the forward part of the ship has "blue" magnetism (the pole that attracts the North-seeking pole of a magnet).
*   **Correction:** This is corrected by placing **permanent fore-and-aft magnets** in the binnacle, in this case with their "red" ends forward to counteract the ship's "blue" magnetism.

#### **Coefficient C (Semicircular Deviation)**

*   **What it is:** Deviation that is maximum on North and South headings.
*   **Cause:** **Permanent** athwartships (side-to-side) magnetism in the ship.
*   **Calculation:** The average deviation on North minus the average deviation on South, all divided by 2.
    *   `C = (Dev on N - Dev on S) / 2`
    *   `C = (-2 - (+4)) / 2`
    *   `C = -6 / 2`
    *   **`C = -3.0°`**
*   **Analysis:** This is a significant negative value. A **negative C** indicates that the starboard side of the ship has "blue" magnetism.
*   **Correction:** This is corrected by placing **permanent athwartships magnets** in the binnacle, in this case with their "red" ends to starboard to counteract the ship's "blue" magnetism.

#### **Coefficient D (Quadrantal Deviation)**

*   **What it is:** Deviation that is maximum on the intercardinal headings (NE, SE, SW, NW).
*   **Cause:** **Induced** magnetism in asymmetrical horizontal soft iron.
*   **Calculation:** The average deviation on intercardinal headings (NE, SW) minus the average deviation on the other intercardinals (SE, NW), all divided by 2.
    *   `D = (Avg Dev on NE & SW - Avg Dev on SE & NW) / 2`
    *   `D = ((-2 + -2)/2 - (+2 + +2)/2) / 2`
    *   `D = (-2 - 2) / 2`
    *   `D = -4 / 2`
    *   **`D = -2.0°`**
*   **Analysis:** This is a notable quadrantal error. A **negative D** is less common and suggests that the soft iron is concentrated along the NW-SE axis. A positive D (more common) suggests soft iron concentrated along the fore-aft and athwartships lines (like beams).
*   **Correction:** This is corrected by placing **soft iron spheres (Quadrantal Correctors)** on the sides of the binnacle. For a negative D, the spheres would need to be placed on the fore-and-aft line from the compass, which is usually not possible. In practice, a large D is almost always positive and corrected by moving the spheres closer to or further from the compass.

*(Note: There is also a Coefficient E, another quadrantal error, but it's typically very small and often ignored in initial analysis.)*

### **Summary of the Analysis and Action Plan**

Based on the calculation of coefficients from the deviation table, the compass adjuster now has a clear picture:

1.  **Significant Coefficient B (-5.5°):** There is strong permanent fore-and-aft magnetism. **Action:** Insert fore-and-aft corrector magnets.
2.  **Significant Coefficient C (-3.0°):** There is moderate permanent athwartships magnetism. **Action:** Insert athwartships corrector magnets.
3.  **Moderate Coefficient D (-2.0°):** There is a quadrantal error from horizontal soft iron. **Action:** Adjust the soft iron spheres.
4.  **Negligible Coefficient A (+0.125°):** The constant error is minimal and likely requires no physical correction.

After placing the correctors, the adjuster would swing the ship again to create a new table of **Residual Deviations**. This new table is then used to create the final **Deviation Card** that the navigator uses for daily corrections.