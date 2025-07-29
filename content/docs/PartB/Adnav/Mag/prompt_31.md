---
title: Marine Magnetic Compass adjustment:analysis of a ship's deviation book to determine
  causes of irregular deviations and suggest measures for their removal;
type: docs
sidebar:
  open: true
---

Excellent and very practical question. Analyzing a ship's deviation book for irregularities is a core skill for a competent navigating officer and a compass adjuster. It's a classic case of nautical detective work.

Here is a comprehensive analysis of how to approach this task, broken down into a systematic process.

---

### **Part 1: The Fundamentals - What We Expect to See**

Before identifying what is "irregular," we must understand what "regular" deviation looks like.

1.  **The Nature of Regular Deviation:** A properly functioning magnetic compass on a steel ship will have deviation caused by the ship's own magnetic field. This field is a combination of:
    *   **Permanent Magnetism (Hard Iron):** Acquired during the ship's construction. This causes **Semicircular Deviation**, which is maximum on two opposite headings (e.g., North and South) and zero on two other headings (e.g., East and West). This is corrected by permanent magnets (Coefficients B and C).
    *   **Induced Magnetism (Soft Iron):** Magnetism induced in the ship's soft iron structures by the Earth's magnetic field. This causes **Quadrantal Deviation**, which is maximum on the four intercardinal headings (NE, SE, SW, NW) and zero on the cardinal headings (N, S, E, W). This is corrected by soft iron spheres or a Flinders bar (Coefficients D and E).

2.  **The Deviation Curve:** When you plot the deviation values from the book against the ship's head, the result should be a smooth, wave-like (sinusoidal) curve. This curve can be mathematically described by the approximate coefficients A, B, C, D, and E.

    *   **A "Regular" Deviation Book:** The values change progressively and predictably as the ship turns through 360 degrees.

### **Part 2: The Analysis - Identifying Irregular Deviations**

"Irregular" deviation is any deviation that does not fit this smooth, predictable sinusoidal pattern. Your analysis of the deviation book should follow these steps:

#### **Step 1: Data Scrutiny and Plotting**

1.  **Gather the Data:** Take the deviation book or deviation card. Note the date of the last adjustment and the conditions under which the observations were made (e.g., location, sea state, cargo status).
2.  **Plot the Curve:** This is the single most important step.
    *   Use graph paper or a spreadsheet.
    *   **X-axis:** Ship's Head by Compass (000° to 360°).
    *   **Y-axis:** Deviation (label East deviations as '+' and West deviations as '-').
    *   Plot each recorded point from the deviation book.

#### **Step 2: Analyzing the Plotted Curve**

Now, look at the pattern of the plotted points. Do they form a smooth curve? Or do you see any of the following signs of irregularity?

*   **Sudden Spikes or Dips:** A single point or a small group of points that are dramatically different from their neighbours.
*   **Scattered Points:** The points do not form any discernible curve at all; they are randomly scattered.
*   **Flat Spots or Kinks:** The curve is smooth in some areas but suddenly flattens or has a sharp, unnatural bend in another.
*   **Inconsistent Readings:** The deviation recorded on a heading one day is vastly different from a reading taken on the same heading a few days later under similar conditions.

---

### **Part 3: Diagnosing the Causes of Irregular Deviations**

Once an irregularity is identified, the next step is to diagnose the cause. Here are the most common culprits, linked to the visual clues from your graph.

| **Observation (from Plotted Curve)** | **Likely Cause(s)** | **Explanation** |
| :--- | :--- | :--- |
| **1. A Single, Large Spike/Dip on one heading.** | **Moveable Magnetic Material or Electrical Interference.** | A temporary magnetic field was present when that specific bearing was taken. The most common cause is a piece of steel equipment being moved near the binnacle. Examples: a crane swung outboard, a steel lifeboat davit moved, a portable grinder, or a crew member placing a toolbox or radio next to the compass. |
| **2. Multiple Randomly Scattered Points.** | **1. Poor Observation Technique.**<br>**2. Sluggish Compass.**<br>**3. Loose Correctors.** | **1. Poor Technique:** The ship was not held steady on the heading, the azimuth mirror was not used correctly, or there were calculation errors. Rough seas can also cause this. <br>**2. Sluggish Compass:** The compass card is sticking due to a worn pivot or a bubble in the liquid. It doesn't respond smoothly to changes in heading. <br>**3. Loose Correctors:** The magnets or soft iron spheres inside the binnacle have worked loose and are shifting position, creating an unstable correcting field. |
| **3. Deviations consistently larger than expected, but curve shape is roughly okay.** | **1. Major Change in Ship's Magnetism.**<br>**2. Incorrect or Outdated Variation.** | **1. Change in Magnetism:** The ship has undergone major structural work (welding), been struck by lightning, carried a highly magnetic cargo (scrap metal, iron ore), or has been laid up on a single heading for a long period. The old deviation card is no longer valid. <br>**2. Calculation Error:** The variation used to calculate the deviation was wrong for the ship's location. |
| **4. Erratic behaviour when specific equipment is used.** | **Electrical Interference.** | The deviation "kicks" when the radar starts transmitting, the HF radio is used, or a high-power deck light is switched on. This is caused by unshielded wiring or strong electromagnetic fields near the compass. DC current is a notorious offender. |
| **5. The whole curve has shifted up or down (a large Coefficient A).** | **1. Misaligned Lubber Line.**<br>**2. Observational Bias.**<br>**3. Asymmetrically placed magnetic material.** | The lubber line on the compass bowl is not perfectly aligned with the ship's fore-and-aft line. Alternatively, the observer consistently stands in the same spot with keys/radio, creating a constant offset. |

