---
title: Discuss with respect to celestial navigation the equation of equal altitudes
  (above and below pole, etc.) of celestial bodies
type: docs
sidebar:
  open: true
---

Of course. This is an excellent topic that gets to the heart of classical celestial navigation. The "Equation of Equal Altitudes" refers to a method, and the underlying mathematical formulas, used to determine a navigator's latitude. The key principle is observing a celestial body at two different times when it has the exact same altitude.

Let's break down the concept, the different scenarios (including above and below the pole), and the relevant equations.

### The Fundamental Principle

Imagine a celestial body (like the Sun or a star). At any given moment, it is directly overhead at one point on Earth's surface. This is called its **Geographical Position (GP)** or sub-stellar point.

Now, imagine drawing a circle on the Earth centered on that GP. For any observer located anywhere on this circle, the celestial body will appear at the exact same altitude in the sky. This is called a **Circle of Equal Altitude**. A navigator's single sight (measuring altitude) tells them they are somewhere on this circle.

The method of equal altitudes uses two such observations:

1.  An observer measures the altitude of a body (e.g., the Sun as it's rising) and notes the time. This places them on a specific Circle of Equal Altitude.
2.  The observer waits. The body continues its path across the sky.
3.  The observer notes the exact time when the body returns to the *very same altitude* (e.g., as the Sun is setting). This places them on a *second* Circle of Equal Altitude.

Since the navigator is on both circles, their position must be at one of the two intersection points of these circles. The ambiguity between the two points is easily resolved because a navigator has a rough idea of their location.

The line connecting these two intersection points is a **Line of Position (LOP)**. In the specific, symmetrical case discussed below, this LOP has a very special property: it is the observer's meridian of longitude, a true North-South line.

### The PZX Triangle: The Key to the Math

All celestial navigation formulas are derived from the **PZX Triangle**, an imaginary spherical triangle on the celestial sphere:

*   **P:** The elevated celestial pole (North or South Pole, depending on your hemisphere).
*   **Z:** The Zenith (the point directly above the observer).
*   **X:** The position of the celestial body.

The sides and angles of this triangle are:
*   **Side PZ:** Co-latitude of the observer (90° - Latitude).
*   **Side PX:** Polar Distance or Co-declination of the body (90° - Declination).
*   **Side ZX:** Zenith Distance or Co-altitude of the body (90° - Altitude).
*   **Angle at P (ZPX):** The Hour Angle (H.A.) of the body.
*   **Angle at Z (PZX):** The Azimuth (true bearing) of the body.

Using the spherical law of cosines on this triangle gives the fundamental navigation equation:
**sin(Alt) = sin(Lat) sin(Dec) + cos(Lat) cos(Dec) cos(H.A.)**

This is the equation we manipulate for the method of equal altitudes.

---

### Case 1: Symmetrical Observations Around the Meridian (Upper Transit)

This is the most common application of the method, often called the **Ex-Meridian method**.

**The Procedure:**
1.  In the morning, an observer measures the altitude of the Sun (or a star) before it reaches its highest point (meridian transit). Let's call this Altitude `Alt` and the time `T1`.
2.  The observer waits for the body to cross the local meridian.
3.  In the afternoon, the observer waits for the Sun to descend to the *exact same altitude* (`Alt`) and notes the time `T2`.

**The Geometry and the "Equation":**
Because the two observations were made at the same altitude and, for a short period, the body's declination is considered constant, the PZX triangles at times T1 and T2 are mirror images of each other. The situation is symmetrical around the observer's meridian.

This symmetry means the Line of Position (LOP) derived from these two sights is the observer's meridian itself—a perfect North-South line. This method, therefore, gives a very accurate **Latitude**, but provides no information about Longitude.

The equation to find latitude is derived from the main navigation formula. Let `h` be half of the elapsed **hour angle** between the two sights.
*   Elapsed Time = `T2 - T1`
*   Elapsed Hour Angle = `Elapsed Time (in hours) * 15°/hour`
*   `h` = `Elapsed Hour Angle / 2`

The governing equation relating the knowns (`Alt`, `Dec`, `h`) to the unknown (`Lat`) is:

**cos(h) = [ sin(Alt) - sin(Lat) sin(Dec) ] / [ cos(Lat) cos(Dec) ]**

This equation can be tricky to solve directly for `Lat` on paper. However, it can be rearranged into various forms for use with tables (like in Bowditch) or solved easily with a calculator. A common rearrangement is:
**sec(Lat) sec(Dec) sin(Alt) - tan(Lat) tan(Dec) = cos(h)**

The key takeaway is that with two equal altitudes taken symmetrically around noon, and knowing the body's declination, you can calculate your latitude without needing a precise chronometer to know your longitude.

---

### Case 2: Observations "Above and Below Pole" (Circumpolar Bodies)

This is a special and very powerful application of the equal altitude principle, primarily used by navigators in high latitudes. A **circumpolar body** is one that never sets below the horizon. It crosses the meridian twice in 24 hours:
*   **Upper Transit:** Its highest point, "above the pole."
*   **Lower Transit:** Its lowest point, "below the pole."

#### A) Symmetrical Observations Around Lower Transit

This is geometrically identical to Case 1. An observer in the Arctic could observe a star as it descends towards its lowest point, note the altitude and time, and then observe it again after it passes the lower transit and rises to the same altitude. The resulting LOP is again the meridian, and the same formula applies to find Latitude.

#### B) The Ultimate Equation of Equal Altitudes: Altitudes at Both Transits

This is the most elegant application of the principle. It requires observing the same circumpolar star at its maximum and minimum altitudes.

**The Procedure:**
1.  Measure the altitude of a circumpolar star at its **Upper Transit** (highest point). Let this be `Alt_U`.
2.  Wait approximately 12 hours.
3.  Measure the altitude of the same star at its **Lower Transit** (lowest point). Let this be `Alt_L`.

**The Geometry and the Equation:**
Let's consider the geometry at the meridian (see diagram below).
*   The altitude of the celestial pole is equal to the observer's latitude (`Alt_P = Lat`).
*   The polar distance of the star is `p = 90° - Dec`.

At **Upper Transit**, the star is above the pole, so its altitude is the altitude of the pole plus its polar distance from the pole.
`Alt_U = Lat + p`

At **Lower Transit**, the star is below the pole, so its altitude is the altitude of the pole minus its polar distance.
`Alt_L = Lat - p`

