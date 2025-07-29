---
title: General principles of compass correction and the methods of finding and compensating
  for A, B. C, D and E types of deviation; different methods of swinging ship to obtain
  a deviation table; relation of components P. Q and R and the rods a. b. c. d, e.
  f. g, h and k to th various coefficients and to heeling error; sextantal and octantal
  deviations; use of the Kelvin deflector; principle of the deflector method and its
  limitation; rules to be followed with regard to th·eplacing of correctors; "wiping"
  and degaussing; construction of a curve of deviations and its practical use in coefficient
  analysis· constant, semi-circular, and quadrantal deviation; analysis of a ship's
  deviation book to determine causes of irregular deviations and suggest measures
  for their removal; analysis of a table of deviations; obtaining and explaining the
  approximate coefficients A, B, C, D and E; types of transmitting magnetic compass
  bowls and repeaters.
type: docs
sidebar:
  open: true
---

Of course. This is a comprehensive request covering the entire syllabus of magnetic compass correction. Below is a detailed breakdown of each topic, structured for clarity.

### 1. General Principles of Compass Correction

The purpose of compass correction is to reduce the effects of the ship's own magnetic field on the magnetic compass, a phenomenon known as **deviation**. The goal is not to eliminate deviation entirely, but to reduce it to small, manageable values (typically < 3°) and to accurately record the remaining residual deviation in a table or curve.

*   **Earth's Magnetic Field:** The compass needle aligns with the horizontal component of the Earth's magnetic field.
*   **Ship's Magnetic Field:** A steel ship develops its own magnetic field, which is a combination of two types:
    1.  **Permanent Magnetism (Hard Iron):** Acquired during construction due to hammering, riveting, and welding in the Earth's magnetic field. It is fixed relative to the ship's structure and does not change as the ship changes heading.
    2.  **Induced Magnetism (Soft Iron):** Magnetism induced in the ship's soft iron by the Earth's field. This magnetism changes in polarity and strength as the ship alters its heading and geographic location (latitude).
*   **Deviation:** The angle between the magnetic meridian (where the compass *would* point) and the compass meridian (where it *actually* points). It is named East (+) or West (-) depending on which side of the magnetic meridian the compass needle is deflected.

Correction involves placing correctors (permanent magnets and soft iron) near the compass to create an equal and opposite magnetic field, neutralizing the ship's deviating field at the compass position.

---

### 2. The Coefficients (A, B, C, D, E)

Deviation is mathematically broken down into five coefficients, which isolate the different magnetic forces acting on the compass.

*   **Constant Deviation (Coefficient A):**
    *   **Nature:** A constant error on all headings.
    *   **Cause:** Purely mechanical or observational errors. Examples include:
        *   Lubber's line not aligned with the ship's fore-and-aft line.
        *   Misalignment of the compass card's North mark with its magnetic axis.
        *   Asymmetrical arrangement of needles in the compass card.
    *   **Compensation:** It cannot be corrected by magnets. It is found by analysis and applied as a constant correction, or the lubber's line is physically realigned.

*   **Semi-circular Deviation (Coefficients B and C):**
    *   **Nature:** Varies as the sine/cosine of the compass heading, reaching maximums on two opposite headings and zero on headings 90° away. It completes one cycle in 360° of swing.
    *   **Cause:** The combined effect of the ship's permanent magnetism (hard iron) and induced magnetism in vertical soft iron.
    *   **Coefficient B:** Maximum deviation on North (or South) headings. Caused by fore-and-aft magnetic forces.
    *   **Coefficient C:** Maximum deviation on East (or West) headings. Caused by athwartships magnetic forces.
    *   **Compensation:**
        *   **Coefficient B** is corrected by **fore-and-aft permanent magnets** and the **Flinders Bar** (for the induced portion).
        *   **Coefficient C** is corrected by **athwartships permanent magnets**.

*   **Quadrantal Deviation (Coefficients D and E):**
    *   **Nature:** Varies as the sine/cosine of twice the compass heading, reaching maximums on four headings and zero on four headings. It completes two cycles in 360° of swing.
    *   **Cause:** Induced magnetism in horizontal soft iron (HSI).
    *   **Coefficient D:** Maximum deviation on the intercardinal headings (NE, SE, SW, NW). Caused by symmetrically placed HSI (e.g., beams athwartships).
    *   **Coefficient E:** Maximum deviation on the cardinal headings (N, S, E, W). Caused by asymmetrically placed HSI.
    *   **Compensation:**
        *   **Coefficient D** is corrected by placing **soft iron spheres (or quadrantal correctors)** on the athwartship line through the compass.
        *   **Coefficient E** is usually negligible. If required, it is corrected by slewing the soft iron spheres off the athwartship line.

