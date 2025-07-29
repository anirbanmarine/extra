---
title: Marine Magnetic Compass adjustment:different methods of swinging ship to obtain
  a deviation table;
type: docs
sidebar:
  open: true
---

Of course. This is an excellent and fundamental topic in marine navigation.

Swinging the ship (or "swinging the compass") is the process of determining the deviation of a vessel's magnetic compass on various headings. This deviation is caused by the ship's own magnetic field (from its steel hull, engines, electrical systems, etc.) interfering with the Earth's magnetic field.

The ultimate goal is to create a **Deviation Table** (or a Deviation Card), which allows the navigator to convert between Compass Headings and Magnetic Headings, ensuring safe navigation.

Here is a breakdown of the process and the different methods used.

---

### **Core Principle of All Methods**

No matter the method, the fundamental principle is the same:

1.  **Steady the ship** on a specific heading.
2.  **Observe a bearing** of an object using the ship's magnetic compass (this is the **Compass Bearing - CB**).
3.  **Simultaneously, determine the correct bearing** of that same object (either the **Magnetic Bearing - MB** or the **True Bearing - TB**).
4.  **Calculate the deviation** for that heading.
5.  **Repeat** this process for multiple headings, typically every 15° or 30°, covering a full 360° circle.

The core formula used is a rearrangement of the mnemonic **"True Virgins Make Dull Company At Weddings"** (True - Variation - Magnetic - Deviation - Compass).

*   If you have a **True Bearing (TB)**:
    *   Compass Error = TB - CB
    *   **Deviation = Compass Error - Variation** (remembering signs: East Variation is +, West is -)

*   If you have a **Magnetic Bearing (MB)**:
    *   **Deviation = MB - CB**

---

### **Methods of Swinging the Ship**

The methods differ in how they establish the "correct" reference bearing (the True or Magnetic bearing).

#### **Method 1: Comparison with a Gyrocompass (Most Common Modern Method)**

This is the fastest and most widely used method for ships equipped with a properly functioning gyrocompass.

*   **Principle:** A gyrocompass points to True North, not Magnetic North. After accounting for any small gyro error, it provides a perfect True reference from which deviation can be calculated.
*   **Procedure:**
    1.  **Determine Gyro Error:** Before the swing, the gyro error must be determined accurately (e.g., by observing a transit, or a celestial body azimuth). Let's say the gyro error is 1° East (meaning the gyro reads 1° higher than True).
    2.  **Commence Swing:** Slowly turn the ship in a circle.
    3.  **Take Readings:** On each desired heading (e.g., 000°, 015°, 030°...), steady the ship. At the same moment, one person reads the ship's heading from the magnetic compass, and another reads the heading from the gyrocompass.
    4.  **Calculate Deviation:** For each data point:
        *   Gyro Heading (GH): 030°
        *   Gyro Error (GE): 1°E (+)
        *   True Heading (TH) = GH - GE = 030° - 1° = 029°
        *   Variation (from chart for the area): 5°W (-)
        *   Magnetic Heading (MH) = TH - Var = 029° - (-5°) = 034°
        *   Compass Heading (CH): 032°
        *   **Deviation = MH - CH = 034° - 032° = 2° East (or +2°)**
    5.  Repeat for all headings and tabulate the results.
*   **Advantages:** Fast, efficient, can be done in open water, day or night, and doesn't require landmarks.
*   **Disadvantages:** Entirely dependent on the accuracy of the gyrocompass and the determination of its error.

#### **Method 2: Using a Known Transit (or Range)**

This is a highly accurate method but is geographically limited. A transit is when two charted, fixed objects are seen in a line.

*   **Principle:** The line of sight over two fixed, charted objects provides a constant, known True Bearing.
*   **Procedure:**
    1.  **Identify a Transit:** Find two objects on the nautical chart that can be lined up (e.g., two lighthouses, a buoy and a shore beacon, two prominent headlands). Plot the line on the chart and determine its True Bearing.
    2.  **Position the Ship:** Manoeuvre the ship to a position where it can cross this transit line multiple times at different angles.
    3.  **Take Bearings:** As the ship crosses the transit line on a steady heading, an observer takes a bearing of the transit using the magnetic compass's azimuth ring or bearing circle.
    4.  **Calculate Deviation:**
        *   True Bearing of Transit (from chart): 125°T
        *   Compass Bearing of Transit (observed): 131°C
        *   Compass Error = TB - CB = 125° - 131° = -6° (or 6°W)
        *   Variation (from chart): 5°W (-)
        *   **Deviation = Compass Error - Variation = -6° - (-5°) = -1° (or 1°W)**
    5.  Repeat this for as many headings as possible.
