---
title: '15. Compass adjustment:'
type: docs
sidebar:
  open: true
---

Excellent topic. "Compass adjustment" is a critical procedure in maritime and aviation navigation for ensuring the accuracy of a magnetic compass.

Here is a comprehensive explanation of compass adjustment, covering the what, why, and how.

---

### **Compass Adjustment**

**1. What is Compass Adjustment?**

Compass adjustment is the process of correcting for **deviation**—the magnetic error caused by the ship or aircraft itself. The goal is not to eliminate deviation completely (which is often impossible) but to reduce it to a minimum and then create a table of the remaining errors so they can be accounted for in navigation.

This process is often called **"swinging the compass"** or **"swinging the ship."**

**2. Why is it Necessary? The Two Magnetic Errors**

A magnetic compass points to Magnetic North, not True North. To navigate accurately, a user must account for two distinct errors:

*   **Variation (or Declination):** This is the angle between True North (the geographic North Pole) and Magnetic North. It is a natural, geographic error that varies depending on your location on Earth. Variation is found on nautical or aeronautical charts and is applied as a known correction. **You cannot adjust the compass for variation.**

*   **Deviation:** This is the error caused by the magnetic fields of the vessel or aircraft itself. Large metal components (the hull, engine), electrical equipment, and even cargo can create their own magnetic fields that "pull" the compass needle away from Magnetic North. This error changes as the vessel changes its heading. **This is the error that compass adjustment corrects.**

> **In short:** Variation is the Earth's error. Deviation is the ship's error. Compass adjustment deals with the ship's error.

**3. The Process: Swinging the Compass**

The adjustment is performed by a licensed Compass Adjuster. The general procedure is as follows:

1.  **Preparation:** All equipment that might affect the compass (engines, generators, radar) should be running as it would be during normal operation. Any large magnetic objects near the compass should be in their usual seagoing positions.
2.  **Swinging:** The vessel is slowly turned through a full 360 degrees.
3.  **Observation:** At various headings (usually every 15 or 30 degrees), the compass reading is compared to the known correct magnetic heading. This "known" heading can be determined by:
    *   **Leading Marks (Transits):** Aligning two fixed objects on shore whose magnetic bearing is known from a chart.
    *   **Gyrocompass:** Comparing the magnetic compass to a gyrocompass (which points to True North and is unaffected by magnetism).
    *   **Celestial Bearings:** Taking a bearing of the sun or another celestial body at a specific time and calculating its true bearing.
4.  **Adjustment:** Based on the observed errors (the deviation), the adjuster uses various correctors built into the compass binnacle to counteract the ship's magnetic fields.

**4. The Tools: The Correctors**

The standard compass binnacle is equipped with several correctors to counteract the different components of the ship's magnetism:

*   **Fore-and-Aft Magnets:** Small permanent magnets placed in a holder running parallel to the ship's centerline. They correct for permanent magnetism in the athwartships (port-starboard) direction.
*   **Athwartships Magnets:** Permanent magnets placed perpendicular to the ship's centerline. They correct for permanent magnetism in the fore-and-aft direction.
*   **Quadrantal Spheres (Kelvin's Balls):** Two soft iron spheres mounted on either side of the compass. They correct for magnetism induced in the ship's horizontal soft iron, which causes errors on the quadrantal headings (NE, SE, SW, NW).
*   **Flinders Bar:** A vertical bar of soft iron placed in a case on the fore or aft side of the binnacle. It corrects for magnetism induced in the ship's vertical soft iron.
*   **Heeling Magnet:** A vertical magnet placed directly underneath the compass card pivot. It corrects for errors that occur when the ship is heeling (rolling).

**5. The Result: The Deviation Card**

After the adjuster has minimized the deviation using the correctors, the small remaining errors are recorded on a **Deviation Card** (or Deviation Table). This card is posted near the helm for the navigator to use.

A typical deviation card looks like this:

| Ship's Head (Compass) | Deviation |
| :-------------------- | :-------- |
| 000°                  | 2° E      |
| 015°                  | 1° E      |
| 030°                  | 0°        |
| 045°                  | 1° W      |
| ... (and so on)       | ...       |
| 345°                  | 1° E      |

The navigator uses this card to find the deviation for their current heading and apply it to their calculations.

**6. Practical Application: The TVMDC Rule**

To convert a True course (from a chart) to a Compass course (to steer), or vice versa, navigators use a simple mnemonic.

**T**rue **V**irgins **M**ake **D**ull **C**ompany
(True - Variation - Magnetic - Deviation - Compass)

*   **Correcting (Compass to True):** When you go "up" the list from Compass to True, you **ADD** Easterly errors and **SUBTRACT** Westerly errors.
    *   Mnemonic: **C**an **D**ead **M**en **V**ote **T**wice?

*   **Un-correcting (True to Compass):** When you go "down" the list from True to Compass, you **SUBTRACT** Easterly errors and **ADD** Westerly errors. (The opposite of above).
    *   A common rhyme for this direction: "Error East, Compass Least. Error West, Compass Best."

**Example:**
A ship wants to steer a **True** course of **085°**.
Variation from the chart is **10° W**.
Deviation from the card for that heading is **3° E**.
What is the Compass course to steer?

1.  **T**rue: 085°
2.  **V**ariation: 10° W  (West is Added when going down)
    *   085° + 10° = 095°
3.  **M**agnetic: 095°
4.  **D**eviation: 3° E (East is Subtracted when going down)
    *   095° - 3° = 092°
5.  **C**ompass: **092°**

The helmsman must steer **092°** by the ship's compass to travel along a true course of 085°.