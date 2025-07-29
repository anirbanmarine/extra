---
title: Marine Magnetic Compass adjustment:relation of components P. Q and R and the
  rods a. b. c. d, e. f. g, h and k to th various coefficients and to heeling error;
type: docs
sidebar:
  open: true
---

Of course. This is a fundamental topic in marine navigation. Let's break down the relationship between the physical forces (P, Q, R), the physical correctors (the rods and magnets), the mathematical coefficients, and heeling error.

### **1. The Foundation: Ship's Magnetism**

A ship, being a large steel mass, develops its own magnetic field that interferes with the Earth's magnetic field, causing the compass to deviate from Magnetic North. This ship's magnetism is divided into two types:

*   **Permanent Magnetism (Hard Iron):** A fixed magnetic field acquired during the ship's construction (due to hammering, welding, and riveting in the Earth's magnetic field). It acts like a permanent bar magnet fixed within the ship. Its effect on the compass changes as the ship turns.
*   **Induced Magnetism (Soft Iron):** A temporary magnetic field induced in the ship's soft iron structures by the Earth's magnetic field. The strength and polarity of this induced field change as the ship's heading and geographic location (magnetic latitude) change.

---

### **2. The Physical Components of Permanent Magnetism (P, Q, R)**

To analyze and correct the permanent magnetism, we resolve it into three mutually perpendicular components relative to the ship's structure.

*   **Component P (Fore-and-Aft):**
    *   **Description:** This represents the permanent magnetism acting along the ship's fore-and-aft line (the keel). A positive `P` force has a "blue" pole (south-seeking) aft and a "red" pole (north-seeking) forward.
    *   **Relation to Coefficient:** Component `P` causes **Coefficient B** deviation. This deviation is maximum when the ship is on East or West headings, as the fore-and-aft force (`P`) is then acting at a right angle to the compass needle, exerting maximum leverage.
    *   **Corrector:** Corrected by permanent **fore-and-aft magnets** placed in the binnacle.

*   **Component Q (Athwartships):**
    *   **Description:** This represents the permanent magnetism acting across the ship (from port to starboard). A positive `Q` force has a "red" pole (north-seeking) on the starboard side.
    *   **Relation to Coefficient:** Component `Q` causes **Coefficient C** deviation. This deviation is maximum when the ship is on North or South headings, as the athwartships force (`Q`) is then acting at a right angle to the compass needle.
    *   **Corrector:** Corrected by permanent **athwartships magnets** placed in the binnacle.

*   **Component R (Vertical):**
    *   **Description:** This represents the permanent magnetism acting vertically through the compass position. A positive `R` force has a "red" pole (north-seeking) pointing downwards.
    *   **Relation to Heeling Error:** On an even keel, Component `R` acts vertically and does not deflect the compass needle horizontally, so it does not cause deviation. However, when the ship **heels** (rolls), this vertical force gains a horizontal component that pushes the needle. This is a primary cause of **Heeling Error**.
    *   **Corrector:** Corrected by the **heeling error magnet (rod `k`)**, a vertical magnet in a central tube directly beneath the compass.

---

### **3. The Mathematical Coefficients of Deviation (A, B, C, D, E)**

Deviation (δ) is expressed by the approximate formula:
**δ = A + B sin(ζ) + C cos(ζ) + D sin(2ζ) + E cos(2ζ)**
(where ζ is the compass course)

*   **Coefficient A:** A constant error on all headings. Usually caused by a misaligned lubber line or a skewed compass card, not magnetism.
*   **Coefficient B:** Semicircular deviation, max on East/West. Caused by **Component P** (permanent) and induced magnetism in vertical soft iron (**rod `g`**).
*   **Coefficient C:** Semicircular deviation, max on North/South. Caused by **Component Q** (permanent).
*   **Coefficient D:** Quadrantal deviation, max on intercardinal headings (NE, SE, SW, NW). Caused by induced magnetism in horizontal soft iron (**rods `a` and `e`**).
*   **Coefficient E:** Quadrantal deviation, max on cardinal headings (N, S, E, W). Caused by induced magnetism in asymmetrical soft iron. Usually negligible.