---

### 3. Relation of Components P, Q, R and Rods to Coefficients

This is the physical model (developed by Archibald Smith) that explains the coefficients. The ship's magnetic forces are resolved into three axes at the compass:

*   **P (Permanent Force):** Fore-and-aft force (+ve forward). Causes **Coefficient B**. Corrected by fore-and-aft magnets.
*   **Q (Permanent Force):** Athwartships force (+ve to starboard). Causes **Coefficient C**. Corrected by athwartships magnets.
*   **R (Permanent Force):** Vertical force (+ve downwards). Does not cause deviation when the ship is upright but is the primary cause of **Heeling Error**. Corrected by a vertical magnet (Heeling Error Corrector) in a bucket below the compass.

The induced magnetism is modeled by nine "soft iron rods" (`a` to `k`), representing the net effect of all soft iron in the ship.

| Rod | Description | Effect on Coefficient | Corrector |
| :-- | :--- | :--- | :--- |
| **`a`** | Fore-and-aft HSI, symmetrical | Affects **B** | Flinders Bar |
| **`b`** | Fore-and-aft HSI, asymmetrical | Affects **B** | Flinders Bar / Magnets |
| **`c`** | Vertical soft iron forward/aft | Affects **B** (induced by Earth's vertical field) | Flinders Bar |
| **`d`** | Athwartships HSI, symmetrical | Affects **D** | Quadrantal Spheres |
| **`e`** | HSI at 45°/135° (asymmetrical) | Affects **E** | Skewed Spheres |
| **`f`** | Vertical HSI below compass | Affects **Heeling Error** | Heeling Error Magnet |
| **`g`** | Vertical soft iron to port/stbd | Affects **C** (induced by Earth's vertical field) | Athwartships Magnets |
| **`h`** | Vertical HSI below compass, asymmetrical | Affects **Heeling Error** | Heeling Error Magnet |
| **`k`** | Vertical soft iron, symmetrical | Affects **Heeling Error** | Heeling Error Magnet |

**Heeling Error:** When a ship heels, permanent vertical force `R` and induced magnetism in vertical iron (`c`, `g`, `k`) gain a horizontal component, causing deviation. It is maximum on North/South headings and zero on East/West. It is corrected by the vertical `Heeling Error Magnet`.

---

### 4. Swinging Ship to Obtain a Deviation Table

"Swinging the ship" is the process of placing the vessel on various known magnetic headings to record the corresponding compass heading and thus find the deviation.

**Methods:**

1.  **Reciprocal Bearings:** An observer on the ship takes a bearing of a shore compass, while a shore observer simultaneously takes a bearing of the ship's compass. The difference between the bearing and its reciprocal (180° difference) is the total error. Subtracting variation gives the deviation.
2.  **Transit Bearings:** The ship is steadied on a heading where two charted, fixed objects are seen in a line (a "transit"). The true bearing of this transit is known from the chart. The magnetic bearing is found by applying variation. The ship's compass bearing is observed. The difference between the magnetic bearing and the compass bearing is the deviation. This is highly accurate.
3.  **Bearing of a Distant Object:** A conspicuous object at a great distance (over 6 miles) is used. Its bearing will not change significantly as the ship swings in a small circle. The magnetic bearing is determined, and deviations are found by comparing it to the compass bearings on different headings.
4.  **Bearing of a Celestial Body (Sun, Star):** The true bearing (azimuth) of the sun is calculated for a specific time and position. The compass bearing is simultaneously observed. The difference is the total compass error (Variation + Deviation). Knowing the variation allows deviation to be found.
5.  **Comparison with a Gyrocompass:** This is the most common modern method. The gyrocompass shows true headings (after applying any known gyro error). The ship is steadied on a heading, and the gyro and magnetic compass readings are recorded. The difference is the total error. `Error = True - Compass`. `Deviation = Error - Variation`.

---

### 5. Methods of Finding and Compensating Coefficients

This is the practical process of compass adjustment, typically done in this order to minimize interaction between correctors.

1.  **Preparation:** Ensure the binnacle is clear of any magnetic material. All correctors are initially removed or in the zero position.
2.  **Correcting Coefficient D (Quadrantal):**
    *   **Find:** Head the ship on an intercardinal heading (e.g., NE magnetic). The amount of deviation is mostly due to `D`.
    *   **Compensate:** Move the soft iron spheres in or out along their arms to reduce the deviation to zero. If deviation is Easterly on NE, the spheres are too close; move them out. If Westerly, move them in.
3.  **Correcting Coefficient C (Semicircular):**
    *   **Find:** Head the ship East or West (magnetic). Any remaining deviation is primarily `C`.
    *   **Compensate:** Insert athwartships permanent magnets into the binnacle. The number and position (height) are adjusted until the deviation is zero. If deviation is Easterly on East heading, the North (red) end of the magnet(s) should be placed to port.
4.  **Correcting Coefficient B (Semicircular):**
    *   **Find:** Head the ship North or South (magnetic). Any remaining deviation is primarily `B`.
    *   **Compensate:** This is a two-part correction:
        *   **Flinders Bar:** Corrects the induced part of `B`. Its size is determined by calculations based on the ship's structure or by swinging the ship in two different magnetic latitudes. It is placed in a tube on the forward or aft side of the binnacle.
        *   **Fore-and-Aft Magnets:** Corrects the permanent magnetism part of `B`. Insert magnets until the remaining deviation is zero. If deviation is Easterly on a North heading, the North (red) end of the magnet(s) should be placed aft.
5.  **Finding Coefficient A:** After correcting B, C, and D, a full swing is conducted to record residual deviations. Coefficient A is the average of the deviations on all headings. It is not corrected mechanically but noted in the deviation card.

---

### 6. Sextantal and Octantal Deviations

These are higher-order deviations caused by more complex interactions of induced magnetism.
*   **Sextantal Deviation:** Varies with `sin(3 x heading)`.
*   **Octantal Deviation:** Varies with `sin(4 x heading)`.
They are almost always negligible on a well-built ship with a properly sited compass and are not corrected.

---

### 7. Use of the Kelvin Deflector

The Kelvin Deflector is an instrument with small magnets used to measure the horizontal directive force (HDF) at the compass position.

*   **Principle:** The deflector applies a known, constant magnetic force to the compass card, deflecting it from the meridian. The amount of deflection achieved by this constant force is inversely proportional to the strength of the ship's HDF on that heading.
*   **Deflector Method of Correction:** This is a method of compass correction without swinging the ship. The deflector is used to measure the HDF on the cardinal and intercardinal headings. By analyzing the variations in HDF, the coefficients can be calculated and the correctors placed.
*   **Limitation:** It is a "dry" or static method. It is less accurate than a full swing because it doesn't account for vibration or the ship's dynamic behavior. It's useful in dry dock or when a swing is impossible, but a verification swing is always recommended.

---

### 8. Rules for Placing Correctors

1.  **Symmetry:** All correctors must be placed symmetrically about the compass pivot.
2.  **Magnets:** Place magnets as low as possible in the binnacle to minimize their effect on the heeling error corrector.
3.  **Flinders Bar:** Always placed on the fore-and-aft line, usually forward of the compass. It should be the first soft iron corrector to be considered.
4.  **Spheres:** Always placed on the athwartship line (unless correcting for Coeff. E), level with the compass card. They should be placed after the Flinders bar.
5.  **Heeling Error Magnet:** Placed vertically in the central tube, directly under the compass card pivot.
6.  **Polarity:** For a positive (+) B (Easterly dev on North), the South (blue) end of the magnet goes forward. For a positive (+) C (Easterly dev on East), the North (red) end of the magnet goes to port.
7.  **Order:** The general order of placing correctors is: Flinders Bar -> Spheres -> Permanent Magnets. This minimizes interaction.

---

### 9. "Wiping" and Degaussing

*   **Degaussing (DG):** The process of neutralizing a ship's magnetic signature to protect it from magnetic mines. Large electrical coils are installed around the ship. When energized, they create a field that opposes the ship's permanent field. Degaussing drastically alters the magnetic field at the compass, rendering its correction invalid. A compass must be re-adjusted after degaussing is installed and tested.
*   **Wiping (Deperming):** A shore-based procedure where heavy electrical cables are wrapped around a ship and energized to erase and reset its permanent magnetism to a very low level. This is done to stabilize the ship's field. The compass must be completely re-adjusted after wiping.

---

### 10. Construction and Use of a Deviation Curve

*   **Construction:** After a swing, a table of residual deviations is created. A graph is plotted with the "Ship's Head by Compass" on the X-axis and "Deviation" on the Y-axis (East is +, West is -). A smooth sine-like curve is drawn through the plotted points.
*   **Practical Use:** It provides a quick visual reference for the navigator to find the deviation for any compass heading without having to interpolate from a table.
*   **Coefficient Analysis:** The shape of the curve gives a visual clue to the dominant coefficients.
    *   A curve shifted up or down from the zero axis indicates **Coefficient A**.
    *   A single wave shape, max/min on N/S, indicates a large residual **B**.
    *   A single wave shape, max/min on E/W, indicates a large residual **C**.
    *   A double wave shape, max/min on intercardinals, indicates a large residual **D**.

