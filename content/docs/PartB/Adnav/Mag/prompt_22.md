---
title: Marine Magnetic Compass adjustment:General principles of compass correction
  and the methods of finding and compensating for A, B. C, D and E types of deviation;
type: docs
sidebar:
  open: true
---

Of course. This is a fundamental and critical skill in marine navigation. Here is a comprehensive breakdown of the principles and methods for adjusting a marine magnetic compass.

### **I. General Principles of Compass Correction**

The goal of compass adjustment (or "compass correction") is **not** to eliminate all deviation, but to reduce it to a minimum manageable level and, most importantly, to accurately determine the remaining deviation across all headings.

**1. The Problem: The Ship's Magnetic Field**

A ship is a large mass of steel, containing both:
*   **Hard Iron (Permanent Magnetism):** Steel that has become permanently magnetized during construction (due to hammering, welding, and sitting in the Earth's magnetic field). This magnetism is fixed relative to the ship's structure.
*   **Soft Iron (Induced Magnetism):** Steel that becomes temporarily magnetized by the Earth's magnetic field. The polarity and strength of this magnetism change as the ship changes its heading and geographic location (latitude).

These two types of magnetism combine to create a complex magnetic field around the ship that pulls the compass needle away from Magnetic North. This error is called **Deviation**.

**2. The Solution: The Binnacle and Correctors**

The compass is housed in a binnacle, which is specifically designed to hold a set of correctors. The principle of adjustment is to create an artificial magnetic field that is **equal and opposite** to the ship's deviating field, thereby neutralizing its effect on the compass.

The primary correctors are:
*   **Permanent Magnets:** Small, strong magnets placed in holders within the binnacle to counteract the ship's permanent magnetism (Hard Iron).
*   **Soft Iron Spheres (Quadrantal Correctors):** Two spheres of soft iron fitted on brackets on either side of the compass bowl to counteract the magnetism induced in the ship's soft iron.
*   **Flinders Bar:** A vertical soft iron bar placed in a case on the binnacle to correct for magnetism induced in vertical soft iron.
*   **Heeling Error Magnets:** Magnets in a central vertical tube beneath the compass to counteract deviation caused when the ship rolls or lists.

---

### **II. The Coefficients of Deviation**

To analyze and correct deviation systematically, it is broken down into five theoretical components called coefficients: A, B, C, D, and E.

The total deviation on any heading can be approximated by the formula:
**Deviation = A + B sin(H) + C cos(H) + D sin(2H) + E cos(2H)**
*(where H is the compass heading)*

Here’s a breakdown of each coefficient:

---

### **Coefficient A**

*   **Description:** A constant error that is the same on all headings.
*   **Cause:** It is primarily a mechanical error, not a magnetic one.
    *   Misalignment of the compass lubber line with the ship's fore-and-aft line.
    *   Asymmetrical arrangement of magnets within the compass card.
    *   A slight error in the calculation after correcting the other coefficients.
*   **Finding Method:**
    1.  "Swing the ship" and record the deviation on at least 8 equally spaced headings (e.g., N, NE, E, SE, S, SW, W, NW).
    2.  Sum all the deviations algebraically (paying attention to East (+) and West (-)).
    3.  **Coefficient A = (Sum of all deviations) / (Number of headings)**.
*   **Compensation Method:**
    *   This is the **last** correction to be made.
    *   If Coefficient A is significant (more than a degree or two), it is corrected by physically rotating the compass bowl in its gimbals.
    *   If the deviation is 2°E, you rotate the bowl 2° to the left (counter-clockwise) to bring the lubber line to the correct position. If 2°W, rotate the bowl 2° to the right (clockwise).

---

### **Coefficient B (Semicircular Deviation)**

*   **Description:** A sine-curved deviation that is maximum on East and West headings and zero on North and South.
*   **Cause:** The fore-and-aft component of the ship's permanent magnetism (Hard Iron) and magnetism induced in vertical soft iron (corrected by the Flinders Bar).
*   **Finding Method:**
    1.  Steady the ship on a heading of **East (090°) or West (270°) by compass**.
    2.  Determine the correct magnetic heading from a gyrocompass (with gyro error applied), a known transit, or by observing a celestial body.
    3.  The difference between the compass heading and the magnetic heading is the deviation. On an East heading, this deviation is almost entirely due to Coefficient B.
*   **Compensation Method:**
    *   This correction is made using the **athwartships permanent magnets**. These are magnets placed in horizontal trays running from port to starboard inside the binnacle.
    *   With the ship on heading East or West, move the athwartships magnets (red ends to starboard for easterly deviation, red ends to port for westerly deviation) in or out of their holders until the compass heading matches the magnetic heading (i.e., deviation is zero).

---

### **Coefficient C (Semicircular Deviation)**

*   **Description:** A cosine-curved deviation that is maximum on North and South headings and zero on East and West.
*   **Cause:** The athwartships (port-starboard) component of the ship's permanent magnetism (Hard Iron).
*   **Finding Method:**
    1.  Steady the ship on a heading of **North (000°) or South (180°) by compass**.
    2.  Determine the correct magnetic heading.
    3.  The difference is the deviation on this heading, which is almost entirely due to Coefficient C.
*   **Compensation Method:**
    *   This correction is made using the **fore-and-aft permanent magnets**. These are magnets placed in horizontal trays running parallel to the ship's keel.
    *   With the ship on heading North or South, move the fore-and-aft magnets (red ends forward for easterly deviation, red ends aft for westerly deviation) in or out of their holders until the deviation is zero.

**Order of Correction for B & C:** It is standard practice to correct B on an East/West heading first, then correct C on a North/South heading.

---

### **Coefficient D (Quadrantal Deviation)**

*   **Description:** A sine-curved deviation with two cycles. It is maximum on the intercardinal headings (NE, SE, SW, NW) and zero on the cardinal headings (N, S, E, W).
*   **Cause:** Magnetism induced by the Earth's field in the ship's **symmetrical horizontal soft iron**.
*   **Finding Method:**
    1.  After correcting for B and C, steady the ship on an **intercardinal heading (e.g., NE, 045° by compass)**.
    2.  Determine the correct magnetic heading.
    3.  The remaining deviation is primarily Coefficient D.
*   **Compensation Method:**
    *   This is corrected using the **soft iron spheres (Quadrantal Correctors)**.
    *   If the deviation is positive (Easterly on NE/SW, Westerly on SE/NW), move the spheres **inward**, closer to the compass.
    *   If the deviation is negative (Westerly on NE/SW, Easterly on SE/NW), move the spheres **outward**, away from the compass.
    *   Adjust the spheres until the deviation on the intercardinal heading is zero.

---

### **Coefficient E (Quadrantal Deviation)**

*   **Description:** A cosine-curved deviation with two cycles. Like D, it is maximum on intercardinal headings and zero on cardinal headings, but it is 90° out of phase with D.
*   **Cause:** Magnetism induced in **asymmetrical horizontal soft iron** (e.g., the compass not being on the ship's centerline).
*   **Finding Method:** This coefficient is usually very small and often ignored. It is found by detailed analysis of the residual deviation curve after A, B, C, and D have been corrected.
*   **Compensation Method:**
    *   Correction is rarely performed by ship's crew.
    *   It is corrected by **skewing the quadrantal correctors**. This means one sphere is moved slightly forward and the other slightly aft. This is a job for a professional compass adjuster.

### **Summary of the Practical Adjustment Process**

1.  **Preparation:** Ensure the ship is upright, all equipment is in its normal sea-going position, and the area is free of external magnetic disturbances (no other ships, cranes, or metal structures nearby).
2.  **Set Flinders Bar (if needed):** Usually set by a professional based on the ship's magnetic latitude and build.
3.  **Correct Heeling Error (Preliminary):** Set the heeling error magnet bucket to the correct height for the magnetic latitude.
4.  **Correct Coefficient B:** Steer East (or West). Adjust the **athwartships magnets** to remove deviation.
5.  **Correct Coefficient C:** Steer North (or South). Adjust the **fore-and-aft magnets** to remove deviation.
6.  **Correct Coefficient D:** Steer NE (or any intercardinal). Adjust the **soft iron spheres** to remove deviation.
7.  **Swing for Residuals:** Swing the ship again, stopping on at least 8 headings. Record the small remaining deviations.
8.  **Find and Correct Coefficient A:** Calculate 'A' from the residual deviations. If significant, correct by **rotating the compass bowl**.
9.  **Create a New Deviation Card:** Record all residual deviations on a new card and post it at the steering station. This card is essential for converting between compass and magnetic headings during navigation.