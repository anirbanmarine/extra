---
title: Discuss with respect to celestial navigation Meridional part
type: docs
sidebar:
  open: true
---

Of course. Let's have a detailed discussion about Meridional Parts, a crucial concept in celestial and marine navigation. We'll cover what they are, the problem they solve, how they are calculated, and their practical application.

---

### 1. The Fundamental Problem: Earth is a Sphere, Charts are Flat

At the heart of navigation lies a geometric challenge: representing the curved surface of the Earth on a flat piece of paper (a chart).

*   **Great Circles:** The shortest distance between two points on a sphere is a **Great Circle** (a circle whose center is the center of the Earth, like the Equator or any meridian of longitude). A great circle track, however, constantly changes its true bearing (except when traveling along the Equator or a meridian). This makes it difficult to steer.
*   **Rhumb Lines (Loxodromes):** A **Rhumb Line** is a line on the Earth's surface that crosses all meridians at the same constant angle. If you steer a constant compass course, you are following a rhumb line. While slightly longer than a great circle path, it is much easier to navigate. On a globe, a rhumb line is a spiral that winds towards the poles.

The ideal chart for a navigator would be one where this easy-to-steer rhumb line appears as a simple **straight line**. This is exactly what the **Mercator Projection** achieves.

### 2. The Solution: The Mercator Projection

The Mercator chart was a revolutionary invention for navigators. It's constructed with two key properties:

1.  **Meridians of longitude** are drawn as equally spaced, parallel vertical lines.
2.  **Parallels of latitude** are drawn as parallel horizontal lines.

However, on the real Earth, meridians converge at the poles. By making them parallel on the chart, the Mercator projection inherently **stretches all east-west distances**. This stretching becomes more and more extreme as you move away from the equator.

To keep the chart **conformal** (meaning angles and shapes of small areas are preserved correctly), the north-south distances must be stretched by the **exact same proportion** at any given latitude.

This is where Meridional Parts come in.

### 3. Defining Meridional Parts (M or Mer. Parts)

A **Meridional Part** is a mathematical value that quantifies this necessary north-south stretching on a Mercator chart.

> **Definition:** The meridional part for a given latitude is the length of the arc of a meridian on a Mercator chart, measured from the Equator to that latitude, expressed in units of minutes of longitude at the Equator.

Let's break that down:
*   **Unit of Measurement:** The baseline unit is one minute of longitude *at the Equator*. On a Mercator chart, this east-west distance is constant everywhere.
*   **Stretched Distance:** The meridional part tells you how many of these "equatorial longitude units" you would need to stack vertically to reach a specific latitude on the stretched-out chart.

**Analogy:** Imagine the Mercator chart is made of rubber. It's not stretched at the Equator. As you pull it north and south to make the meridians parallel, the N-S distance increases. The Meridional Part is the new, stretched "ruler measurement" from the Equator (latitude 0°) to your latitude of interest.

| Latitude | True Distance from Equator | Meridional Part (approx.) |
| :--- | :--- | :--- |
| 0° | 0 NM | 0.0 |
| 10° | 600 NM (10° * 60 NM/°) | 603.6 |
| 45° | 2700 NM (45° * 60 NM/°) | 3030.3 |
| 60° | 3600 NM (60° * 60 NM/°) | 4527.4 |
| 80° | 4800 NM (80° * 60 NM/°) | 7808.8 |

Notice how the meridional parts increase much faster than the true distance (measured in nautical miles, which are minutes of latitude). This reflects the increasing stretch of the Mercator chart.

### 4. How are Meridional Parts Used? The Sailing Triangle

The genius of meridional parts is that they allow us to use simple plane trigonometry to solve navigation problems on a curved surface. This is called **Mercator Sailing**.

We construct a right-angled triangle on the plane of the Mercator chart:

*   **Adjacent Side:** The north-south distance on the chart. This is **not** the true difference in latitude (dLat). Instead, it is the **Difference of Meridional Parts (DMP)**.
    `DMP = Mer. Part of Lat₂ - Mer. Part of Lat₁`
*   **Opposite Side:** The east-west distance on the chart. Since meridians are parallel, this is simply the **Difference of Longitude (dLo)**, expressed in minutes of arc.
*   **Angle:** The **Course Angle (C)**.
*   **Hypotenuse:** This represents the distance *on the chart*, not the true distance over the ground.

