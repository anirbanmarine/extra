---
title: Marine Magnetic Compass adjustment:magnetic fields;
type: docs
sidebar:
  open: true
---

Of course. This is an excellent topic and is fundamental to marine navigation. Let's break down the adjustment of a marine magnetic compass by focusing on the magnetic fields involved.

### The Core Problem: The Ship is a Magnet

A magnetic compass works by aligning itself with the Earth's magnetic field lines. On a non-magnetic vessel (like a wooden sailboat), it would point to Magnetic North. However, a modern ship is a massive, complex structure of steel and electrical equipment. This creates its own magnetic field, which interferes with the Earth's field at the compass location.

The goal of **compass adjustment (or compensation)** is not to eliminate this interference completely (which is impossible) but to counteract its effects as much as possible, leaving a small, predictable error that can be tabulated and applied by the navigator.

The two primary sources of error are **Variation** and **Deviation**.

*   **Variation (or Declination):** An error caused by the Earth itself. It's the difference between True North (the geographic pole) and Magnetic North. This is not corrected for on the compass itself; it is found on nautical charts and applied mathematically during navigation.
*   **Deviation:** An error caused by the **ship's own magnetic field**. This is the error that we physically adjust or "compensate" for using correctors.

---

### Understanding the Ship's Magnetic Fields

The ship's magnetic field is a combination of two types of magnetism: **Permanent Magnetism (Hard Iron)** and **Induced Magnetism (Soft Iron)**.

#### 1. Permanent Magnetism ("Hard Iron")

This is a fixed magnetic field that the ship acquires during its construction. The constant hammering, riveting, and welding of steel plates in the Earth's magnetic field aligns the magnetic domains within the steel, turning the ship into a giant, permanent magnet.

*   **Characteristics:** The strength and polarity of this field are "frozen" into the ship's structure. It does not change strength, but its effect on the compass changes as the ship turns.
*   **Analogy:** Think of a small bar magnet glued to a turntable. As the turntable spins, the magnet's field affects a nearby compass differently depending on its orientation.

**Components of Hard Iron Magnetism:**

The ship's permanent magnetism is resolved into three components relative to the ship's axes:
*   **P-Force:** The fore-and-aft component. It has its maximum effect on the compass when the ship is heading East or West.
*   **Q-Force:** The athwartships (side-to-side) component. It has its maximum effect when the ship is heading North or South.
*   **R-Force:** The vertical component. It combines with other forces to cause "Heeling Error" when the ship rolls.

**Correction for Hard Iron:**
To counteract a permanent magnetic field, you use other permanent magnets.
*   **B Corrector:** A set of small, powerful permanent magnets placed in a holder fore-and-aft of the compass binnacle. They are adjusted to create an equal and opposite field to counteract the ship's **Q-Force**.
*   **C Corrector:** Identical magnets placed in an athwartships holder to counteract the ship's **P-Force**.
*   **Heeling Magnet:** A vertical magnet in a tube directly below the compass pivot to counteract the **R-Force** and other vertical fields that cause heeling error.

#### 2. Induced Magnetism ("Soft Iron")

This is temporary magnetism induced in the ship's soft iron structures (like the hull, superstructure, masts, etc.) by the Earth's magnetic field.

*   **Characteristics:** This field is not permanent. Its strength and polarity change depending on the ship's heading and its location on Earth (latitude). As the ship turns, different parts of its soft iron structure align with the Earth's field, becoming temporarily magnetized and distorting the field at the compass.
*   **Analogy:** Think of an unmagnetized iron bar. When you bring a magnet near it, the bar itself becomes a temporary magnet. Its magnetism disappears when the external magnet is removed. The ship's soft iron acts like this bar, and the Earth's field is the external magnet.

**Effects of Soft Iron Magnetism:**

*   **Quadrantal Deviation:** Caused by symmetrical soft iron structures around the compass. It is maximum on the inter-cardinal headings (NE, SE, SW, NW) and zero on cardinal headings (N, S, E, W).
*   **Semicircular Deviation:** Caused by asymmetrical soft iron and vertical soft iron (like funnels or masts). The effect from vertical soft iron changes significantly with latitude.

**Correction for Soft Iron:**
To counteract a temporary, induced field, you use other pieces of soft iron.
*   **Quadrantal Spheres:** Two soft iron spheres mounted on brackets on either side of the compass binnacle. By moving them closer to or further from the compass, they acquire their own induced magnetism that counteracts the quadrantal deviation caused by the ship's structure.
*   **Flinders Bar:** A vertical bar of soft iron placed in a case on the forward or after side of the binnacle. It is used to counteract the induced magnetism in the ship's vertical structures. This is especially important for vessels that travel across many latitudes, as the vertical component of the Earth's magnetic field changes dramatically from the equator to the poles.

---

### The Adjustment Process: "Swinging the Ship"

The process of adjusting the compass involves systematically separating and correcting for these different magnetic fields. This is done by a certified compass adjuster in a procedure called "swinging the ship."

1.  **Initial Setup:** The ship is taken to an area of calm water with minimal current. All equipment that might affect the compass (radar, cranes, etc.) is placed in its normal sea-going position. The Heeling Magnet is often set first in port.

2.  **Swinging:** The ship is slowly turned in a full 360° circle, stopping on various headings (usually the 8 cardinal and inter-cardinal points).

3.  **Correcting on Cardinal Headings (N, S, E, W):**
    *   **On a North or South heading:** The effect of the athwartships **Q-Force** (hard iron) is maximum. The adjuster observes the deviation and moves the **B Corrector magnets** in or out to remove it.
    *   **On an East or West heading:** The effect of the fore-and-aft **P-Force** (hard iron) is maximum. The adjuster moves the **C Corrector magnets** in or out to remove this deviation.

4.  **Correcting on Inter-Cardinal Headings (NE, SE, SW, NW):**
    *   With the hard iron effects minimized, any remaining deviation on these headings is primarily **Quadrantal Deviation** (soft iron). The adjuster moves the **Quadrantal Spheres** closer or further away from the compass to remove this error.

5.  **Final Swing and Deviation Card:** The ship is swung again to verify the corrections and record any small, remaining **Residual Deviation**. This data is used to create a **Deviation Card**, which is posted near the compass. The navigator uses this card to find the deviation for any given heading and apply it to their course calculations.

### Summary Table

| Magnetic Field Type | Source | Effect on Compass | Corrected By |
| :--- | :--- | :--- | :--- |
| **Permanent (Hard Iron)** | Ship's fixed magnetism from construction | Semicircular Deviation (P & Q Forces) | **Permanent Magnets** (B & C Correctors) |
| **Permanent (Hard Iron)** | Vertical component (R Force) | Heeling Error | **Heeling Magnet** |
| **Induced (Soft Iron)** | Symmetrical horizontal soft iron | Quadrantal Deviation | **Soft Iron Spheres** |
| **Induced (Soft Iron)** | Vertical soft iron (masts, funnels) | Semicircular Deviation & Heeling Error | **Flinders Bar** |
| **Earth's Field** | Planet's core | Variation / Declination | **Not Corrected**, applied via charts |

By understanding these distinct magnetic fields and their effects, a compass adjuster can methodically apply the correct physical correctors to ensure the magnetic compass remains one of the most reliable and essential tools for safe marine navigation.