---

### **Part 4: Suggesting Measures for Removal and Correction**

Based on the diagnosis, you can suggest specific actions. **The primary rule is to remove the source of the irregular deviation before attempting to re-adjust the compass.** You cannot correct for an unstable field.

#### **Immediate Actions & Investigations**

1.  **Establish a "Circle of No Offence":**
    *   **Action:** Paint a circle of 2-3 meters radius around the binnacle.
    *   **Rule:** Enforce a strict policy that NO magnetic or electronic items are to be placed or used inside this circle. This includes tools, radios, mobile phones, speakers, etc. This is the single most effective measure for preventing irregular deviations.

2.  **Inspect the Compass and Binnacle:**
    *   **Action:** Visually inspect the compass bowl. Is the liquid clear and free of bubbles? Does the card swing freely and settle quickly when deflected by a small magnet (held well away and then removed)?
    *   **Action:** Open the binnacle door. Check that the correcting magnets in their trays and the soft iron spheres on their brackets are securely fastened and have not shifted.

3.  **Standardize Ship's Conditions:**
    *   **Action:** Create a checklist for "Compass Observation Conditions." All future deviations should be observed with equipment in a standard sea-going state (e.g., cranes stowed, derricks lowered, metallic doors/hatches secured in their sea position).

4.  **Investigate Electrical Interference:**
    *   **Action:** Station an observer at the compass. Systematically switch on and off all major electrical equipment nearby, especially the radar, echo sounder, navigation lights, and deck lights. Note any deflection ("kick") of the compass card. If a circuit is identified, its wiring needs to be inspected for faults, and it may need to be re-routed or shielded.

#### **Long-Term Solutions & Recommendations**

1.  **If observational error or rough seas were the cause:**
    *   **Recommendation:** Wait for calm weather and good conditions. Re-swing the ship and observe a new set of deviations, ensuring a steady helm and careful observation.

2.  **If moveable magnetic objects were the cause:**
    *   **Recommendation:** Remove the offending object(s) permanently. Enforce the "Circle of No Offence." Observe a new deviation curve.

3.  **If the ship's magnetism has fundamentally changed (post-refit, lightning, etc.):**
    *   **Recommendation:** The current deviation card is **invalid and dangerous**. The ship **must** be swung and have its compass professionally re-adjusted by a certified compass adjuster. The adjuster will re-assess the permanent and induced magnetism and apply the correctors accordingly.

4.  **If the compass itself is faulty (sluggish, large bubble):**
    *   **Recommendation:** The compass must be repaired or replaced by a qualified technician.

### **Example Walkthrough**

**Deviation Book Entry:**
*   N: 2°E
*   NE: 10°E  *(<- Large jump)*
*   E: 4°E   *(<- Drops back)*
*   S: 3°W
*   W: 5°W

**Analysis:**
1.  **Plotting:** The plot would show a massive, sharp spike at NE that doesn't fit a smooth sine curve.
2.  **Diagnosis:** This is not quadrantal or semicircular deviation. It is a classic sign of a localized magnetic field affecting the compass primarily on that one heading. The most likely cause is a piece of steel near the starboard bow quadrant of the compass (e.g., a portable steel fitting, a fire extinguisher left out of place, a steel ladder lashed to the railings).
3.  **Suggested Measures:**
    *   **Immediate:** Conduct a thorough physical search of the bridge wings and area around the compass, particularly on the starboard side.
    *   **Follow-up:** Once the area is clear, steer a course of NE and check the deviation again. If it has returned to a more normal value (e.g., 3°E), the problem is solved.
    *   **Final:** A full new deviation table should be produced to ensure the integrity of the compass.