---

### **4. The Physical Correctors (The Rods and Magnets)**

These are the physical devices in the compass binnacle used to create equal and opposite fields to counteract the ship's magnetism. The letters `a` through `k` are Poisson's standard notation for the soft iron parameters of the ship.

| Corrector | Rod/Component Symbol | Description & Purpose | Corrects For |
| :--- | :--- | :--- | :--- |
| **Fore-and-Aft Magnets** | - (Corrects for **P**) | Small permanent bar magnets placed in a tray/holder in the binnacle, oriented fore-and-aft. | **Coefficient B** (the permanent part) |
| **Athwartships Magnets** | - (Corrects for **Q**) | Small permanent bar magnets placed in a tray/holder, oriented athwartships (port-starboard). | **Coefficient C** |
| **Quadrantal Correctors** | **Rods `d`** (the correctors for rods `a` & `e` in the ship) | Two soft iron spheres placed on brackets to the side of the compass. Their position can be adjusted. | **Coefficient D** |
| **Flinders Bar** | **Rod `g`** (the corrector for rod `g` in the ship) | A vertical bar of soft iron placed in a case on the binnacle, usually forward or aft of the compass. | **Coefficient B** (the induced part) |
| **Heeling Error Magnet** | **Rod `k`** (the corrector) | A permanent magnet in a central vertical tube ("bucket") directly beneath the compass. It can be raised or lowered. | **Heeling Error** |

**Note on Rods `a, b, c, e, f, h`:** These are not physical correctors themselves. They are Poisson's mathematical parameters representing the ship's soft iron structures that *cause* induced magnetism. The physical correctors (Spheres, Flinders Bar) are designed to counteract the effects of these parameters.

*   **Rods `a` & `e`**: Symmetrical horizontal soft iron. Causes **Coefficient D**. Corrected by **Quadrantal Spheres**.
*   **Rod `g`**: Vertical soft iron forward/aft of the compass (e.g., mast, funnel). Causes the induced part of **Coefficient B** and contributes to **Heeling Error**. Corrected by the **Flinders Bar**.

---

### **5. Heeling Error Explained**

Heeling error is the deviation observed when the ship rolls. It is most prominent on North and South courses.

**Causes:**
1.  **Vertical Induced Magnetism:** The Earth's vertical field induces magnetism in the ship's vertical soft iron (masts, funnels - **rod `g`**). When the ship heels, this vertical force gains a horizontal component that deflects the compass.
2.  **Permanent Vertical Magnetism (Component R):** The ship's own permanent vertical field. When the ship heels, this force also gains a horizontal component.
3.  **Transverse Induced Magnetism:** Magnetism induced in the athwartships deck beams beneath the compass.

**Correction:**
The **Heeling Error Magnet (`k`)** is a vertical magnet placed directly below the compass. It is raised or lowered to create a vertical field at the compass that is equal and opposite to the combined vertical fields from **Component R** and the ship's induced magnetism. This neutralizes the force, ensuring that when the ship heels, there is no net vertical force to create a deflecting horizontal component. The adjustment is typically made in port by using a heeling error instrument or at sea by observing the compass swing on a Northerly/Southerly course while the ship is rolling.

### **Summary of Relationships**

| Cause of Error | Physical Force/Component | Mathematical Coefficient | Physical Corrector |
| :--- | :--- | :--- | :--- |
| Permanent Fore-Aft Magnetism | **Component P** | **Coefficient B** (Permanent part) | **Fore-and-Aft Magnets** |
| Permanent Athwartships Magnetism | **Component Q** | **Coefficient C** | **Athwartships Magnets** |
| Induced Vertical Magnetism | Ship's Soft Iron (**Rod `g`**) | **Coefficient B** (Induced part) | **Flinders Bar** |
| Induced Horizontal Magnetism | Ship's Soft Iron (**Rods `a`, `e`**) | **Coefficient D** | **Quadrantal Correctors** (Spheres) |
| Vertical Forces (Permanent & Induced) when Heeled | **Component R** & Ship's Soft Iron (**Rod `g`**) | **Heeling Error** | **Heeling Error Magnet** (**Rod `k`**) |