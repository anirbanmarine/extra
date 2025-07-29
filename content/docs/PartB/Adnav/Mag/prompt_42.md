---
title: Marine Magnetic Compass adjustment:Correcting errors of magnetic compass;
type: docs
sidebar:
  open: true
---

Of course. Here is a comprehensive guide to the adjustment and correction of a marine magnetic compass.

---

### **Marine Magnetic Compass Adjustment: A Comprehensive Guide**

A magnetic compass is a primary navigation tool on any vessel and a mandatory backup to electronic systems under SOLAS regulations. Its accuracy is paramount for safe navigation. However, the compass is subject to two main types of errors: **Variation** and **Deviation**.

**Compass adjustment** is the process of physically correcting for **Deviation**.

---

### **Part 1: Understanding the Errors**

Before you can correct the errors, you must understand them.

#### **1. Variation (or Magnetic Declination)**

*   **What it is:** The angular difference between **True North** (the geographic North Pole) and **Magnetic North** (where the Earth's magnetic field lines point).
*   **Cause:** The Earth's magnetic field is not aligned with its axis of rotation. This value changes depending on your location on the globe and slowly changes over time.
*   **How it's "Corrected":** Variation is **not** corrected by adjusting the compass itself. It is a known, predictable value that is **accounted for** during navigation calculations.
*   **Where to find it:** The value of Variation for your specific location is found on the **compass rose** of a nautical chart. The chart will state the variation for a given year and the annual rate of change (e.g., "Var 7°15'W (2018), increasing 6' annually").

#### **2. Deviation**

*   **What it is:** The angular difference between the **Magnetic North** heading and the direction the **Compass Needle** actually points (Compass North).
*   **Cause:** The ship's own magnetic field, created by its steel hull, engine, electrical equipment, and other metallic structures. This field deflects the compass needle.
*   **How it's Corrected:** Deviation **is** corrected by a process called **compass adjustment** or **"swinging the compass."** This involves placing small magnets and soft iron correctors near the compass to counteract the ship's magnetic field.

Deviation is broken down into components caused by two types of magnetism on the ship:

*   **Hard Iron Magnetism:** Permanent magnetism in the ship's steel structures. This creates **Semicircular Deviation** (maximum on North/South or East/West headings).
*   **Soft Iron Magnetism:** Induced magnetism that the ship acquires from the Earth's magnetic field. This changes as the ship changes heading and latitude. This creates **Quadrantal Deviation** (maximum on intercardinal headings: NE, SE, SW, NW).

---

### **Part 2: The Process of Compass Adjustment ("Swinging the Compass")**

This procedure is typically carried out by a qualified and licensed Compass Adjuster.

#### **Step 1: Preparation**

1.  **Choose a suitable location:** Calm seas, clear weather, and an area free of local magnetic anomalies (e.g., away from bridges, power lines, underwater cables, and large metal structures).
2.  **Gather tools:** The compass binnacle, which houses the correctors:
    *   **Fore-and-Aft Magnets (B Corrector):** Small bar magnets placed in a tray below the compass to correct for magnetism along the ship's centerline.
    *   **Athwartships Magnets (C Corrector):** Magnets placed perpendicular to the centerline to correct for magnetism across the ship.
    *   **Quadrantal Spheres (D Corrector):** Two soft iron spheres mounted on either side of the binnacle to correct for induced magnetism.
    *   **Flinders Bar:** A vertical soft iron bar placed in a case on the binnacle to correct for induced magnetism from vertical steel structures.
    *   **Heeling Error Magnet:** A vertical magnet placed directly under the compass card's pivot to correct for errors when the ship rolls.
3.  **Establish a Reference:** You need a way to know the ship's *actual* magnetic heading to compare it against the compass reading. Common methods include:
    *   **Gyrocompass:** The most common method. The gyro heading (True) is converted to a Magnetic heading by applying Variation.
    *   **GPS Heading (COG):** Course Over Ground can be used if there is no current or wind.
    *   **Leading Marks (Ranges):** Aligning two fixed objects on shore to give a known True bearing.
    *   **Celestial Bearings:** Taking a bearing of the sun or another celestial body at a time when its azimuth (True bearing) is known.

#### **Step 2: The "Swing" and Correction Sequence**

The ship is slowly turned in a full circle, stopping at various headings (typically every 15° or 30°) to record the deviation. The corrections are made in a specific order to prevent one adjustment from affecting another.

**The Standard Correction Sequence:**

1.  **(Optional) Heeling Error Correction:** This is usually done in port by simulating a heel and adjusting the vertical magnet.

2.  **Remove Semicircular Deviation (Coefficients B and C):**
    *   **Correcting Coefficient B (Fore-and-Aft Magnetism):**
        *   **Steer the ship East (090°) or West (270°) by the reference (e.g., Gyro).**
        *   Read the deviation on the magnetic compass.
        *   Adjust the **fore-and-aft (B) corrector magnets** (moving the tray in or out, or adding/removing magnets) until the deviation is reduced to zero (i.e., the magnetic compass reads 090° or 270° Magnetic).
    *   **Correcting Coefficient C (Athwartships Magnetism):**
        *   **Steer the ship North (000°) or South (180°) by the reference.**
        *   Read the deviation on the magnetic compass.
        *   Adjust the **athwartships (C) corrector magnets** until the deviation is zero.

3.  **Remove Quadrantal Deviation (Coefficient D):**
    *   **Steer the ship on an intercardinal heading: Northeast (045°) or Southwest (225°).**
    *   Read the remaining deviation.
    *   Adjust the **quadrantal spheres (D correctors)**. Move them closer to the compass to increase the correction or further away to decrease it. Adjust until the deviation is eliminated or minimized.
    *   Verify the correction on another intercardinal heading (e.g., Southeast 135°).

#### **Step 3: Creating the Deviation Card**

After the physical correctors have been adjusted, it's impossible to remove *all* the deviation on every heading. The ship is swung again, and the small remaining **residual deviation** is recorded on every 10° or 15° of heading.

This data is used to create a **Deviation Card** or **Deviation Table**, which is posted near the helm. This card shows the navigator what deviation to expect on any given heading.

**Example Deviation Card:**

| Ship's Head (Compass) | Deviation | Ship's Head (Compass) | Deviation |
| :-------------------- | :-------- | :-------------------- | :-------- |
| 000°                  | 1.0° E    | 180°                  | 1.5° W    |
| 015°                  | 0.5° E    | 195°                  | 2.0° W    |
| 030°                  | 0.0°      | 210°                  | 2.5° W    |
| ...etc.               | ...       | ...etc.               | ...       |

---

### **Part 3: Practical Application for the Navigator**

Once the compass is adjusted and the deviation card is created, the navigator must use it to convert between True, Magnetic, and Compass headings.

The common mnemonics are essential:

*   **T V M D C** ("**T**rue **V**irgins **M**ake **D**ull **C**ompany") - For converting from a True course (from the chart) to a Compass course (to steer). **Add West** variation/deviation, **Subtract East**.
*   **C D M V T** ("**C**an **D**ead **M**en **V**ote **T**wice?") - For converting a Compass bearing (observed) to a True bearing (to plot on the chart). **Add East** variation/deviation, **Subtract West**.

**Example:**
You want to steer a course of **245° True**.
*   **T**rue Course: **245°**
*   **V**ariation (from chart): **10° West**
    *   245° + 10° = **255° Magnetic** (This is your target magnetic heading)
*   **M**agnetic Course: **255°**
*   **D**eviation (from deviation card for heading ~255°): **3° East**
    *   255° - 3° = **252° Compass**
*   **C**ompass Course to Steer: **252°**

### **When is Compass Adjustment Required?**

According to SOLAS, a magnetic compass should be professionally adjusted:

*   After it is first installed.
*   After any major structural work or repairs that could affect its magnetic field.
*   After the vessel has been laid up or aground.
*   After new equipment (especially electrical) is installed near the compass.
*   If the recorded deviations are found to be excessive (generally > 5°).
*   At regular intervals (e.g., every one or two years) as a matter of good practice and company policy.