*   **Advantages:** Extremely accurate reference. No gyro needed.
*   **Disadvantages:** Requires suitable, charted objects. Limited to specific coastal areas. Can be time-consuming.

#### **Method 3: Bearing of a Distant Object**

This is a variation of the transit method, using a single object.

*   **Principle:** If an object is sufficiently far away (at least 6-10 miles), its bearing will not change significantly as the ship swings in a small circle.
*   **Procedure:**
    1.  **Select Object & Position:** Choose a single, distinct, charted object on shore (e.g., a mountain peak, a tower). Position the ship where it can swing in a circle without the object's bearing changing due to parallax.
    2.  **Determine Reference Bearing:** From the center of your planned swinging circle, determine the True Bearing of the object from the chart.
    3.  **Swing and Observe:** Swing the ship, and on each steady heading, take a bearing of the distant object with the magnetic compass.
    4.  **Calculate Deviation:** The calculation is identical to the Transit Method.
*   **Advantages:** Simpler than finding a transit.
*   **Disadvantages:** Prone to parallax error if the object is not far enough away or the swinging circle is too large. Finding a suitable, isolated object can be difficult.

#### **Method 4: Sun's Azimuth (Celestial Navigation)**

This is the classic, traditional method that can be used anywhere in open sea.

*   **Principle:** The True Bearing (Azimuth) of the sun can be calculated for any given time (GMT) and position (Lat/Long). This calculated True Bearing is then compared to the observed compass bearing of the sun.
*   **Procedure:**
    1.  **Prerequisites:** Requires a clear view of the sun, an accurate chronometer (GMT), the ship's position, a sextant (for older methods) or azimuth ring, and the Nautical Almanac/Sight Reduction Tables (or navigation software).
    2.  **Swing and Observe:** As the ship is steadied on a heading, an observer takes a bearing of the sun using the compass. The exact GMT of the observation is noted.
    3.  **Calculate True Azimuth:** Using the GMT, date, and ship's position, the navigator calculates the sun's True Azimuth.
    4.  **Calculate Deviation:** The calculation is identical to the Transit Method.
        *   Calculated True Azimuth of Sun: 275°T
        *   Observed Compass Bearing of Sun: 271°C
        *   Compass Error = 275° - 271° = 4° East
*   **Advantages:** The ultimate independent reference. Can be done anywhere, anytime the sun is visible and not too high in the sky.
*   **Disadvantages:** Requires skill in celestial navigation. Slower than the gyro method. Cannot be done in overcast weather.

#### **Method 5: Reciprocal Bearings**

This method is less common today and requires coordination with a shore station.

*   **Principle:** A bearing is taken from the ship to a shore compass, while simultaneously a bearing is taken from the shore compass to the ship. The reverse of the shore bearing is the correct Magnetic Bearing from the ship.
*   **Procedure:**
    1.  **Set Up:** A calibrated compass (pelorus or another magnetic compass) is set up on shore in a location free from magnetic influence. Communication is established with the ship.
    2.  **Take Bearings:** On a signal, observers on the ship and on shore take bearings of each other.
    3.  **Calculate Deviation:**
        *   Shore compass bearing to ship: 270°
        *   Reciprocal (correct magnetic bearing from ship): 270° - 180° = 090° (MB)
        *   Ship's compass bearing to shore: 088° (CB)
        *   **Deviation = MB - CB = 090° - 088° = 2° East**
*   **Advantages:** Directly measures deviation without needing to involve Variation.
*   **Disadvantages:** Requires a shore party, good communication, and a suitable location. Rarely used in commercial shipping.

### **Final Step: Creating the Deviation Table**

Once the deviations are calculated for all headings, they are tabulated. A professional compass adjuster will also use this data to calculate the magnetic **Coefficients (A, B, C, D, E)** and physically adjust the compass correctors (Flinders bar, quadrantal spheres, heeling magnets) to reduce the deviation as much as possible before producing the final card.

A simple deviation table would look like this:

| Ship's Head (Compass) | Deviation | Ship's Head (Compass) | Deviation |
| :-------------------- | :-------- | :-------------------- | :-------- |
| 000°                  | 2°W       | 180°                  | 3°E       |
| 015°                  | 1°W       | 195°                  | 4°E       |
| 030°                  | 0°        | 210°                  | 5°E       |
| ...etc                | ...       | ...etc                | ...       |
| 165°                  | 2°E       | 345°                  | 1°W       |