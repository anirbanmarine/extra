---
title: Marine Magnetic Compass adjustment:construction of a curve of deviations and
  its practical use in coefficient analysis· constant, semi-circular, and quadrantal
  deviation;
type: docs
sidebar:
  open: true
---

Of course. This is an excellent and fundamental topic in marine navigation. Let's break down the process of creating and using a deviation curve and analyzing the coefficients.

### **Introduction: The Core Problem**

A magnetic compass points to the Magnetic North Pole. This direction is affected by two main errors:

1.  **Variation:** The angle between True North and Magnetic North. This is a geographical error, found on navigational charts.
2.  **Deviation:** The angle between the Magnetic North line and where the compass needle actually points. This error is caused by the ship's own magnetic field (its steel hull, engines, electrical equipment, etc.).

Compass adjustment is the process of minimizing **deviation** and then documenting the remaining, unavoidable error on a **deviation card or curve**.

---

### **Part 1: Construction of a Curve of Deviations**

This is the practical, hands-on part of the process, often called **"Swinging the Ship."** The goal is to measure the deviation on various headings.

#### **Procedure: Swinging the Ship**

1.  **Preparation:**
    *   **Location:** Choose an area with calm seas, little to no wind, and a clear view of landmarks or the sky. The water depth must be sufficient for maneuvering.
    *   **Ship's Condition:** The ship should be in its normal seagoing condition. Derricks stowed, all movable magnetic material in its usual place, and all electrical equipment that might affect the compass turned on.
    *   **Reference Heading:** You need a reliable, independent way to know the ship's true heading. This is typically done using:
        *   A calibrated **Gyrocompass**.
        *   **Transit Bearings:** Aligning two fixed shore objects.
        *   **Reciprocal Bearings** with a compass on shore.
        *   **Celestial Bearings** of the sun or other celestial bodies.

2.  **The Swing:**
    *   The ship is slowly turned in a complete 360° circle.
    *   At steady intervals (typically every 15° or 30°), the process is paused.
    *   At each pause, two readings are taken simultaneously:
        *   The **Ship's Head by Magnetic Compass**.
        *   The **"Correct" Magnetic Heading**. This is derived from your reference. For example, if using a gyrocompass: `Gyro Heading + Variation = Correct Magnetic Heading`.

3.  **Recording the Data:** The readings are recorded in a table.

| Ship's Head (by Gyro) | Variation (from Chart) | **Correct Magnetic Head (A)** | Ship's Head (by Compass) **(B)** | **Deviation (A - B)** |
| :-------------------- | :--------------------- | :---------------------------- | :------------------------------- | :-------------------- |
| 000°                  | 3°W (-3)               | 357°                          | 355°                             | **2°W (-2°)**         |
| 030°                  | 3°W (-3)               | 027°                          | 028°                             | **1°E (+1°)**         |
| 060°                  | 3°W (-3)               | 057°                          | 053°                             | **4°E (+4°)**         |
| 090°                  | 3°W (-3)               | 087°                          | 082°                             | **5°E (+5°)**         |
| 120°                  | 3°W (-3)               | 117°                          | 114°                             | **3°E (+3°)**         |
| 150°                  | 3°W (-3)               | 147°                          | 148°                             | **1°W (-1°)**         |
| 180°                  | 3°W (-3)               | 177°                          | 180°                             | **3°W (-3°)**         |
| ...and so on for 360° | ...                    | ...                           | ...                              | **...**               |

*Note: Easterly deviation is named (+) and Westerly is named (-).*

4.  **Plotting the Curve:**
    *   Draw a graph.
    *   The **X-axis** is the **Ship's Head by Compass**.
    *   The **Y-axis** is the **Deviation**. Easterly (+) deviations are plotted above the line, and Westerly (-) deviations are plotted below.
    *   Plot the points from your table.
    *   Draw a smooth, flowing curve that best fits the plotted points.

